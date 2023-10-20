#
# **5. Understand the usefulness of the Bitcoin blockchain**



In this article, you will understand how blockchain technology works on Bitcoin. You will also understand why the data recorded in the blockchain is secure and almost impossible to corrupt.

Blockchain enables secure and transparent decentralization of transactions and information, reducing the need for trusted third parties.

## **What is blockchain**

Blockchain is a decentralized, secure and transparent information storage and transfer technology.

It is often compared to a public and distributed accounting ledger which records [transactions](###)and other types of data. There [blockchain](####)is made up of a series of blocks that contain data and each block is cryptographically linked to the previous one, making it extremely difficult to modify or tamper with the information once it has been added to the chain.

Here are some key features of the [blockchain](###):

1. Decentralization: There is no central authority that controls or manages the blockchain. Instead, it is maintained and updated by a network of independent nodes that follow the same rules to add new blocks to the chain.
2. Security: Transactions or data stored in the blockchain are secured through the use of [cryptography](https://coinacademy.fr/academie/cryptographie-blockchain-chiffrement-asymetrique/). The blocks are linked to each other, making it very difficult to change the information once it has been added to the chain.
3. Transparency: All transactions or data stored in the blockchain are visible to all network participants. This allows everyone to ensure data integrity and verify its authenticity. You don't have to trust, you can check for yourself.
4. Immutability: Once a block has been added to the chain, it is virtually impossible to modify or remove it. This ensures that the data stored in the blockchain is permanent and resistant to tampering.

Blockchain is the underlying technology of many cryptocurrencies, such as Bitcoin and Ethereum, but it is also used in various applications and industries to ensure data integrity and security, such as supply chain management , electronic voting systems, product traceability,[smart contracts](https://coinacademy.fr/academie/smart-contracts-fonctionnement/)and more.

![](RackMultipart20231011-1-et3x4p_html_5c5d286a764a33a4.png)

## **Blockchain is an accounting ledger**

A "ledger" is a term used in accounting to describe a set of accounting entries.

These records are used to document all of a company's financial transactions. This general ledger is usually managed by a single entity (for example, the company's accounting department) and is centralized.

Blockchain is a form of digital ledger with some key differences. Blockchain records digital transactions across many computers in a decentralized manner. Each block in the chain contains a list of transactions.

When a block is completed, it is added to the chain in a[order](https://coinacademy.fr/academie/comprendre-differents-types-ordres/)chronological. Additionally, once a block is added to the chain, the information it contains is very difficult to change due to the design of blockchain technology.

What advantages does blockchain technology bring compared to an accounting ledger?

- Centralization vs. Decentralization: A traditional ledger is usually managed by a single entity, making it centralized. In contrast, a blockchain is decentralized and is managed by several participants (or nodes).
- Transparency: Transactions on a blockchain are generally more transparent to all participants in the chain. In a traditional ledger, only those responsible for the ledger have full access to all transactions.
- Purpose of transactions: In a blockchain, once a[transaction](https://coinacademy.fr/academie/transaction-blockchain/)is added to the chain, it is considered final. In a traditional ledger, transactions can be adjusted or corrected.

If this explanation is still not clear, here is how transactions in a block are noted on the blockchain:

![](RackMultipart20231011-1-et3x4p_html_a01ea794333ac577.png)

In the blockchain[bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/), your name or your pseudonym will not be indicated, this example simply allows you to understand that several pieces of information are written in a block, namely the block number, the amount in bitcoins sent, the public address issuing the transaction, the public address of receipt of the transaction as well as the date and time of the transaction.

The site[blockchain.com](https://www.blockchain.com/explorer/blocks/btc/789537)allows you to visualize a lot of information in the Bitcoin blockchain, we will see in a future article how to decipher and understand all this data. As you can see, a lot of valuable information is stored on[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/).

![](RackMultipart20231011-1-et3x4p_html_fd9b285c74b0af74.png)

## **Hash function and hash**

Imagine you have a magic cake making machine. This machine is very special because you can put any ingredients in it: fruit, chocolate, cheese, even inedible things like shoes or a hairbrush. No matter what you put in it, the machine will always produce the same size cake.

Plus, each combination of ingredients results in a unique cake. If you change the ingredients even a little bit, like adding a pinch more salt, the cake will be completely different.

![](RackMultipart20231011-1-et3x4p_html_1407102feee6a659.png)

This cake maker is very similar to the chopping function used in[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/).

The "ingredients" are the transaction information[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)that you want to record.

If someone tries to change even a tiny part of the transaction information like a number or letter, the "cake" (or hash) will come out completely different. This is how you can ensure that no one has changed the transaction information once it has been saved.

And just like our cake machine, no matter how much information you put into the hash function, it always produces a hash of the same size.

The hashing process involves taking all of the information in a block and putting it through a hash function (e.g. SHA256 for[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/)).

![](RackMultipart20231011-1-et3x4p_html_d707050d1cd43dcf.png)

This function then produces output in hexadecimal\* format of precisely 64 characters. It is important to note that the hash function may vary depending on the cryptocurrency. For example, Litecoin and Dogecoin use the hash function[Scrypt](https://en.wikipedia.org/wiki/Scrypt)rather than SHA256.

\*Hexadecimal is a base 16 positional number system. It uses sixteen distinct symbols to represent numbers. The first ten symbols are the numbers 0 to 9, and the other six are the letters A to F.

| Binary | Decimal | Hexadecimal |
| --- | --- | --- |
| 0000 | 0 | 0 |
| 0001 | 1 | 1 |
| 0010 | 2 | 2 |
| 0011 | 3 | 3 |
| 0100 | 4 | 4 |
| 0101 | 5 | 5 |
| 0110 | 6 | 6 |
| 0111 | 7 | 7 |
| 1000 | 8 | 8 |
| 1001 | 9 | 9 |
| 1010 | 10 | HAS |
| 1011 | 11 | B |
| 1100 | 12 | VS |
| 1101 | 13 | D |
| 1110 | 14 | E |
| 1111 | 15 | F |

The SHA-256 cryptographic hash function always produces a fixed output of 64 hexadecimal characters, regardless of the size or content of the input, ensuring the consistency and security of the processed data.

An input can contain one word or 100,000 words, the output will always be 64 characters long.

You can test for yourself on the site[Blockchain Demo by Anders Brownworth](https://andersbrownworth.com/blockchain/hash)! Type a word of your choice as input in the "Data" field you will always obtain the same output (hash). If you change even the slightest character, the hash changes.

![](RackMultipart20231011-1-et3x4p_html_26e4466866653976.png)

So instead of checking the entire data of a block of the blockchain, it is enough to simply check the hash of each block, if a character in a block has changed, then the hash changes and it shows. It is thanks to this trick that the numerous nodes on the network[Bitcoin](https://coinacademy.fr/bitcoin-btc-fondamental/), anywhere in the world, can verify in real time that the data written in the blocks remains intact.

Hash functions are designed to be unidirectional, that is, they transform input data into a single output in an irreversible manner. This means that from the hash it is practically impossible to find the original data. This property is fundamental to guarantee the security and integrity of data, particularly in the context of cryptography.

## **The blocks of the blockchain are linked together, hence the expression "block chain"**

![](RackMultipart20231011-1-et3x4p_html_61d1eda58bddfe28.jpg)

The term "blockchain" is[derivative](https://coinacademy.fr/academie/produits-derives-crypto-monnaies/)the way this technology stores information: in blockchains. Each "block" contains a certain number of transactions and data. When a block is filled, it is "sealed" with a hash and then a new block is created linked to the previous one. This link creates a chain of blocks, hence the name "blockchain".

![](RackMultipart20231011-1-et3x4p_html_f4e2de351bfbbf68.png)

This structure allows for great security and transparency of information, because each block is linked to the previous one, making retroactive changes extremely difficult.

You can test for yourself on the site[Blockchain Demo by Anders Brownworth](https://andersbrownworth.com/blockchain/hash): have fun writing information in the Data field of the first 2 blocks then click on the blue "Mine" button. Then change data in the Data field of the first block, you will instantly see that the hash of the first block will be different from the hash indicated in the "Prev" field of the next block.

![](RackMultipart20231011-1-et3x4p_html_9e55cf933e245fe8.png)

Now that the notion of blockchain is clearer, we will be able to look in more detail at how a transaction works.

#
# **What you must remember**

[Free Bitcoin Training – 2023 Edition](https://coinacademy.fr/formations/bitcoin-ca/)[5. Understand the usefulness of the Bitcoin blockchain](https://coinacademy.fr/cours/comprendre-lutilite-de-la-blockchain-bitcoin/)[What you must remember](https://coinacademy.fr/chapitres/btc-ce-quil-faut-retenir-5/)

**IN PROGRESS**

- Blockchain is a decentralized, secure and transparent information storage and transfer technology.
- Once a block has been added to the chain, it is virtually impossible to modify or remove it. This ensures that the data stored in the blockchain is permanent and resistant to tampering.
- Blockchain is often compared to a public, distributed accounting ledger that records[transactions](https://coinacademy.fr/academie/transaction-blockchain/)and other types of data
- When a block is filled, it is "sealed" with a hash and then a new block is created, linked to the previous one. This link creates a chain of blocks, hence the name "blockchain" because the blocks are linked together.
- A hash function is a mechanism that transforms input data into a unique output in an irreversible manner.
- On Bitcoin, the SHA256 hash function is used: the output is always 64 characters regardless of the number of input characters.
- Hexadecimal is a number system using sixteen distinct symbols to represent numbers. The first ten symbols are the numbers 0 to 9, and the other six are the letters A to F.
- Checking the hash of a block allows you to verify that the data written in the block is intact.


[Next Section ->](07-complete-operation-of-a-bitcoin-transaction.md)