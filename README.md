# Dion Pay-Chain
## Specifications and uses of the Dion Pay Utility Chain

Dion Pay Chain version 0.1.0 beta

"DION" is the ticker for the Dion Pay token. Dion Pay is a utility token, which gives our users access to the services provided by www.dionpay.com


## What is a utility token?

A utility token represents access to a future product or service. When you buy a utility token, you are buying your “right” to use a service that’s being developed by a project once it’s finished and launched. ChainDion Pay plans to extend the functionalities and implement them into the company structure and services we offer.
    
## Dion Pay Tech Specification

    Max Supply: 143000000000 DION 
    Circulating Supply: 3900000000
    Block Time: 1M
    Block Reward: 222.22
    Mining Algorithm: Equihash
    RPCPORT: 23895
    This version of Komodo Independent Chain contains Bitcore support for komodo and all its assetchains.    

## Dion Pay Resources

    Website: https://www.dionpay.com
    Twitter: https://twitter.com/DionPay
    BitcoinTalk: 
    Email: info@dionpay.com
    

## Getting started
Dependencies
------------
Install Komodo: https://docs.komodoplatform.com/en/latest/komodo/install-Komodo-manually.html#installing-komodo-manually

After installing the Komodo repository, DONOT run the Komodo deamon, instead follow the steps:

`cd Komodo/src`

# Now run the following command to start the Dion Pay daemon

`./komodod -ac_name=DION -ac_supply=3900000000 -ac_reward=22260000000 -ac_staked=100 -ac_cc=1 -ac_end=4300000000 -addnode=51.75.124.34`


Once the Dion Pay chain is synched, you are able to use the wallet functionality

# Commands
In order to perform a command you must navigate to

`cd komodo src`

and execute commands with the following prefix

`./komodo-cli -ac_name=DION`

i.e. Command to get wallet info

`./komodo-cli -ac_name=DION getinfo`

# Main Commands
## Wallet
- getinfo
- backupwallet "destination"
- dumpprivkey "Dion Pay address"
- dumpwallet "filename"
- encryptwallet "passphrase"
- getaccount "Dion Pay_address"
- getaccountaddress "account"
- getaddressesbyaccount "account"
- getbalance ( "account" minconf includeWatchonly )
- getnewaddress ( "account" )
- getrawchangeaddress
- getwalletinfo
- importaddress "address" ( "label" rescan )
- importprivkey "dionprivkey" ( "label" rescan )
- importwallet "filename"
- listaccounts ( minconf includeWatchonly)
- listaddressgroupings
- listlockunspent
- listtransactions ( "account" count from includeWatchonly)
- listunspent ( minconf maxconf  ["address",...] )
- lockunspent unlock [{"txid":"txid","vout":n},...]
- resendwallettransactions
- sendfrom "fromaccount" "toDion Payaddress" amount ( minconf "comment" "comment-to" )
- sendmany "fromaccount" {"address":amount,...} ( minconf "comment" ["address",...] )
- sendtoaddress "Dion Pay_address" amount ( "comment" "comment-to" subtractfeefromamount )
- setaccount "Dion Pay_address" "account"
- settxfee amount
- signmessage "Dion Pay address" "message"

## Zero Knowledge Addresses
- z_exportkey "zaddr"
- z_exportviewingkey "zaddr"
- z_exportwallet "filename"
- z_getbalance "address" ( minconf )
- z_getnewaddress
- z_getoperationresult (["operationid", ... ])
- z_getoperationstatus (["operationid", ... ])
- z_gettotalbalance ( minconf includeWatchonly )
- z_importkey "zkey" ( rescan startHeight )
- z_importviewingkey "vkey" ( rescan startHeight )
- z_importwallet "filename"
- z_listaddresses ( includeWatchonly )
- z_listoperationids
- z_listreceivedbyaddress "address" ( minconf )
- z_mergetoaddress ["fromaddress", ... ] "toaddress" ( fee ) ( transparent_limit ) ( shielded_limit ) ( memo )
- z_sendmany "fromaddress" [{"address":... ,"amount":...},...] ( minconf ) ( fee )
- z_shieldcoinbase "fromaddress" "tozaddress" ( fee ) ( limit )
- zcbenchmark benchmarktype samplecount
- zcrawjoinsplit rawtx inputs outputs vpub_old vpub_new
- zcrawkeygen
- zcrawreceive zcsecretkey encryptednote
- zcsamplejoinsplit

