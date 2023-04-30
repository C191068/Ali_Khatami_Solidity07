## Ali_Khatami_Solidity07

### Oracle and chainlink

To convert ethereum to USD, oracle and chainblink are needed.The USD value of ethereum is something that we have assigned outside of the blockchain to each ethereum.
In order to get any value that is outside of the blockchain we have to use decentralized oracle network to get the price of one ether in bterms of USD.
We have to note that blockchain are deterministic systems which means they can interact with real world data and events.It can do any external computation.
Blockchains can't all agree on what random number is.If we start adding random that return from API(Application programme interface) call, diiferent nodes <br>
will get differnt results and they would never reach a consensus.Such problem is called smart contract connectivity problem or Oracle problem.<br>
For this problem we can't replace smart contracts with traditional agreements and traditional agreements neeed data and they need to interact with real world.<br>


Blockchain oracle is gonna be any device that interacts with off-chain world to provide external data or computataion to smart contracts<br>
We have to keep in mind that we don't want to get or external computation through centralized nodes<br>
Chainlink is a decentralized Oracle network for bringing data and external computation into our smart contracts<br>
Hybrid smart contracts combine on chain and off chain to make incredibly feature rich and powerful applications<br>
Chainlink is also modular decentralized oracle network that can be customized to deliver any data or do any external computataion that we like<br>
Blockchain nodes can't make https calls<br>

features of chainlink<br>

1.Chainlink data feeds: it is powering over 50 billion dollars in the DeFi world. The way it works that a network of chainlink nodes gets data from differnt <br>
exchanges and data providers and brings that data through a network of decentralized chain link nodes and the nodes use a meduium to figure out what the<br>
actual price of the asset is and then deliver that in asingle transaction to what is called a reference contract/price feed contract/data contract<br>
The smart contract use those pricing information to power their DeFi(Decentralized finanace) application<br>

A better example of it we can see by visiting this link https://data.chain.link/ where we can change networks,price feeds <br>

![f4](https://user-images.githubusercontent.com/89090776/235355940-6d255edb-3324-441b-962d-1f743e005385.jpg)
Figure1:On Eth/USD we can see a whole network of independent chain link node operators each giving differnt answers for Eth/USD<br>
here Deviation threshold 0.5% means how often they are updated

![f5](https://user-images.githubusercontent.com/89090776/235356200-2190e2c3-0599-4441-b310-5185fff0e9f0.jpg)
Figure2: here we can see it was last updated 51 minutes ago<br>

Like the transaction gas whenever the chainlink node operators delivers data to smart contract they are paid little bit of oracle gas in chainlink token<br>
![f6](https://user-images.githubusercontent.com/89090776/235356606-f1b508e8-f872-4c0f-876f-6b6b20b06c80.jpg)
Figure3: here these users are paying these oracle gas<br>

Data feeds are use by some largest protocols in space. they are<br>
They are:<br>
1.Synthetic(synthetic assets) secured 3 billion USD<br>
2.SushiSwap(Dex) secured 3 billion USD<br>
3.Compound(lending and borrowing) secured 10 billion USD<br>
4.AAVE(lending and borrowing) secured 15 billion USD<br>

to see example we will go to this link https://docs.chain.link/ <br>

![f7](https://user-images.githubusercontent.com/89090776/235358084-bda8ad5e-dbf0-4435-8881-514ce2ece474.jpg)
Figure4: Then we will click on Data Feeds option

![f8](https://user-images.githubusercontent.com/89090776/235358181-a2cc77c2-74fe-444a-9615-688107f07e1d.jpg)
Figure5: then we click on the left side under ```Ethereum and EVM chains``` section ```Using Data Feeds``` option

![f9](https://user-images.githubusercontent.com/89090776/235358429-619253f1-5ea0-419c-8a13-9d5b094594bb.jpg)
Figure6: if we scroll down we will see a sample contract and we will open this at Remix.

![f10](https://user-images.githubusercontent.com/89090776/235358588-819e004c-509d-43db-938a-28179d567267.jpg)
Figure7: here it is reading from a price feed on sepolia<br>















