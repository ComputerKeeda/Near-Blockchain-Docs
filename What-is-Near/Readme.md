# What is Near

NEAR is a user-friendly and `carbon-neutral` blockchain, built from the ground up to be performant, secure, and infinitely scalable.

In technical terms, NEAR is a `layer one`, `sharded`, `proof-of-stake` blockchain built with usability in mind.

In simple terms, NEAR is blockchain for everyone.

1. **Carbon-neutral**: A carbon-neutral process or system has a net-zero carbon footprint, meaning it doesn't contribute to an increase in atmospheric CO2 levels. In the context of a blockchain, this means that the energy consumed during the operation and maintenance of the network is either offset by renewable energy sources or compensated for through carbon offset initiatives. This is important as it helps to minimize the environmental impact of the technology.

2. **Layer one**: Layer one refers to the base or foundational layer of a blockchain protocol. This is where the core blockchain infrastructure, including consensus algorithms, transaction validation, and data storage, takes place. Other layers, such as layer two solutions, can be built on top of layer one to improve scalability or add specific features. In the case of NEAR, it is a layer one blockchain, which means it provides the primary infrastructure for building decentralized applications (dApps).

3. **Sharded**: Sharding is a technique used to increase the scalability of a blockchain network by dividing the network into smaller, interconnected sub-networks, called shards. Each shard processes a portion of the overall transactions, allowing the network to handle more transactions in parallel. This helps to improve the throughput of the network and reduces the risk of congestion. NEAR employs sharding to achieve high performance and scalability.

4. **Proof of Stake (PoS)**: Proof of Stake is a consensus mechanism used by some blockchain networks to validate transactions and create new blocks. Unlike Proof of Work (PoW), which relies on computational power to solve complex mathematical problems, PoS relies on the amount of a specific cryptocurrency held by users (their "stake") to determine their ability to validate transactions and create new blocks. PoS is considered more energy-efficient and environmentally friendly compared to PoW, as it requires significantly less computational power. NEAR Protocol uses a PoS mechanism for its consensus algorithm.

# Blockchain basics

Before diving deeper into the intricacies of Web 3 development, let’s explore what it is and why it exists. First of all - what does number 3 mean? The World Wide Web, or Internet in general, has evolved through the years and can be loosely divided into the 3 “generations”:

- Web 1.0 - the first generation, roughly from 1991 to 2004. At this time, the Internet was slow, expensive, and dominated by static web pages. Most people were content consumers, with only a handful of content creators who created and hosted sites. JavaScript was at its infancy, media was rarely seen (due to speed and cost), and social media hadn't been invented yet. The Internet was highly decentralized and open to anyone. Everyone ran their own server or used one of the numerous hosting providers. Open protocols and standards were used for everything - HTTP, HTML, FTP, SMTP.

- Web 2.0 - the current generation, from around 2004 till now. A massive paradigm shift started to happen in the early 2000s. The Internet became faster and cheaper, and slowly but steadily spread into the lives of ordinary people. And as people trickled in, businesses followed. More and more services were offered through the web, like payments, shopping, and deliveries. Pages became more interactive and rich with media, but most importantly - users transitioned from just consuming content, to actively creating one. Social media boomed, smartphones were invented, and the web began its explosive growth we are still seeing to this day. At present day, the Internet touches almost every aspect of modern life, but with all of its usefulness comes a darker side. As it grew, it became more and more centralized. While this centralization brought a number of benefits, there are a number of problems as well. Digital ownership is one of them. As digital assets became ubiquitous, it became apparent that users don't really own them. Instead, ownership remained with centralized companies. Google can block access to your emails on Gmail any time it wants (one example), or a game company can shut down a game server and destroy forever a game you once bought. Another major problem is a loss of privacy. A new business model has emerged, where users “pay” for the services with their personal data. Social platforms ask us to share our personal information so they can feed us information we want to see. Once they have our attention they sell it to anyone who will buy it, effectively harming society for financial gain.

- Web 3.0 - the next generation. It’s still in its early stages, and no one knows for sure how it will evolve, but several key aspects can already be outlined:
  - Focus on decentralization and privacy. Shift digital ownership from companies to users.
  - Trustless and permissionless.
  - Driven by the community through tokenomics and governance.