## Blockchain
- getbestblockhash
- getblock "hash|height" ( verbose )
- getblockchaininfo
- getblockcount
- getblockhash index
- getblockhashes timestamp
- getblockheader "hash" ( verbose )
- getdifficulty
- getspentinfo

## Control
- getinfo
- help ( "command" )
- stop

## Generating
- generate numblocks
- getgenerate
- setgenerate generate ( genproclimit )

## Network
- addnode "node" "add|remove|onetry"
- clearbanned
- getconnectioncount
- getdeprecationinfo
- getnettotals
- getnetworkinfo
- getpeerinfo
- listbanned
- ping
- setban "ip(/netmask)" "add|remove" (bantime) (absolute)

## For all commands type the following
```
cd komodo/src
./komodo-cli -ac_name=DION help
```
## About Komodo

Komodo is based on Zcash and has been  by their innovative consensus algorithm called dPoW which utilizes Bitcoin's hashrate to store Komodo blockchain information into the Bitcoin blockchain. Other new and native Komodo features are the privacy technology called JUMBLR or our assetchain capabilities (one click plug and play blockchain solutions). More details are available under https://komodoplatform.com/.

## List of Komodo Platform Technologies

    Delayed Proof of Work (dPoW) - Additional security layer.
    zk-SNARKs - Komodo Platform's privacy technology
    Jumblr - Decentralized tumbler for KMD and other cryptocurrencies
    Assetchains - Easy way to fork Komodo coin
    Pegged Assets - Chains that maintain a peg to fiat currencies
    Peerchains - Scalability solution where sibling chains form a network of blockchains
    More in depth covered here
    Also note you receive 5% APR on your holdings. See this article for more details
    CryptoConditions - UTXO based smart and simple contracts


## Komodo Development Resources

    Komodo Web: https://komodoplatform.com/
    Organization web: https://komodoplatform.com/
    Forum: https://forum.komodoplatform.com/
    Mail: info@komodoplatform.com
    Support: https://support.komodoplatform.com/support/home
    Knowledgebase & How-to: https://komodoplatform.atlassian.net/wiki/spaces/KPSD/pages
    API references: http://docs.supernet.org/ #Not up to date.
    Whitepaper: Komodo Whitepaper
    Komodo Platform public material: Komodo Platform public material


Deprecation Policy
------------------

This release is considered deprecated one year after the release day. There
is an automatic deprecation shutdown feature which will halt the node some
time after this one year period. The automatic feature is based on block
height and can be explicitly disabled.


Building
--------
Build Zcash along with most dependencies from source by running
`./zcutil/build.sh`. Currently only Linux is officially supported.

**NOTE TO EXCHANGES:**
https://bitcointalk.org/index.php?topic=1605144.msg17732151#msg17732151

There is a small chance that an outbound transaction will give an error due to mismatched values in wallet calculations. There is a -exchange option that you can run komodod with, but make sure to have the entire transaction history under the same -exchange mode. Otherwise you will get wallet conflicts.

**To change modes:**

a) backup all privkeys (launch komodod with `-exportdir=<path>` and `dumpwallet`)

b) start a totally new sync including `wallet.dat`, launch with same `exportdir`

c) stop it before it gets too far and import all the privkeys from a) using `komodo-cli importwallet filename`

d) resume sync till it gets to chaintip

For example:
```shell
./komodod -ac_name=DION -exportdir=/tmp &
./komodo-cli -ac_name=DION dumpwallet example
./komodo-cli -ac_name=DION stop
mv ~/.komodo/DION ~/.komodo/DION.old && mkdir ~/.komodo/DION && cp ~/.komodo/DION.old/DION.conf ~/.DION.old/peers.dat ~/.komodo
./komodod -ac_name=DION -exchange -exportdir=/tmp &
./komodo-cli -ac_name=DION importwallet /tmp/example
```

License
-------
For license information see the file [COPYING](COPYING).

