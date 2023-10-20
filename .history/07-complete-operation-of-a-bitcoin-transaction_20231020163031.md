
#
# **7. Complete Operation of a Bitcoin Transaction**





In this article you will discover the different stages of a transaction[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/), contrary to appearances, a sent transaction is not automatically added to the blockchain, before that it is stored in a waiting list called mempool.

## **The mempool: the transaction waiting list**

Mempool is short for "Memory Pool". In Bitcoin, the mempool is a kind of "waiting list" for transactions that have not yet been confirmed and included in a block of the [blockchain](https://coinacademy.fr/academie/histoire-blockchain/).

When a transaction[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)is created, it is first transmitted to all nodes in the network. These nodes verify that the[transaction](https://coinacademy.fr/academie/transaction-blockchain/)is valid (e.g. that the sender has enough bitcoins to complete the transaction) and, if so, they add it to their mempool.

![](RackMultipart20231011-1-et3x4p_html_53f63d94559feaec.jpg)

Minors of[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)then draw from their mempool to create new blocks. They generally choose[transactions](https://coinacademy.fr/academie/transaction-blockchain/)which offer the highest transaction fees, because these fees are a source of income for them.

Once a transaction has been included in a block and that block has been added to the[blockchain](https://coinacademy.fr/academie/quest-ce-que-blockchain/), the transaction is confirmed and is removed from the mempool.

It should be noted that not all nodes have the same mempool, as transactions may take some time to propagate through the network and nodes may have different policies as to which transactions they accept into their mempool. For example, some nodes may refuse to include transactions with very low transaction fees.

You can view pending transactions in a mempool in real time on the site[txstreet](https://txstreet.com/v/btc).

![](RackMultipart20231011-1-et3x4p_html_fa0258fd37ff33c4.png)

In this image we can see that more than 90,000 transactions are pending, knowing that a block[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)generally contains 2000 to 4000 transactions. As a reminder, a block is generated every 10 minutes.

The maximum size of a block[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)is 1 MB (megabyte) in the original Bitcoin protocol, although an update called SegWit (in August 2017) increased this effective limit to around 4 MB per block by changing how certain information is stored .

When the block is filled, it is necessary to wait for the next block to be able to add new transactions. But as seen above, you have to wait on average 10 minutes per block. If you are in a hurry, you will have to[obligation](https://coinacademy.fr/academie/obligation-entreprise-fonctionnement-explication/)to pay more for your transaction to motivate bitcoin miners to prioritize your transaction.

_FYI: a Bitcoin block can contain 1 to 4 MB of transactions, knowing that a Bitcoin transaction can take around 250 to 500 bytes (i.e. 0.00025 to 0.0005 MB). A Bitcoin block can contain 2000 to 4000 transactions without SegWit and 4 times more with SegWit, i.e. 8000 to 16000 transactions._

### **Cryptocurrency transactions work a bit like auctions**

In the Bitcoin system, transaction fees are paid by users to miners to prioritize the inclusion of their transactions in the next block that will be added to the blockchain, with these fees generally being higher when the network is overloaded.

Bitcoin transactions are similar to auctions because users "bid" with higher transaction fees to have their transactions prioritized by miners.

![](RackMultipart20231011-1-et3x4p_html_b23fa70285e16896.png)

## **The stages of a transaction until its finalization**

Find below the essential steps of a transaction:

1. A user issues a transaction.
2. The transaction is broadcast to all computers participating in the Bitcoin network: these computers are called nodes. All transactions are published to the mempool.
3. Miners verify the transaction against certain validation rules set by the creators of the specific blockchain network.
4. Validated transactions are stored in a block and are sealed with a key called a hash.
5. This new block is added to the Bitcoin blockchain and becomes part of the blockchain when other computers on the network check whether the block key is correct.
6. The transaction is complete and can no longer be modified in any way.

## **Confirmation of transactions in Bitcoin**

In the Bitcoin network, a confirmation means that a transaction has been verified by the network and added to the blockchain.

Here's how it works:

1. First Confirmation: When a transaction is first issued, it is pending and has not yet been confirmed. When a miner solves the cryptographic puzzle necessary to add a new block to the blockchain (a process called "mining"), they add a set of pending transactions to that block. The transaction is then considered "confirmed". This is the first confirmation.
2. Additional Confirmations: Each time a new block is added to the blockchain after the block containing your transaction, it counts as an additional confirmation for your transaction. This essentially means that the transaction is increasingly ingrained in the blockchain, as changing or deleting a transaction would require re-mining all subsequent blocks.

The more confirmations there are, the more secure the transaction is considered against a possible double-spend attack, where someone attempts to spend the same bitcoins more than once.

Generally, a transaction is considered sufficiently secure after 6 confirmations, which takes on average about an hour (considering that Bitcoin blocks are mined approximately every 10 minutes).

Centralized platforms for buying bitcoins like Binance have a lower tolerance threshold (2-3 confirmations or around 20-30 minutes) in order to allow their users to receive their bitcoins more quickly but tolerate a lower number of confirmations n It's not without risk.

## **What is the risk in accepting a bitcoin transaction with a single confirmation?**

When you accept a Bitcoin transaction with a single confirmation, there is a small risk that it could be reversed in a so-called "double spend" attack. A double spending attack occurs when a bad actor manages to spend the same bitcoins more than once.

This can happen in the following way: the bad actor sends a transaction with bitcoins to a person or company, then immediately creates another transaction sending the same bitcoins to a public address they control. These two transactions cannot coexist in the blockchain, so miners must choose one of the transactions to include in the next block.

If the bad actor controls a significant amount of mining power on the Bitcoin network, they could potentially mine a block containing their second transaction and add it to the blockchain before other honest miners have a chance to add a block containing the first transaction. If this happens, the first transaction would be rolled back.

However, a double spending attack is very difficult to achieve in practice. It requires a huge amount of computing power and is therefore very expensive. Additionally, after each new confirmation, it becomes more and more difficult to cancel a transaction.

If you would like to learn more about the double spend attack, feel free to[consult our dedicated article](https://coinacademy.fr/academie/attaque-double-depense/)on this subject.

## **View transaction fees on Bitcoin in real time**

![](RackMultipart20231011-1-et3x4p_html_fa66bda38d580a66.png)

On the site[mempool.space](https://mempool.space/fr/)you can view in real time the estimated price of a transaction necessary for your transaction to be prioritized.

Sat/vb is a unit of measurement used to determine transaction fees in the Bitcoin network. "Sat" is short for "satoshi," the smallest unit of bitcoin, named in honor of[Satoshi Nakamoto](https://coinacademy.fr/satoshi-nakamoto/), the creator of Bitcoin. One bitcoin is made up of 100 million satoshis.

"vB" is short for "vByte". It is a measure of the size of a transaction introduced with Bitcoin's SegWit update. Before SegWit, transaction size was measured in bytes. However, SegWit changed the way certain data is counted, leading to the introduction of the "vbyte" measurement.

Therefore, "sat/vB" represents the number of satoshis you are willing to pay in transaction fees. The higher this number, the faster your transaction is likely to be processed, as miners tend to prioritize transactions with higher fees.

#
# **What you must remember**

[Free Bitcoin Training – 2023 Edition](https://coinacademy.fr/formations/bitcoin-ca/)[6. Complete Operation of a Bitcoin Transaction](https://coinacademy.fr/cours/fonctionnement-complet-dune-transaction-bitcoin/)[What you must remember](https://coinacademy.fr/chapitres/btc-ce-quil-faut-retenir-6/)

**IN PROGRESS**

- A mempool is a kind of waiting list for transactions that have not yet been confirmed and included in a block of the[blockchain](https://coinacademy.fr/academie/histoire-blockchain/).
- The mempool is not always perfectly identical across all full nodes. There are several reasons for this, nodes can have different configuration parameters and synchronization problems with the network depending on their location or their internet connection.
- Cryptocurrency transactions work a bit like auctions: transactions with the most fees are generally processed first.
- A transaction is considered confirmed when it has been added to a block by an honest miner who has solved a "cryptographic puzzle".
- As soon as a new block is submitted to the network, the number of confirmations increases. The more confirmations there are, the more secure a transaction is considered.
- Generally, a transaction is considered sufficiently secure after 6 confirmations (6 blocks of 10 minutes on average)
- It is not recommended to consider a transaction valid after a single confirmation because there is a risk that this transaction will be canceled.
- "sat/vB" represents the number of satoshis you are willing to pay in transaction fees
- Reminder: 1 satoshi = 0.00000001 BTC

[Next Section ->](08-bitcoin-miners-and-nodes.md)