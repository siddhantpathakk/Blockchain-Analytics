# Blockchain Analytics

This repository is for summer project, under the guidance of Dr. Sourav Sen Gupta, lecturer at School of Computer Science and Engineering, here at Nanyang Technological University, Singapore.

Team members : Siddhant Pathak, Dhruv Chopra

The project aims to understand the basics of the basics of blockchain, cryptocurrency (special emphasis on Bitcoin and Ethereum), and transaction graphs. The primary focus is to analyse Bitcoin blockchain data (transaction graphs) to find potential indicators of incidents. 

Basic Terminology:

Blockchain : Blockchain is a system of recording information in a way that makes it difficult or impossible to change, hack, or cheat the system. A blockchain is essentially a digital ledger of transactions that is duplicated and distributed across the entire network of computer systems on the blockchain. Each block in the chain contains a number of transactions, and every time a new transaction occurs on the blockchain, a record of that transaction is added to every participant’s ledger. 

Cryptocurrency : A cryptocurrency is a digital or virtual currency that is secured by cryptography. A defining feature of cryptocurrencies is that they are generally not issued by any central authority, rendering them theoretically immune to government interference or manipulation.

Bitcoin : Bitcoin is a decentralized digital currency created in January 2009. It follows the ideas set out in a white paper by the mysterious and pseudonymous Satoshi Nakamoto. The identity of the person or persons who created the technology is still a mystery. Bitcoin mining is the process by which Bitcoin is released into circulation. Generally, mining requires solving computationally difficult puzzles to discover a new block, which is added to the blockchain.

Ethereum : Ethereum is a blockchain platform with its own cryptocurrency, called Ether (ETH) or Ethereum, and its own programming language, called Solidity. As a blockchain network, Ethereum is a decentralized public ledger for verifying and recording transactions. The network's users can create, publish, monetize, and use applications on the platform, and use its Ether cryptocurrency as payment. As a cryptocurrency, Ethereum is second in market value only to Bitcoin, as of May 2021. 

Transaction Graphs : A transaction graph is a directed acyclic graph G = (V ,E). The vertices V can be partitioned into states S and witnesses W , that is, V = S ∪ W . At a high level the edges E represent transitions between states.

We initially analysed some research paper publications with respect to our problem. They are listed in the reference section of this document.

File Directory:

Notebook 1.ipynb is a Jupyter Notebook file for understanding as to how one can make use of various APIs to extract data from blockchain.info about blocks and metadata such as number of transactions, block height, transaction indices etc.
