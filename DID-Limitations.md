# DID Limitations



### **Introduction**
Since the evolution of the internet, there has been a growing need for 
entities- people, animals, things, places, organizations, concepts, ideas or anything that can be represented on the internet to be identified uniquely on the internet and thus a continuous evolution 
of identity Models from Silo Identity Model which was easy to use but largely 
limited due to the lack of persistence and reusability, then we moved to the IDP Federated Identity Model which basically has a single point of failure and lacks persistence, so in search for yet a better option, Self-Sovereign Identity(SSI) Model emerged, which proposes fixes to the challenges of the previous models.

### **What is Self-Sovereign Identity(SSI)**
Self-Sovereign Identity(SSI) is an identity model that makes it possible for an entity to establish a pairwise connection with another entity in a purely decentralized manner. The model comprises Decentralized Identifiers(DIDs) as the base layer, Decentralized Key Management Systems(DKMS), DID Authentication(DID Auth) and Verifiable Credentials(VC). We would be looking closely at DID
### **What is Decntralized Identifier (DID)**

A [Decntralized Identifier (DID)](https://www.w3.org/TR/did-core/#dfn-decentralized-identifiers)refers to a pseudo-anonymous way of identifying an entity in a cryptographically verifiable way. Technically we can say a DID is a URI because it hybrids the URL which locates resources on a network and a URN which is a persistent name for a resource on the network as stated by [Drummond Reed](https://ssimeetup.org/decentralized-identifiers-dids-fundamentals-identitybook-info-drummond-reed-markus-sabadello-webinar-46/) and this is what it looks like 

![parts of a DID](/Users/isirfitech/Projects/blockchain/Tutorials/Ceramic/DID-Li/did.png) 

There are four core properties of a DID

a DID is :-
- **A Persistent or Permanent Identifier**: It never needs to change with the course of time
- **A Resolvable Identifier**: Anyone can look it up to get its metadata
- **A cyptographically-verifiable Identifier**: The owner can prove control using cryptography
- **A decentralized Identifier**: No centralized registration authourity is needed.

### **How does a DID work?**

With a DID, a verifier would be able to resolve it into a [DID Document](https://www.w3.org/TR/did-core/#dfn-did-documents) which contains the minimum amount of information needed to bootstrap other necessary information needed to interact or connect with the [DID Subject](https://www.w3.org/TR/did-core/#did-subject) such as one or more public keys or other verification methods used for authenticating the DID Subject during an interaction, under the control of the DID Controller, one or more services endpoints that specify how to interact with the DID Subject and some optional elements like timestamps for audit history, digital signature for integrity, information related to delegation and authorization. A DID has three parts, the DID [scheme](https://www.w3.org/TR/did-core/#dfn-did-schemes) idebtifier, the identifier for the DID [method](https://www.w3.org/TR/did-core/#dfn-did-methods), and the DID method-spcific-identifier which is described by the DID method eg for Ethereum based DIDs, it could be the smart contract address of the DID, or the hash of the key as in Bitcon reference



### **What can we do with DIDs**
 DIDs can be used for a platera of things and they include

 - **Enterprise Identifiers**
 - - At the enterprise level, DIDs would ensure 1) A competative market place, 2) Low management overhead for the government 3) Self management of Identifiers and cryptographic materials. Imagine a government that wants to ensure that the supply chain that feeds electronic products into her borders is secure, so she authorizes a new way of submitting digital documentation to her Customs office, that all documentations are provided as a machine-readable digitally signed data with proof of provenance from supply chain partners whose identities are also known to a great degree of certainty. Documents that are signed with digital proofs are provided at every stage from the manufacturing, to packaging down to shipping. This document is submitted to the Customs on arrival where all the digital signatures are verified and checked to verify and ensure that the products arrived the borders of the country as they left the manufacturing facility, and have not been tempered with.

---

 - Life-Long Credential
 - - 
 - ---
 - Prescriptions
 - ---
 - Digital Executor
 - ---
 - Bob rents a car
 - ---
 - Portable Secure Communication
 - ---

### **Challenges with DIDs Use cases**
- The Customs and the downstream customers of the products as mentioned in the Enterprise Identifier above are required to use the same documentation and digital signature to verify the product, this could be problematic. Governments usually create ad-hoc solutions for their inports. This would make securing the global supply chain difficult as because each government have her own way of identifying coporations that downstream customers intergrate with and securing her supply chain. Now the challeng would be if you are a global company, it means intergrating with many different supply chain system with different capabilities. That means to secure the supply chain with the downstream customers would depend on country specific coporate identification and Public Key Infrastructure solutions which would in summary drive up cost of doing business across border for the global comapanies.

---
- 
### **What does the specifications of DID allow us to do?**

As we have established, DIDs do not exist on a single registry. DIDs are implemented using [Methods](https://www.w3.org/TR/did-core/#methods) which refers to the approach or implementation of the DID. Different DID methods have different implementations, some are implemented on a Decentralized Ledge Technology (DLT) eg [btcr](), [ethr](), [3]() or stored on a specialized site eg GitHub, or on ephemeral DIDs with lighter requirements eg the ones used on IoT devices 

### **What does the specifications of DID limit us from doing?**





<!--(https://w3c.github.io/did-core/#referring-to-verification-methods)--> 
  

  <!--
- **Adoption issue** : With an estimated population of about [8 billion people](https://www.un.org/development/desa/pd/sites/www.un.org.development.desa.pd/files/wpp2022_summary_of_results.pdf), and more than half of those using various digital products, there needs to be a large-scale buy-in to get the technology to mainstream adoption. Technology giants like Apple, Google, Microsoft, Facebook etc would need to incorporate the system into their products to get it to speedy and broad adoption.


- **Exclusion** : For mass adoption, we look at the poor nations of the world to also be able to afford to key into this technology revolution, but the gadgets required to make use of these services are relatively expensive and would not reach the grassroots just yet


- **Education** : Being a new piece of technology, blockchain is not quite yet intuitive to most of its users as such, and it is paramount for users to be able to grant/restrict permissions to what credentials they want to share per time.
-->


<!--DIDs have alot of promises for making life easer for both users and enterprises as it proposes to make processes faster, convinient and more efficient. It however comes with some limitations and that is what we are going to consider, but first first let us talk about what we casn do with DIDs.-->

<!-- To create a DID, the entity would create a SSI and generate a pair of private and public keys. The generated public key is associated with the DID and the private key is used to prove ownership of the credentials associated with the public key or the DID.-->