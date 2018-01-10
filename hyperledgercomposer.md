# Hyperledger Composer

Hyperledger Composer is an extensive, open development toolset and framework to make developing blockchain applications easier. 

Our primary goal is to accelerate time to value, and make it easier to integrate your blockchain applications with the existing business systems. 

You can use Composer to rapidly develop use cases and deploy a blockchain solution in weeks rather than months. Composer allows you to model your business network and integrate existing systems and data with your blockchain applications.

[Hyperledger Composer Mocdeling Language](https://hyperledger.github.io/composer/reference/cto_language.html)

Sample Business Networks:

<img src="https://farm5.staticflickr.com/4770/39618901931_01983c3d45_z.jpg" width="406" height="578" alt="Hyperledger Composer 1">

[Hyperledger Composer](https://composer-playground.mybluemix.net/editor)

# Datamodel for the Marble Trading Network

~~~
/**
 * Defines a data model for a marble trading network
 */
namespace org.hyperledger_composer.marbles

enum MarbleColor {
  o RED
  o GREEN
  o BLUE
  o PURPLE
  o ORANGE
}

enum MarbleSize {
  o SMALL
  o MEDIUM
  o LARGE
}

asset Marble identified by marbleId {
  o String marbleId
  o MarbleSize size
  o MarbleColor color
  --> Player owner
}

participant Player identified by email {
  o String email
  o String firstName
  o String lastName
}

transaction TradeMarble {
  --> Marble marble
  --> Player newOwner
}
~~~

# Let's play marbles!
In the test pane

<img src="https://farm5.staticflickr.com/4624/25748073888_82b8668a47_z.jpg" width="640" height="280" alt="Hyperledger Composer Test Pane">

create two Player participants
```
{
  "$class": "org.hyperledger_composer.marbles.Player",
  "email": "memberA@acme.org",
  "firstName": "Jenny",
  "lastName": "Jones"
}

{
  "$class": "org.hyperledger_composer.marbles.Player",
  "email": "memberB@acme.org",
  "firstName": "Billy",
  "lastName": "Thompson"
}
~~~

Create a Marble Asset:

~~~

{
  "$class": "org.hyperledger_composer.marbles.Marble",
  "marbleId": "marbleId:1234",
  "size": "SMALL",
  "color": "BLUE",
  "owner": "resource:org.hyperledger_composer.marbles.Player#email:memberA@acme.org"
}

Submit a Transaction:

~~~

{
  "$class": "org.hyperledger_composer.marbles.TradeMarble",
  "marble": "resource:org.hyperledger_composer.marbles.Marble#marbleId:1234",
  "newOwner": "resource:org.hyperledger_composer.marbles.Player#email:memberB@acme.org"
}


