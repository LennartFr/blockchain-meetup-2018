# Blockchain for developers: from zero to running app in the cloud. 
<a href="http://ibm.biz/bcmeetup2018"><img src="https://farm5.staticflickr.com/4739/39515037702_7c97e80df1_b.jpg" width="805" height="180" alt="bcmeetup2018"></a> 

# Speakers

## Lennart Frantzell 

Lennart is a Developer Advocate with IBM on the San Francisco City Team focusing on Blockhain and Fintech. With a background in program development he works with startups and developers to help them adopt Blockchain and Fintech, talks at industry events and spends his weekends at hackathons. 

## Raheel Zubairy

Raheel is a software Engineer focused on developing journeys for Emerging Technologies team, part of IBM’s Digital Business Group. He has worked on journeys showcasing Blockchain technologies and Fintech services. In addition, his interests include IoT and Data Science. Raheel’s previous experience includes over five years in the energy industry. He completed his bachelors and masters degrees from Texas A&M University. Raheel is an avid sports fan. 

# Agenda:

6:00-6:30pm: Light dinner and registration

6-30-8:30pm: Talks and demos: <p>
             Lennart: The Blockchain Building Blocks:  your first app, how do you deploy it. 
                      Overview of the latest programming resources.<br>                          
             Raheel: Writing Blockchain apps. An experience report. How to plan your app, how to write it, how to deploy it.
                                           
8:30-9:00pm : Wrap up & Networking

Requirements:

Bring a laptop

<img src="https://farm5.staticflickr.com/4622/38808577705_378b51940b_o.png" width="539" height="307" alt="Blockchain Dev"><p>
<a href="https://developer.ibm.com/blockchain/sandbox/">IBM Blockchain Sandbox</a>

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# How did it all start?
 
