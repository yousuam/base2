# base2
Understanding How Base Achieves Low Fees Through Optimism’s OP Stack  Base is built on the OP Stack, which batches transactions and posts compressed data to Ethereum. This architecture allows fees to remain extremely low while maintaining security.
from web3 import Web3

eth = Web3(Web3.HTTPProvider("https://ethereum.publicnode.com"))
base = Web3(Web3.HTTPProvider("https://mainnet.base.org"))

gas_price_eth = eth.eth.gas_price
gas_price_base = base.eth.gas_price

print("ETH gas price:", gas_price_eth)
print("Base gas price:", gas_price_base)
print("Base is cheaper by:", gas_price_eth / gas_price_base)
How much cheaper is Base in your results?