# Building blocks of Web decentralization

As we already briefly discussed, the current Web is highly centralized, and mostly built using client-server architecture on centralized servers hosted on one of the clouds (AWS, Azure, GCP, etc). According to one report, 90% of mobile traffic goes to the clouds, which means a significant portion of the Internet is basically controlled by a handful of companies. This consolidation of power has a number of downsides and this article on "Why Decentralization Matters" does a good job explaining some of those problems.

The first decentralization revolution happened in file sharing, with the arrival of the (in)famous BitTorrent protocol. By being a p2p protocol, it’s truly decentralized, and allows data to be stored distributedly without any central authority (and sometimes without consent of a central authority, which caused a lot of drama, but that’s a story for another time). Ideas behind this protocol have been used in modern decentralized file storages like IPFS and FileCoin, we’ll come back to this later and explore it in more details.

The next revolution happened in the world of finance. For a long time transferring money required a central authority (banks), which would monitor, approve and execute these transfers. This has changed when the first cryptocurrency - Bitcoin - appeared. As already mentioned <u>**BitTorrent**</u> protocol, it also uses p2p communication, but instead of files it operates a transaction ledger, which is stored as a blockchain. Blockchain structure is needed to ensure that stored ledger cannot be altered, and at the same time to incentivize storage of this data. Unlike BitTorrent, Bitcoin network participants are rewarded for their services using a process called “mining”. This created a foundation for a new form of currency - digital currency (or cryptocurrency), with a unique property that it doesn’t need a central authority to function. Instead, users themselves maintain and operate it. And as with the previous decentralized system, BitTorrent, central authorities have issues with this.

Following the success of Bitcoin, other cryptocurrencies started to appear. The most important one is Ethereum, which took the concept of blockchain one step further and adapted it to store not just a transactions leger, but any kind of data, and, most importantly code (which is just another form of data). Basically, it turned out we can use it as a decentralized database transaction log. And if we have data and code living in the decentralized database, the only thing we lack to build a decentralized application is an ability to execute this code. So Ethereum did just that, and a Smart Contract was born. Now, let's dive deeper into the world of blockchains, smart contracts, and explore how we can build decentralized applications with them.


### Let's start with a brief overview of what blockchain and smart contracts are.


🌐 In classical Web 2.0 apps, you need 2 things to build the backend: a 💾 database to store data and a 🖥️ server to execute your code.

🌐 **Web 3.0 apps also need a backend, but instead of a database, we have a 🧱 blockchain, and instead of a server, we have 🤖 smart contracts.**

🧱 The blockchain is a secure and transparent way to store data, while smart contracts automate business logic and transactions without intermediaries.

🖥️ However, in Web 3.0 apps, we may still need a traditional database and server for tasks like user authentication and storing data that's not suitable for the blockchain.

🌐 So, while Web 3.0 apps rely on the blockchain and smart contracts for their backend, they may still need traditional components found in Web 2.0 apps.




Blockchain is like a 📜 scroll that contains a list of all the transactions that happened. But to make it work faster, the transactions are grouped into 🧱 blocks. Each block has a special code called a 🔑 hash that links it to the previous block in the chain.

🔑 Hashes make it impossible to change any individual transaction in the chain, because it would change the hash of that block and all the following blocks too. This means that the whole chain would be 🚫 invalid.

🧱 This makes blockchain perfect for storing data in a decentralized way, because anyone can quickly check if a transaction or the whole chain has been 🚫 tampered with.


![](https://docs.near.org/assets/images/web3-1-2074f0379a1152437f0b274f4c5b31bb.png)


In a blockchain, we create a list of all transactions 📝 that happen in the system. This list acts like a shared database 🗃️ everyone can access. Each new transaction is added to the end of the list and can't be changed 🚫.

We can think of this as a "decentralized event sourcing pattern" 🔗, where each transaction is like an event 🎉 that changes the system's state. By replaying these events in order 🔄, we can figure out the current state of the system at any point in time ⏳.