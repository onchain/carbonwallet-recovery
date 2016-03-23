Carbon Wallet Recovery Tool
============================

You can use this open source tool to send all the coins from your CarbonWallet backup to any bitcoin address you choose.

In order to do this you will need the data from your wallet backup that you either printed out or saved somewhere. It would loo  something like this.

![Wallet Backup](https://raw.githubusercontent.com/onchain/carbonwallet-recovery/gh-pages/wallet-backup.png)

You can download this github code and use it locally or you can trust github and access it with the link below.

http://onchain.github.io/carbonwallet-recovery

## Usage

### Required input

To complete this recovery process, you will need the following information:

* 2 extended public keys (xpubkeys)
* 1 BIP38 Keys
* Your Carbon Wallet passphrase
* Your CarbonKey backup passphrase

### Online/Offline

Internet connection is only required in **Step 1**, where you input the public keys, so that we can fetch the unspent outputs from your vault addresses.

Before inputting your keys in **Step 2** and signing the transaction you can safely go _offline_.

In **Step 3** you will get a signed transaction in raw hex form.

You can then copy this transaction and verify it with [Bitcoin Core](https://bitcoin.org/en/download) and `decoderawtransaction` or using an online tool like [Coinb.in](http://coinb.in/multisig/#verify).

After verifying you then broadcast it using [Bitcoin Core](https://bitcoin.org/en/download) and `sendrawtransaction` or any other API or client that supports broadcasting transactions into the Bitcoin network.

### Running

http://onchain.github.io/carbonwallet-recovery

#### Running locally

Download the files and access index.html from your browser. (Tested with Firefox)