October 2008 It all started with Satoshi Nakamoto and his paper [Bitcoin: A Peer-to-Peer Electronic Cash System](https://bitcoin.org/bitcoin.pdf) which addressed a key problem in electronic commerce:

<img src="https://farm5.staticflickr.com/4505/24079519258_ab8a80f7ed_o.png" width="769" height="229" alt="Double Spending">
<p>
<i>
The first work on a cryptographically secured chain of blocks was described in 1991 by Stuart Haber and W. Scott Stornetta.[17] In 1992, Bayer, Haber and Stornetta incorporated Merkle trees to the design, which improved its efficiency by allowing several documents to be collected into one block.
  </i><p><i>
A blockchain database is managed autonomously using a peer-to-peer network and a distributed timestamping server. The first blockchain was conceptualised by an anonymous person or group known as Satoshi Nakamoto in 2008. 
</i><p>
https://en.wikipedia.org/wiki/Blockchain
<p>
<i>A blockchain is a decentralized virtual ledger for recording transactions without central authority through a distributed cryptographic protocol. It is made up of three technologies 

1. cryptographic algorithms, 
1. a distributed protocol, 
1. and replicated data 
<p>
which combined provide a trustworthy service to a group of nodes that do not fully trust each other. 
<p>
With blockchain, several users can write entries into a block or a record of information, and a community can control how the record of information is modified and updated.
</i>
Consensus protocol is pluggable, currently an implementation of Byzantine fault-tolerant consensus using the PBFT (Practical Byzantine Fault Tolerance) protocol.
<p>
Christian Cachin <a href="https://www.ibm.com/blogs/research/2017/10/resilient-consensus-protocols-blockchains/">Resilient Consensus Protocols for Blockchains</a>
<p>
Source: https://www.zurich.ibm.com/dccl/papers/cachin_dccl.pdf

## The Blockchain Distributed Ledger
<img src="https://www.ibm.com/blogs/internet-of-things/wp-content/uploads/2017/05/2-1.jpg">
<p>
  
  
## Blockchain main components 

### Ordering Service – Ordering and synchronizing transactions
... the ordering service is the definition of the network. It contains identity information for each member, information on channels and a set of policies dictating which members are permitted to perform certain tasks (e.g. invite other members, create channels, etc.). Every transaction and configuration operation will flow through the ordering service, so it’s a beyond critical piece in the overall scheme of things.......

###  Certificate Authority – Issuing certificates to participants
To put it simply, the Certificate Authority (CA) provides membership. All entities in the network (peers, orderers, clients, etc.) must have an identity to communicate, authenticate and ultimately transact. These “identities” exist in the form of x509 certificates (i.e. enrollment certificates), which are required for any direct participation in the blockchain network.... 

###  Peer – Validating/endorsing transactions
The peer exists to perform two main functions: execute/validate transactions & maintain ledgers. The peer runs smart contracts, and is the holder of transaction history and the current state of assets on the network’s channels. At the end of the day it’s all about accessing the peer (directly or indirectly) and performing reads and writes against the ledger. When a member provides an end user access to the network, they’re really providing access to the functionality of the peer.
<br>
https://console.bluemix.net/docs/services/blockchain/index.html#ibm-blockchain-platform
  
## Example of the importance of a shared ledger. <p> 
<a href="https://en.wikipedia.org/wiki/Air_France_Flight_447">Air France Flight 447 flight from Rio de Janeiro, Brazil to Paris, France, June 1 2009</a>  
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/Airspeed_p1230157.jpg/375px-Airspeed_p1230157.jpg">
<p>
Pitot Tube
<p>
  
# Blockchain Usecases
[Blockchain usecases from IBM](https://www.ibm.com/blockchain/use-cases/)

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

<img src="https://www.hyperledger.org/wp-content/uploads/2016/09/logo_hl_new.png">

# Hyperledger : http://hyperledger.org/

Hyperledger, an open source collaborative effort to advance cross-industry blockchain technologies, 
is hosted by The Linux Foundation®. 

Deployed in Docker images.

<img src="https://farm5.staticflickr.com/4494/37926120211_b7dddb090d_o.png" width="682" height="423" alt="Hyperledger Services">
<p>
https://medium.com/@robertgreenfieldiv/hyperledger-blockchain-for-a-web-2-0-architecture-6d3c83818eb1
<p>
<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

[Hyperledger Documentation](https://hyperledger-fabric.readthedocs.io/en/release/)

# Developing Blockchain apps in Hyperledger


# Exercises

## Exercise 1: Hyperledger Composer Marbles Network 
<img src="https://farm5.staticflickr.com/4652/39667642831_41001d8453_z.jpg" width="640" height="429" alt="Composer">

[Hyperledger Composer Tutorial](https://hyperledger.github.io/composer/tutorials/tutorials.html)
<p>
<a href="https://hyperledger.github.io/composer/introduction/introduction.html">Hyperledger Composer Documentation</a>
<p>
<a href="https://hyperledger.github.io/composer/reference/commands.html">Hyperledger Composer Command Line</a>
<p>
  
## Excercise 2 Create the full marbles app
<img src="https://farm5.staticflickr.com/4665/27889047409_53ae2f45fd_z.jpg" width="640" height="371" alt="bigmarbles">

https://github.com/IBM-Blockchain/marbles

## Exercise 3 [IBM Blockchain Platform](https://www.ibm.com/cloud/blockchain-platform)<p>
An enterprise-ready blockchain platform designed to accelerate the development, governance and operation of a multi-institution business network<p>

### Exercise 3.1 Setting up a Blockchain app in the IBM Container Service ready for IBM Blockchain
[Develop in a cloud sandbox IBM Blockchain Platform](https://ibm-blockchain.github.io/)

### Exercise 3.2 Setting up a Blockchain app in the IBM Cloud
<a href="https://console.bluemix.net/catalog/services/blockchain/">IBM Blockchain in the IBM Cloud</a><br>

<img src="http://34b70.http.dal05.cdn.softlayer.net/broker-static/v1-ga1/img1.png"><br>
<img src="http://34b70.http.dal05.cdn.softlayer.net/broker-static/v1-ga1/img2.png"><br>
<img src="http://34b70.http.dal05.cdn.softlayer.net/broker-static/v1-ga1/img3.png"><br>
<img src="http://34b70.http.dal05.cdn.softlayer.net/broker-static/v1-ga1/img4.png"><br>

## Exercise 4 Create a full application with a .bna file running on a laptop: Decentralized energy with Hyperledger Composer
<a href="https://developer.ibm.com/code/patterns/decentralized-energy-hyperledger-composer/?ca=dw-_-DeveloperJourney-_-dwtv-Blockchain-_-topic"> Decentralized energy with Hyperledger Composer </a>

<img src="https://farm5.staticflickr.com/4503/37148677233_71edc5a37b_o.png" width="1041" height="53" alt="blueband">

# Resources

## Blockchain in the IBM Cloud 
<a href="https://ibm-blockchain.github.io/">Set up the environment</a>

<a href="https://ibm-blockchain.github.io/">Hyperledger Composer on IBM Cloud</a>

## Zero to Bockchain
<a href="https://www.redbooks.ibm.com/Redbooks.nsf/RedbookAbstracts/crse0401.html">Zero to Blockchain</a>

[IBM Code: Blockchain Distributed database maintaining a continuously growing list of secured records or blocks](https://developer.ibm.com/code/technologies/blockchain/)

[Welcome to Hyperledger Fabric](https://hyperledger-fabric.readthedocs.io/en/release/)

[Blockchain on IBM Cloud](https://console.bluemix.net/catalog/services/blockchain/)

[Develop in a cloud sandbox IBM Blockchain Platform](https://ibm-blockchain.github.io/)

## Nodered and Hyperledger Composer

[Integrate your Blockchain with anything using Hyperledger Composer and NodeRed](https://medium.com/@CazChurchUk/integrate-your-blockchain-with-anything-using-hyperledger-composer-and-nodered-4226676f7e54)

