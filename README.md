# Blockchain Analytics

This repository is for summer project, under the guidance of Dr. Sourav Sen Gupta, lecturer at School of Computer Science and Engineering, here at Nanyang Technological University, Singapore.

Team members : Siddhant Pathak, Dhruv Chopra

The project aims to understand the basics of blockchain, cryptocurrency (special emphasis on Bitcoin and Ethereum), and transaction graphs. The primary focus is to analyse Bitcoin blockchain data (transaction graphs) to find potential indicators of incidents. 

We are highly grateful to the professor for providing us with the opportunity to explore this field of cryptocurrency and utilise the power of machine learning.

![image](![image](Blockchain-Analytics/Communities.png))

## Definition: 

Blockchain : Blockchain is a system of recording information in a way that makes it difficult or impossible to change, hack, or cheat the system. A blockchain is essentially a digital ledger of transactions that is duplicated and distributed across the entire network of computer systems on the blockchain. Each block in the chain contains a number of transactions, and every time a new transaction occurs on the blockchain, a record of that transaction is added to every participant’s ledger. 

Cryptocurrency : A cryptocurrency is a digital or virtual currency that is secured by cryptography. A defining feature of cryptocurrencies is that they are generally not issued by any central authority, rendering them theoretically immune to government interference or manipulation.

Bitcoin : Bitcoin is a decentralized digital currency created in January 2009. It follows the ideas set out in a white paper by the mysterious and pseudonymous Satoshi Nakamoto. The identity of the person or persons who created the technology is still a mystery. Bitcoin mining is the process by which Bitcoin is released into circulation. Generally, mining requires solving computationally difficult puzzles to discover a new block, which is added to the blockchain.

Mining Pools : A mining pool is a joint group of cryptocurrency miners who combine their computational resources over a network to strengthen the probability of finding a block or otherwise successfully mining for cryptocurrency.

Transaction Graphs : A transaction graph is a directed acyclic graph G = (V ,E). The vertices V can be partitioned into states S and witnesses W , that is, V = S ∪ W .

Centrality of a node : Node centrality is a measure of the importance of a node in a graph. There are numerous ways to define node centrality, the most well known being arguably the degree centrality, where a node is important if its degree is high. In our analysis, centrality will be of prime importance.

Harmonic Centrality : Harmonic centrality of a node u is the sum of the reciprocal of the shortest path distances from all other nodes to u.

Global Reaching Centrality : The global reaching centrality of a weighted directed graph is the average over all nodes of the difference between the local reaching centrality of the node and the greatest local reaching centrality of any node in the graph.

Load Centrality : The load centrality of a node is the fraction of all shortest paths that pass through that node.

Dispersion between two nodes in a graph: A link between two actors (u and v) has a high dispersion when their mutual ties (s and t) are not well connected with each other.

We initially analysed some research paper publications with respect to our problem. They are listed in the reference section of this document.

The distribution of mining power or hash rate can be seen as a key indicator for the market shares of mining pools and represents a core security parameter in Bitcoin. Statistics published by popular analytics platforms indicate that the overall mining power is concentrated among a relatively small number of pools, with BTC.com, ViaBTC and AntPool holding—or being close to hold—the majority, but none of them exceeding the 50% limit. 

As of now, major pools direct their mining revenue to publicly known addresses, specified in the output of a block’s coinbase transaction. We refer to this address as reward address. Furthermore, mining pools have been observed to usually reveal their identity by adding human-readable text or markers to the coinbase.

## File Directory:

Notebook_1.ipynb is a Jupyter Notebook file for understanding as to how one can make use of various APIs to extract data from blockchain.info about blocks and metadata such as number of transactions, block height, transaction indices etc. We make use of the NetworkX library from Python to visualise a small sub-section (due to computational constraints) of the graph. 

CoinGecko_API.ipynb is a Jupyter Notebook file for understanding the functionality of the reknoned CoinGecko API for collecting and curating historical as well as real-time data pertaining to cryptocurrencies, Bitcoin in our case. We later ruled this API out for discussiion due to its account restrictions.

Analysis.ipynb is a Jupyter Notebook file for analysing the data collected and curated by the previous steps. Basic cleaning and pre-processing is performed upon it to make better inferences from it. We made use of NetworkX library to create and store the graph. We also utilised various algorithms such as the VoteRank Algorithm. The centrality of all nodes has been computed too. The various types of centrality taken into consideration are : closeness_centrality, in_degree_centrality, out_degree_centrality, harmonic_centrality, global_reaching_centrality, load_centrality. Dispersion among all the nodes has also been computed where the output is a dictionary of nodes with dispersion for all "target" nodes.

Graph.csv is a Comma Seperated Value file consisting of the various Bitcoin addresses as nodes and the amount of cryptocurrency in the transaction between them as the edge weight.

Mining_Pool.ipynb is a Jupyter Notebook file for understading the basic concepts of mining pools. We expand our research into mining pools and various levels to understand payout patterns to various reward addresses. 

## Room for improvement:
Address clustering refers to construct the one-to-many mapping from entities to addresses in the Bitcoin system. Various heuristics (pre-determined as well as newly developed ones) can be utilised for the same purpose to classify various addresses and more easily understand transactions and flow of cryptocurrency. 
