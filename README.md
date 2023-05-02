
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

![f11](https://user-images.githubusercontent.com/89090776/235647190-2cbeab27-c62b-4af1-9963-bc8d18cbe49c.jpg)
Figure8:It is our metamask wallet account which is running under sepolia test network and which has about ```0.1983 SepoliaEth``` and <br>
our sample contract supports Sepolia test network<br>

![f12](https://user-images.githubusercontent.com/89090776/235647740-89c3868e-8358-4cda-9cdd-847ec5335672.jpg)
Figure9: after clicking the compile button the contract is successfully compiled<br>

![f14](https://user-images.githubusercontent.com/89090776/235648015-28eb31e3-952f-410b-9828-364ab673eb6a.jpg)
Figure10: after clicking the ```Deploy``` button our metamask window will pop up and will show the amount needed for the transaction<br>
we will click the ```Confirm``` button<br>

![f15](https://user-images.githubusercontent.com/89090776/235648530-432e399a-9d61-4cd1-b60e-033da0668c8c.jpg)
Figure11: thus successful transaction occured <br>

![f16](https://user-images.githubusercontent.com/89090776/235648693-1a84d751-9181-4783-b089-f31549e09e65.jpg)
Figure12:then on our deployed contract if we click the ```getLatestPrice``` button we wil get the latest price of ethereum in terms of USD<br>
here which is about ```2809807930000``` it is a large number becauews decimel does not work well at solidity,according to common knowledge <br>
the amount will be ```$2809.807930000```

Price feeds are one of the most powerful out of the box decentralized features you can use your smart contracts to level them up especially for <br>
Decentralized finance(DeFi)<br>

![f17](https://user-images.githubusercontent.com/89090776/235651833-6ec01c32-1620-487f-81ab-d730c40c1849.jpg)
Figure13: If we want different contracts of different price feeds go to this section of this link ```https://docs.chain.link/data-feeds/price-feeds/addresses```<br>


```Chainlink verifiable randomness function``` is another decentralized out of the box feature application.Blockchain are deterministic system which means they can't have randomness<br>

an out of the box feature is a feature that is readily available and can be used immediately after installation or activation, without the need for any further development or modification. This is in contrast to features that require additional coding, customization, or configuration to work properly.<br>


If we can determine what a random number is , it is not really a random number anymore<br>

So we need to get a provably random number by looking outside of the blockchain and oracle are able to do that<br>

Chainlink VRF is a way to get provably random number to guarantee fairness and guarantee randomness of applications<br>
It is used for lotteries,for randomizing NFTs ,for gaming and for more<br>




A provably random number is a number that is generated in a way that is transparent, verifiable, and unbiased, meaning that it cannot be manipulated or predicted by anyone, including the party generating the number.


Chainlink keepers is also an out of the box decentralized feature of chainlink and it is a decentralized event driven execution<br>
chainlink keepers are chainlink nodes that listen to a registration contract for different events that we specify,it can be some minutes or week<br>

End-to-end reliablity is another out of the box feature of chain link and is the ultimate promise of smart contracts and we want them to be able to do anything<br>
by this we want be able to take any input and get any output<br>



![f18](https://user-images.githubusercontent.com/89090776/235679906-a52e758e-412a-486a-b579-5845b2671fbf.jpg)
Figure14: making HTTP GET and HTTP POST request is an easy way to customize our chainlink nodes to make it able do anything<br>


Chainlink nodes can make API calls by themselves. it can make direct request to any API that you specify<br> For this we have to choose both the <br>
chainlink node and URL slash(/) data to send a request to <br>


![f19](https://user-images.githubusercontent.com/89090776/235685687-1d2dc811-636e-42da-8743-5fe6158f3100.jpg)
Figure15: We can take look at example by going through this section of the document<br>


![f20](https://user-images.githubusercontent.com/89090776/235686840-377e0ef9-1abc-4ab9-8a5a-3c61644bf621.jpg)
Figure16: Here our example contract is successfully compiled at remix platform<br>

![f21](https://user-images.githubusercontent.com/89090776/235688095-4a567659-3520-4b31-b5c6-694a02539198.jpg)
Figure17: when we click the ```deploy``` button the metamask windows pop uop showing the amount needed for this transaction and click the confirm button<br>



![f22](https://user-images.githubusercontent.com/89090776/235689112-5ba7cdce-97eb-41f7-a83f-dc11cf7b2b3f.jpg)
Figure18: thus successful transaction occured <br>



![f23](https://user-images.githubusercontent.com/89090776/235689708-0cbd7080-9d43-4f9e-b66b-242e743ee048.jpg)
Figure19: this is our deployed contract<br>

Whenever we request data from chainlink node we have to pay a little bit of Oracle gas or link token



















