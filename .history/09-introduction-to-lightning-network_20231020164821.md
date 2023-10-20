
#
# **9. Introduction to Lightning Network**



We will now focus on the Lightning Network. You must know that [Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)was designed to promote decentralization, censorship resistance and security at the expense of scalability.

Scalability refers to the capacity of a [crypto]()currency as a whole (blockchain network) to handle an increase in transaction volume while maintaining efficient performance. In the context of blockchain[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/), for example, each block is limited to approximately 1 MB of data, which, given the frequency of 10 minutes per block, limits the number of transactions the network can process per second.

When the network is overloaded with transactions, processing times can increase and transaction fees[transaction](https://coinacademy.fr/academie/transaction-blockchain/)may become higher as users offer to pay higher fees to have their transactions processed as a priority.

Scalability is a major challenge for[cryptocurrencies](https://coinacademy.fr/academie/cryptomonnaie-crypto-monnaie/), because it is necessary to find a balance between the capacity to process a large number of transactions, the security of the network and its decentralization. THE[Lightning Network](https://lightning.network/)is an attempt to resolve the scalability problem by proposing a network on top of Bitcoin (Layer 2).

![](RackMultipart20231011-1-et3x4p_html_b6ee956daa313e14.jpg)Visual representation of Lightning Network –[Source Blockgeeks](https://blockgeeks.com/guides/lightning-network/)

## **What is Lightning Network and how does it work?**

The Lightning Network is a "second layer" or Layer 2 solution designed to accelerate transactions on[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/). It was developed to solve the scalability problems of[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)enabling fast, low-cost transactions.

The transactional capacity of[Lightning Network](https://coinacademy.fr/dossier/a-quoi-sert-le-lightning-network-de-bitcoin/)is theoretically very high and could potentially handle millions of transactions per second. This is due to the nature of its architecture, which allows transactions outside of the bictoin blockchain (offchain).

Here's how it works:

Opening the Lightning Payment Channel: Two people (or 2 businesses) who want to conduct many transactions with each other can open a payment channel on the Lightning Network. They create a first so-called "channel opening" transaction on the Bitcoin blockchain which locks a certain quantity of Bitcoin in the channel. Once the channel is open, they can carry out an unlimited number of transactions between them outside the blockchain (offchain), that is to say without recording each transaction individually on the Bitcoin blockchain.

-

Transactions in the payment channel (offchain): each transaction made in the channel updates the distribution of bitcoins locked in the channel, but these transactions are only known to the two parties involved. This allows for near-instantaneous (less than a second) and low-cost (less than a penny of a dollar) transactions because they do not require validation of the entire Bitcoin network.

-

Closing the Lightning payment channel: When the two people (or 2 companies) have completed their transactions, they close the channel by creating a so-called "channel closure" transaction on the Bitcoin blockchain which reflects the final distribution of bitcoins. This is the only other transaction that must be recorded on the blockchain, no matter how many transactions were made in the Lightning channel.

There are therefore only 2 transactions on the Bitcoin blockchain, an opening transaction and a channel closing transaction, all other transactions take place outside the Bitcoin blockchain (offchain).

![](RackMultipart20231011-1-et3x4p_html_7082f51be575be90.png)Lightning Network Stats –[Source mempool.space/lightning](https://mempool.space/lightning)

### **Lightning Channel Network**

The Lightning Network also allows channels to be connected together, forming a network. If Alice has an open channel with Bob, and Bob has an open channel with Charlie, then Alice can pay Charlie using her pooled channel with Bob, without having to open a direct channel with Charlie. This creates a network of payment channels that enables fast, low-cost transactions between any participants in the network.

-

The Lightning Network is an important innovation because it allows Bitcoin to process a greater volume of transactions, faster and at a lower cost, which is essential for Bitcoin to be used for everyday payments.

These off-chain transactions are limited only by the capacity of individual payment channels and the speed of communication between the parties.

## **Lightning Network transaction example for better understanding**

Imagine you have a big box of Lego with a friend. To make sure that no one cheats or takes more Lego than they should, you decide to create a notebook where you note how many Lego each person has, this notebook is the blockchain.

Now, you decide to play a game with your friend where you exchange lots of Lego, for hours or even several days, you know in advance that you are going to make a lot of "transactions". Instead of writing down each exchange in the notebook, which would take a lot of time, you decide to create a "channel" between the two of you. In this channel you can trade as many Legos as you want, as often as you want, without having to write in the notebook every time.

When you're done playing, you count how many Legos each person has and write the final total in the notebook. It's as if you wrote down each exchange, but in reality you only wrote down the end result. It's much faster and easier.

The Lightning Network works the same way. Instead of writing each Bitcoin transaction to the blockchain (the notebook), users open a "channel" between them and only write the final balance to the blockchain once they have completed their transactions, this end result c 'is what the "close channel transaction" will write.

![](RackMultipart20231011-1-et3x4p_html_8f794e4b283b9101.jpg)Example offchain transaction –[Source Arcane Research](https://k33.com/research/archive/articles/how-does-the-lightning-network-function)

## **What are the flaws of Lightning Network and why is it not used more?**

In practice, the transactional capacity of the Lightning Network is currently limited, each payment channel has a limited capacity, which is determined by the amount of Bitcoin that was "locked" in the channel when it was opened.

A transaction on the Lightning channel cannot be larger than the remaining channel capacity. for example, if the opening transaction of a channel contains 10 bitcoins, then it is impossible to make a transaction of more than 10 bitcoins between the different users on the channel.

There are several reasons why the Lightning Network is not more widely adopted, despite its advantages in speed and low transaction costs. Here are some of these reasons:

- Technical complexity: The Lightning Network is a relatively new and complex technology. To use it effectively, users and developers need to understand how it works, which can be intimidating for some. Additionally, setting up and managing a Lightning Network node may require technical skills that not all Bitcoin users possess.
- Lack of user adoption: For the Lightning Network to be widely used, it must be integrated into Bitcoin wallets, exchanges, and other services. Although many services are starting to integrate with the Lightning Network, the process takes time. Additionally, for the Lightning Network to be widely used, Bitcoin users must be willing to adopt it. This requires education about the pros and cons of the Lightning Network, as well as confidence in its security and reliability.
- Liquidity and Routing Issues: The Lightning Network relies on keeping payment channels open and adequately funded. If the channels are not properly funded, or the network is not properly meshed, it can be difficult to find a path to get a payment from one user to another. This can make the network less reliable for certain transactions.

These issues are being actively addressed by Lightning Network developers and adoption of the network is growing. However, it is likely that it will still be some time before the Lightning Network becomes a standard method for conducting Bitcoin transactions.

![](RackMultipart20231011-1-et3x4p_html_65b786dfa0e1c9e6.png)Total value locked in Lightning Network (May 2023) –[Source Defillama](https://defillama.com/protocol/lightning-network)

## **Some use cases for Lightning Network**

The Lightning Network was designed to enable faster and cheaper Bitcoin transactions, which opens up a number of potential use cases. Here are a few :

1. Online Payment and Instant Commerce: For online merchants, accepting payments through the Lightning Network can help reduce transaction fees and speed up the payment process. Transactions on the Lightning Network are almost instantaneous, which can be useful for merchants who need to confirm payments quickly. The Lightning Network is perfect for purchasing digital products, like apps, games, e-books, and more.
2. Tipping online, in restaurants, bars or taxis: The Lightning Network can be used to tip especially for small amounts of money where traditional transaction fees would make tipping unprofitable. You like a creator's content on YouTube or Twitch and want to pay them quickly, Lightning Network is the ideal solution for this.
3. Micropayments: Due to low or no transaction fees on the Lightning Network, it is possible to make micropayments, which is generally not economical on the main Bitcoin blockchain due to higher transaction fees. This could make it possible to pay quickly to unlock access to online content such as newspapers, mobile applications or games.[video](https://coinacademy.fr/tag/videos-podcasts/)For example.
4. Payment streaming services: The Lightning Network could be used to create payment streaming services, where users pay for every second (or other small unit of time) of a service they use like listening to music or audio podcasts.

These use cases are just a few examples of the many possibilities offered by the Lightning Network. As the technology continues to develop and mature, it is likely that new use cases will emerge.

## **Understanding Transaction Routing on Lightning Network**

Routing transactions on the Lightning Network can be a little complex, but we'll try to simplify it.

Imagine the Lightning Network as a city with many buildings (the network nodes) and roads (the payment channels) connecting them. If you want to send money to a friend who is in another building, you can't just throw the money out the window and hope it reaches their building. You have to use the roads to get there.

Every road has a cost to use it and that cost is determined in advance by the person who owns the road. The more the road is used (the more traffic it has), the higher the cost can be. This cost is what we call "network fees".

Now, let's say you want to send 10 bitcoin to your friend and you don't want to spend more than 1 bitcoin for sending. So you're looking for the cheapest way to reach your friend's building. The Lightning Network uses an algorithm to find the cheapest path, taking into account the costs of each route.

Once the path is found, the transaction is completed. Each node (building) on ​​the path takes a small portion of the network fee as payment for using its route. This is how fees are paid on the Lightning Network.

Fees on Lightning are much lower than on the Bitcoin blockchain because there are more routes available and the competition between them helps keep fees low.

![](RackMultipart20231011-1-et3x4p_html_32184bf805417.png)Transaction Routing Example –[Source report Diamond hands](https://docsend.com/view/x2yscafayexddzps)

## **How to install and use a Lightning Network wallet**

There are still many wallets on PCs and smartphones allowing you to interact with the Lightning Network. For this tutorial we will use the[Phoenix Wallet](https://phoenix.acinq.co/)which is a simple smartphone wallet, non-custodial, so you have total control of your funds.

In order to be able to receive satoshi or bitcoins on your[Phoenix Wallet](https://phoenix.acinq.co/)you need to find a way to send and receive payments on the Lightning Network, because yes, the Lightning Network is not the same as the original Bitcoin network, so you should not send your bitcoins from your Blockstream Green wallet, Exodus or from an exchange that does not manage Lightning Network like Binance because Binance does not (yet) manage the Lightning Network,[but it should happen soon](https://twitter.com/binance/status/1655419624962527233).

You can find on this[Github](https://github.com/theDavidCoen/LightningExchanges)a complete list of centralized exchanges that manage the Lightning Network.

![](RackMultipart20231011-1-et3x4p_html_e0ef132e6ad131f0.png)

## **Install Phoenix Wallet on your smartphone to use Lightning**

Go to the[official site](https://phoenix.acinq.co/)from Phoenix Wallet or directly on the[Apple Store](https://apps.apple.com/us/app/phoenix-wallet/id1544097028)where the[Google Play Store](https://play.google.com/store/apps/details?id=fr.acinq.phoenix.mainnet)In order to download the Phoenix Wallet, install it, launch it then read the information displayed on the screen and click continue.

Once the wallet is in place, click on the receive button, it will display a QR Code that you can scan with another application or your computer webcam to save time and not have to copy paste the receiving address. Alternatively, you can click on the "copy" button to copy your (very) long Lightning Network address, you are now ready to receive[satoshi](https://coinacademy.fr/satoshi-nakamoto/)(sats) on your wallet!

## **OPTION 1: Send bitcoins (BTC) and receive BTC LN via Phoenix Wallet**

This option is ideal for paying low conversion fees between Bitcoin (BTC) and[BTC](https://coinacademy.fr/bitcoin-btc/)converted for the Lightning Network (BTC LN).

Please note that it is also possible to directly deposit funds in Bitcoin ([BTC](https://coinacademy.fr/bitcoin-btc/)) on Phoenix Wallet in order to receive Bitcoin (Lightning), the company Aquin which is responsible for developing the Phoenix Wallet will ensure the conversion of your native BTC into BTC LN (Bitcoin Lightning) for you by applying a slight commission of 1%, this solution. Please note, the Phoenix Wallet is NOT a wallet designed to store native BTC.

If you wish to receive bitcoins (BTC) to convert them, go to the Phoenix Wallet application, click on "Receive" then "Show a Bitcoin address" finally, copy this address and use it from a centralized exchange or a wallet in order to to be able to send bitcoins to your Phoenix Wallet.

Do you want to send funds from a wallet or exchange to another wallet but are you afraid of doing something stupid?[Do not hesitate to consult our dedicated article on the subject.](https://coinacademy.fr/academie/transferer-ses-crypto-dun-exchange-a-un-wallet-coinbase-binance-ledger/)



![](RackMultipart20231011-1-et3x4p_html_e46445a408f2f838.png)

![](RackMultipart20231011-1-et3x4p_html_60034f0998f3b523.png)

![](RackMultipart20231011-1-et3x4p_html_4fcb66a939a4c833.png)

You must send at least 10,000 satoshi or 0.00010000 BTC for your transfer to be taken into account by Phoenix Wallet, otherwise your transaction will not arrive at its destination and your funds will be lost.

The transaction can take several tens of minutes depending on the transaction fees applied by the exchange and the slowness of the Bitcoin network. You will have to be patient... Your Phoenix Wallet will notify you when the transaction has been added to the blockchain with a "+13000 sat incoming" notification to tell you that they will soon be added to your solid.

![](RackMultipart20231011-1-et3x4p_html_c23ab3bc130057f6.png)

![](RackMultipart20231011-1-et3x4p_html_752079e986cc6539.png)

![](RackMultipart20231011-1-et3x4p_html_f362661be0203de0.png)

Once the transaction is completed and added to the blockchain, you will receive your funds in your Phoenix Wallet.

Well done, you are now in the Lightning Network. You can save your recovery key on paper or on a solution like Bitwarden, the same way for your Blockstream Green or Exodus wallet.

![](RackMultipart20231011-1-et3x4p_html_a4e7d93dcff7d1dd.png)

![](RackMultipart20231011-1-et3x4p_html_8f69c821d37b4528.png)

![](RackMultipart20231011-1-et3x4p_html_4134178879998aa0.png)

## **OPTION 2: FixedFloat, transform your bitcoins (BTC) into bitcoins on the Lightning network (BTC LN)**

As an example for this tutorial, we will send bitcoins from the centralized exchange Coinbase to a bitcoin to Lightning Network converter named[FixedFloat](https://fixedfloat.com/fr/), this is not the ideal solution because[FixedFloat](https://fixedfloat.com/fr/)takes a lot of transaction costs but it works and will mainly serve as an example to understand.

_If you want to test a FixedFloat competitor, you can also try_[_Boltz Exchange_](https://boltz.exchange/)_._

We advise you to use a centralized exchange like[Kraken](https://coinacademy.fr/exchange/kraken/)to withdraw your funds directly to your Phoenix Wallet via the Lightning Network.

First, connect to your exchange or your wallet, in my case I will go to[Coinbase](https://coinacademy.fr/exchange/coinbase/). Select Bitcoin in your[assets](https://coinacademy.fr/academie/actif-passif-crypto/)then click send. On Coinbase you will need to click on the "Send and receive" button at the top right.

![](RackMultipart20231011-1-et3x4p_html_e5601f8ef7ea77b0.png)

Now go to[FixedFloat](https://fixedfloat.com/fr/), we will define the amount in bitcoin that we wish to send, for this example we wish to send 0.0003 BTC or approximately €7.5 (not including transaction fees) and we should receive 0.00017022 BTC LN (i.e. ~4.5€), it It is important to have at least 10000 sats or 0.00010000 BTC LN otherwise Phoenix Wallet will not receive the money.

As mentioned above this is not ideal because there are Bitcoin transaction fees, those applied by FixedFloat and those of the Lightning Network channel which add up, but the most important thing here is to understand how to do it.

Now we will have to place our Lightning address in the field "your Bitcoin address (Lightning) of FixedFloat, for my part I will click on the Webcam option in order to scan the QR Core of my phone and save time, the address will thus being deposited automatically in the field.

![](RackMultipart20231011-1-et3x4p_html_ae46dce38e39c834.png)

Once your long Lightning address has been placed in this field (do not use the wrong address otherwise you will not receive your money), click on "exchange now", the page will show you the Bitcoin address on which you will need send your funds in order to receive your Bitcoin on the Lightning network, you can copy it and deposit it on your wallet or in the address field on the centralized exchange you use.

![](RackMultipart20231011-1-et3x4p_html_e918d6eac65a5fd9.png)

In our case on Coinbase this will give this:

![](RackMultipart20231011-1-et3x4p_html_cc87ba2a5937a9d.png)

All you have to do is click on "Continue" then "Send now".

The transaction can take several tens of minutes depending on the transaction fees applied by the exchange and the slowness of the Bitcoin network. You will have to be patient... Once the transaction has been completed and added to the blockchain, you will receive your funds on your Phoenix Wallet.

![](RackMultipart20231011-1-et3x4p_html_8e1e8f83bc80d2ad.png)

![](RackMultipart20231011-1-et3x4p_html_ef823151dd30ea55.png)

![](RackMultipart20231011-1-et3x4p_html_e77c21bcfe856721.png)

Well done, you are now in the Lightning Network. You can save your recovery key on paper or on a solution like Bitwarden, the same way for your Blockstream Green or Exodus wallet.

#
# **What you must remember**

[Free Bitcoin Training – 2023 Edition](https://coinacademy.fr/formations/bitcoin-ca/)[8. Introduction to Lightning Network](https://coinacademy.fr/cours/introduction-a-lightning-network/)[What you must remember](https://coinacademy.fr/chapitres/btc-ce-quil-faut-retenir-8/)

**IN PROGRESS**

- [Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)was designed to promote decentralization, censorship resistance and security at the expense of scalability.
- Scalability refers to the capacity of a[crypto](https://coinacademy.fr/academie/cryptomonnaie-crypto-monnaie/)currency as a whole (blockchain network) to handle an increase in transaction volume while maintaining efficient performance.
- Lightning Network is a layer 2 network built on top of Bitcoin.
- Lightning Network can help reduce transaction fees and speed up payments.
- Lightning Network transaction routing is the process by which transactions are transmitted through a series of participating nodes in the Lightning Network, from payer to recipient, efficiently and securely.
- A Lightning Payment Channel Allows Payments to Be Made Outside of the Bitcoin Blockchain
- Lightning Network has not yet been widely adopted due to its technical complexity, liquidity issues and routing issues. In addition, few centralized cryptocurrency exchanges integrate Lightning Network.



[Next Section ->](10-conclusion.md)