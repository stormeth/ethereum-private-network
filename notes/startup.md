Copy the files from this top level folder called genesis to

/tmp67/ethgenesis

### gethinit1

Initialize your --datadir with the genesis block

```
alias gethinit1='geth --datadir /tmp67/why1 init /tmp67/ethgenesis/genesis1.json'
```

### accnew1

Set up a new account on Ethereum

```
alias accnew1='geth --datadir /tmp67/why1 account new'
```

The above command will return an account number which you will insert next.

See genesis2.json on how to alloc to the above account.

### gethinit2

And run this command again:

```
alias gethinit2='geth --datadir /tmp67/why1 init /tmp67/ethgenesis/genesis2.json'
```

### gethc

Then go ahead and bring up your geth console with this command

```
alias gethc='geth --datadir /tmp67/why1 --nodiscover --maxpeers 0 --rpc --rpccorsdomain "http://localhost:3000" console'
```

The following commands will show the amount of ether in the account

```
eth.accounts
primary = eth.accounts[0]
balance = web3.fromWei(eth.getBalance(primary), "ether");
```
