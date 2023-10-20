
#
# **8. Bitcoin miners and nodes**





In this part we will talk about the different types of nodes on [Bitcoin](###), miners and we will learn the basics of Bitcoin mining in order to quickly identify if Bitcoin mining is a profitable business for the most curious among you.

## **The different types of Bitcoin nodes**

There are several types of nodes in the Bitcoin network, each with a specific function. Here is a description of some of them:

1. Full Nodes: These are the most important nodes in the network [Bitcoin](###). They keep a complete copy of the [blockchain](###), verify all transactions and blocks, and respect network rules. Full nodes serve as a reference to verify transactions and blocks that are transmitted in the network.
2. Mining Nodes or miners: These nodes use computing power to solve mathematical problems to create new blocks in the [blockchain](###). Once a mining node resolves the issue, it broadcasts the new block to all other nodes in the network.
3. Lightweight Nodes (SPV Nodes): These nodes do not maintain a complete copy of the blockchain. They only download block headers from the blockchain, which requires fewer resources in terms of storage and (internet) bandwidth. Light nodes must trust full nodes to obtain correct information about the state of the blockchain.

![](RackMultipart20231011-1-et3x4p_html_7472a28e29da5d7f.png)

## **What "mathematical problem" does the Bitcoin miner solve exactly?**

The "mathematical problem" that miners[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)solve is actually a Proof-of-Work task. This task is basically a cryptographic hashing operation that is deliberately designed to be time-consuming and difficult to solve, but easy to verify once a solution is found.

Here is how the process works for an individual minor:

1. The miner gathers a set of pending transactions and organizes them into what is called a candidate block.
2. It takes the block header, which includes information like the hash of the previous block, timestamp and a nonce (random number) and applies the SHA-256 hash function (in the case of[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)) to this data.
3. The hash function produces an output (called a hash), which is a string of numbers and letters. For the block to be accepted by the network, this hash must be less than a certain target value of[difficulty](https://coinacademy.fr/academie/difficulte-minage-mining-bitcoin-hash/)defined by the Bitcoin protocol. This target is adjusted every 2016 blocks (approximately two weeks) so that the average block generation time remains around 10 minutes.
4. The miner changes the nonce of the block header and repeats the hashing process until it finds a hash that is less than the target value. This is what we call the "mathematical problem" to solve. In reality, it's more of a brute force competition in which the miner generates billions of hashes per second until they find a solution.
5. When the miner finds a solution, it broadcasts the block to all other nodes in the network. Other nodes easily verify the solution by performing the hash function once with the same data. If the block is valid, they add it to their copy of the blockchain.
6. The miner who solved the problem receives a reward in the form of newly created bitcoins (the so-called block reward) as well as the fees for[transaction](https://coinacademy.fr/academie/transaction-blockchain/)included in the block.

It is thanks to this proof of work process that[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)manages to maintain the security and integrity of its decentralized network. Each miner contributes to this process by participating in the competition to find the next valid block.

![](RackMultipart20231011-1-et3x4p_html_eae022206508125e.jpg)

## **Quick history of the evolution of hardware for mining Bitcoin**

The evolution of mining equipment[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)has followed a rapid and exciting trajectory, characterized by innovation and constant improvement in efficiency. Here is an overview of this development:

1. Processors (CPU): Originally, mining[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)was carried out on personal computers using processors (CPU). This is how the creator of Bitcoin, Satoshi[Nakamoto](https://coinacademy.fr/satoshi-nakamoto/), mined the first blocks of Bitcoin.
2. Graphics Cards (GPU): Miners quickly discovered that graphics cards were much more efficient for Bitcoin mining than CPUs. GPUs are designed to perform parallel calculations for graphics rendering, which happens to be very useful for Bitcoin mining.
3. Programmable Front Gate Circuits (FPGAs): FPGAs were later adapted for Bitcoin mining. These devices can be programmed to perform specific tasks, including calculating Bitcoin's hashing algorithm. They were more energy efficient than GPUs, which helped reduce mining costs.
4. Application-Specific Integrated Circuits (ASICs): ASICs are the pinnacle of efficiency in Bitcoin mining. They are designed to perform a single task – in this case, the SHA-256 hashing algorithm used by Bitcoin – and they do it extremely well. ASICs are much more powerful and energy efficient than FPGAs, but they are also more expensive to produce.

![](RackMultipart20231011-1-et3x4p_html_9ca0461d9f35c9ad.jpg)

Today, the majority of Bitcoin mining is done with ASICs, and competition is so fierce that individual miners often struggle to compete with large mining "farms," which can afford to purchase thousands of ASIC.

Additionally, new generations of ASICs are constantly being developed, providing better energy efficiency and greater computing power. This means that miners must constantly upgrade their hardware to stay competitive.

Importantly, the growing use of ASIC has also led to controversy, with some arguing that it goes against the decentralized spirit of Bitcoin, as it promotes a concentration of mining power in hands. of a small number of players capable of obtaining this expensive equipment.

## **What is a mining pool**

A mining pool is a group of miners who combine their computing power to increase their chance of solving a block and earning mining rewards.

Bitcoin mining, and many others[cryptocurrencies](https://coinacademy.fr/academie/cryptomonnaie-crypto-monnaie/), is a very computationally and concurrency intensive operation. Each miner or group of miners tries to solve a "math problem" to add the next block to the blockchain. The first to solve the problem wins the block reward, currently 6.25 bitcoins and the transaction fees contained in the block.

Since the difficulty of these problems is so high, it is very difficult for an individual miner to be the first to find the solution. Therefore, miners began to group together into mining pools, where they combine their computing power and share the rewards every time a pool member solves a block.

Rewards are typically shared in proportion to the computing power each member contributed, meaning each miner receives a share of the mined bitcoins that corresponds to their contribution to the pool's overall power.

Mining pools allow individual miners to receive more regular and predictable, although generally smaller, payouts rather than relying on luck to obtain a large block reward.

![](RackMultipart20231011-1-et3x4p_html_8002adf40fcf0c7d.png)Bitcoin Mining Pools –[Source HashrateIndex](https://hashrateindex.com/hashrate/pools)

There are many different mining pools, each with their own rules, fees, and payment methods. Some of the largest and most well-known include Foundry USA, F2Pool, and Antpool.

## **How to calculate the profitability of Bitcoin mining**

Calculating the profitability of Bitcoin mining depends on several factors, including:

The cost of electricity: Bitcoin mining consumes a lot of electricity. The cost of this electricity can vary considerably depending on your location (country) and the type of contract you have negotiated with your electricity supplier. You'll need to know how much you're paying per kilowatt-hour (kWh) to be able to calculate your energy costs.

Since Russia's invasion of Ukraine in February 2022, the price of electricity in Europe for individuals and professionals has exploded. The price of the kWh EDF (Électrcité de France) is currently ~0.21€ for individuals and professionals, you can find much cheaper electricity in other countries in Africa and Asia ([source](https://fr.globalpetrolprices.com/electricity_prices/)). It is therefore not advisable to mine seriously in Europe.

![](RackMultipart20231011-1-et3x4p_html_e7bb9d2b9162dedf.png)

_Be careful, it may be tempting to want to get into bitcoin mining in certain African or Asian countries but there is always the risk of your equipment being seized by the state or burglarized._

The power of your mining hardware (hash rate): The more powerful your mining hardware is, the more Bitcoins you will be able to mine. This mining power is generally measured in terahashes per second (TH/s).

The power consumption of your mining hardware: Besides mining power, you also need to take into account how much electricity your hardware consumes. This is usually measured in watts.

The cost of mining hardware: ASIC mining machines can cost several thousand dollars. It is important to take into account the initial cost of your hardware when calculating profitability.

![](RackMultipart20231011-1-et3x4p_html_8183286390ec4524.png)

_In this image we can see ASIC miners sold by the company Bitmain. Each machine has a price, a computing power measured in terahashes per second (T) and a displayed energy consumption. We will see below how to simulate the profitability of Bitcoin mining._

Bitcoin mining difficulty: Mining difficulty is a measure of the difficulty of finding a hash lower than the given target when creating a new block. It is adjusted approximately every two weeks to ensure that a new block is mined every 10 minutes on average. The higher the mining difficulty, the less likely you are to mine a block.

The Bitcoin Block Reward: Currently, the block reward is 6.25 bitcoins. However, this reward is halved every four years during events called "halvings". The next[halving](https://coinacademy.fr/academie/bitcoin-prochain-halving-compte-a-rebours/)is scheduled for April 2024.

The price of Bitcoin: The price of Bitcoin constantly fluctuates. If the price of Bitcoin increases, your mining revenue is worth more in terms of dollars or euros. However, if the price drops, your mining revenue may not cover your costs.

There are many Bitcoin mining profitability calculators online where you can enter these factors and get an estimate of your potential profits or losses. It is important to note that Bitcoin mining is very competitive, and there is no guarantee of profitability.

### **Simulate the profitability of Bitcoin mining with CryptoCompare**

[Cryptocompare](https://www.cryptocompare.com/mining/calculator/btc?HashingPower=90&HashingUnit=TH%2Fs&PowerConsumption=3100&CostPerkWh=0.20&MiningPoolFee=1)is an online tool allowing you to easily simulate the profitability of Bitcoin mining at time T. The simulation takes into account the price of Bitcoin at time T as well as the block reward and the difficulty of mining bitcoins at time Don't understand that, if the price of Bitcoin changes and if the difficulty of mining increases, the future result will not be the same but it is a good basis to get an idea.

Let's imagine we want to mine bitcoins with an ASIC."[Bitmain Bitcoin Miner S19](https://shop.bitmain.com/product/detail?pid=000202305061049401097z99C0ug0660)". We know that this hardware consumes around 3105 Watt per hour and offers computing power (Hash Power) of around 90 terahashes per second (TH/s).

![](RackMultipart20231011-1-et3x4p_html_f567ad15e78793f9.png)

We can now report all this data on the Cryptocompare simulator[.com](https://www.cryptocompare.com/mining/calculator/btc?HashingPower=90&HashingUnit=TH%2Fs&PowerConsumption=3105&CostPerkWh=0.20&MiningPoolFee=1)by adding the price of our electricity per kWh ($), we can leave the commission percentage of 1% for the mining pool because it is a commission that we will have to pay in all cases if we connect to a pool . As seen earlier, it is almost impossible to successfully mine bitcoin on your own due to lack of power. Typically, Bitcoin mining pools take 1% commission.

![](RackMultipart20231011-1-et3x4p_html_79edd14993ec68d8.png)

In this simulation, we see that bitcoin mining makes us lose money every month because electricity is far too expensive. Let's try with cheap electricity of around $0.03 per Kilowatt-hour (kWh) instead of $0.20 now:

![](RackMultipart20231011-1-et3x4p_html_2430659f2b44e74e.png)

This time we are profitable by over $1500 per year at current prices, not bad knowing that ASIC "[Bitmain Bitcoin Miner S19](https://shop.bitmain.com/product/detail?pid=000202305061049401097z99C0ug0660)" costs about $1,000 each. You will have understood, the price of electricity is the crux of the matter and we must add to that the fact that the machines (ASICs) make a lot of noise, the price of Bitcoin can go down and the difficulty in the increase (which will therefore reduce profitability).

Cheap electricity is not always easy to obtain, do not launch headlong into a Bitcoin mining project without consulting with real professionals in the sector because it requires a lot of organization to install the equipment and protect it against theft and/or seizures!

## **How to mine Bitcoin?**

We will not explain in this article how to mine Bitcoin because the manipulation is simply not profitable on a personal computer or on a smartphone.

Today Bitcoin mining must be done with specialized equipment, if you absolutely want to try the adventure of mining cryptocurrencies to accumulate bitcoins with your personal computer, do not mine Bitcoin, redirect yourself to alternative cryptocurrencies more profitable to mine and resell these cryptocurrencies to accumulate Bitcoin.

Mining is a very attractive market at first glance but it is becoming more and more complex to make your investment profitable by taking into consideration the price of equipment, the price of electricity, the increasing difficulty of mining blocks but also the time spent to set up the machine.

Many people have embarked on an adventure to mine Ethereum, another cryptocurrency, without taking into account the price of electricity and the constant increase in difficulty.

#
# **What you must remember**

[Free Bitcoin Training – 2023 Edition](https://coinacademy.fr/formations/bitcoin-ca/)[7. Bitcoin miners and nodes](https://coinacademy.fr/cours/mineurs-et-noeuds-bitcoins/)[What you must remember](https://coinacademy.fr/chapitres/btc-ce-quil-faut-retenir-7/)

**IN PROGRESS**

- There are different types of nodes: full nodes, mining nodes (Mining Nodes or miners) and light nodes.
- When a miner "mines" bitcoins he is carrying out a task that is time-consuming (which takes time) and is difficult to solve. This task requires good equipment and consumes energy, it is proof of work.
- When Bitcoin was launched, miners mined with their personal computer with their processor (CPU) then their graphics card (GPU) then, as miners became more professional, they gradually moved to hardware components dedicated to "calculation". " of hashes namely FPGAs then finally ASICs.
- Today it is difficult to be profitable and competitive in crypto mining with anything other than ASICs (application specific integrated circuits)
- A mining pool is a group of miners who combine their computing power to increase their chance of solving a block and earning mining rewards.
- The profitability of mining bitcoins and cryptocurrencies in general depends on many factors but mainly on the cost of hardware and the cost of electricity.
- It is not recommended to mine bitcoins in Europe because of the high cost of electricity compared to many countries.

[Next Section ->](09-introduction-to-lightning-network.md)