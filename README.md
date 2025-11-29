# CyptoWalletMiner

This program is using the bitcoin and requests modules to hunt for private keys with non-zero balances on the blockchain. Here is how it works:

1. The bitcoin and requests modules are imported for generating private/public key pairs and making HTTP requests to the blockchain.info API.

2. A keep_running flag is set to True to control the main loop.

3. The gen_private_key() function uses bitcoin.random_key() to generate a random private key, then derives the corresponding public key and address. This is returned as a tuple. 

4. The check_balance() function calls gen_private_key() to get a new private key/address pair each time. It makes a request to the blockchain.info balance endpoint, checking for any non-zero final_balance under that address. 

5. If a balance is found, the private key is written to a file. Otherwise, it continues looping. 

6. Any errors are caught and printed.

7. The main loop runs continuously, calling check_balance() each time to hunt for private keys holding Bitcoin. This will run indefinitely until stopped.

So in summary, it is generating random private keys and checking their balances on the blockchain via API to "hunt" for any that have coins associated with them.

# Features
✈️ Multi-platform: Android ,IOS , Windows, macOS and Linux

💻 Super Light Programme

# Build and Use
Android IOS Windows macOS Linux
```
git clone https://github.com/HugoXOX3/CryptoWalletMiner
cd BTC Hunter
pip3 install bitcoin
cd Bitcoin_Wallet_Miner
python3 main.py

```
