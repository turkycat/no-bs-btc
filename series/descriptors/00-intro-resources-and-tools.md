# intro

this series of videos is meant to help explain how modern descriptor-based wallets work. I will attempt to demonstrate the explain the concepts so that anyone can understand them, but these videos are developer-focused.

wherever possible I will demonstrate the tools you can use to explore these concepts yourself and improve your understanding. The best way to learn is by doing- so I encourage you to follow along and experiment on your own machine.

# resources

https://learnmeabitcoin.com/

BIP-380 -- Output Script Descriptors General Operation
(The general descriptor reference)
https://github.com/bitcoin/bips/blob/58ffd93812ff25e87d53d1f202fbb389fdfb85bb/bip-0380.mediawiki

BIP-382 -- Segwit Output Script Descriptors
https://github.com/bitcoin/bips/blob/58ffd93812ff25e87d53d1f202fbb389fdfb85bb/bip-0382.mediawiki

# tools used

## bitcoin explorer

https://github.com/libbitcoin/libbitcoin-explorer

as of version 3.8 the `seed` command is removed from `bitcoin-explorer`. You can replicate the behavior using the following command, but please note that this is not a cryptographically-secure means of generating entropy and should not be used to create production wallets that secure real money. Many people have been burned by this in the past, hence the removal of the function.

```bash
xxd -l 24 -p /dev/urandom
```

## bdk & bdk-cli

Bitcoin Development Kit (BDK) is a Software Development Kit (SDK) written in Rust. The BDK Rust Crate can easily be added to any Rust project. The CLI is a Command-Line Interface built on top of BDK which can be used within your terminal to utilize BDK functionality without writing any code.

**bdk github home:**
https://github.com/bitcoindevkit

**bdk:**
https://github.com/bitcoindevkit/bdk

**bdk-cli:**
https://github.com/bitcoindevkit/bdk-cli

# alternative resources or tools

https://en.bitcoin.it/wiki/Deterministic_wallet_tools

https://github.com/jlopp/xpub-converter
