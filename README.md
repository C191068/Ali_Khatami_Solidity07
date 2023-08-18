

## Ali_Khatami_Solidity07

### Oracle and chainlink

To convert ethereum to USD, oracle and chainblink are needed.The USD value of ethereum is something that we have assigned outside of the blockchain to each ethereum.
In order to get any value that is outside of the blockchain we have to use decentralized oracle network to get the price of one ether in bterms of USD.
We have to note that blockchain are deterministic systems which means they can't interact with real world data and events.It can't do any external computation.
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

It ensures that blockchain applications can react to real-world data changes, like price feeds, without relying on manual interventions<br>
Manual interventions" refer to actions or steps that need to be taken by people. In the context of Chainlink Keepers, it means that without automated systems like Keepers, humans would need to manually check for specific events or changes in the real world and then trigger actions on the blockchain. With Chainlink Keepers, these actions can be executed automatically without the need for human involvement, making the process more efficient and reducing the reliance on manual efforts.<br>




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

Whenever we request data from chainlink node we have to pay a little bit of Oracle gas or link token<br>

In order to pay some link token we need to have some link token in our these example APIconsumer contract 


![f24](https://user-images.githubusercontent.com/89090776/235694995-4b13551d-fcad-4372-a79b-741734c2e470.jpg)
Figure19: For this we will go to https://faucets.chain.link/ and to request for 20 test link which is known as ERC20 token<br>

ERC20 is a technical standard used for creating tokens on the Ethereum blockchain. ERC stands for "Ethereum Request for Comment," which is a type of technical proposal that developers can submit to suggest changes to the Ethereum network.

ERC20 tokens are tokens that follow a specific set of rules outlined in the ERC20 standard. These rules include how the tokens are transferred, how they are tracked, and how they interact with other tokens and smart contracts on the Ethereum network. By following these rules, ERC20 tokens are designed to be easily exchangeable with other ERC20 tokens and to work seamlessly with other applications built on the Ethereum network.<br>



![f25](https://user-images.githubusercontent.com/89090776/235695178-a15f3503-0204-4a6a-b27a-74817bfc37cc.jpg)
Figure20: When we click the ```send request``` button the transfer of token will occur successfully

![f26](https://user-images.githubusercontent.com/89090776/235695286-97c20eed-31f6-427c-ba9e-24d5f96de037.jpg)
Figure21: on our metamask wallet account under asset section we will ckick on ```Import token``` option

![f27](https://user-images.githubusercontent.com/89090776/235695368-ac71a932-4f96-44cd-9fed-936df89f7d8d.jpg)
Figure22: Going to https://docs.chain.link/ we will search for ```Link Token contracts```


![f28](https://user-images.githubusercontent.com/89090776/235696155-65b9da21-10f2-4fa7-b2f1-e49002066675.jpg)
Figure23: At ```Sepolia testnet``` section at ```Address``` part we will click on ```Add to wallet``` button



![f30](https://user-images.githubusercontent.com/89090776/235697663-aa3473da-1cbf-484c-9a3b-4090745d8215.jpg)
Figure24:After we click the ```Add to wallet``` button the metamask window will pop up asking for confirmartion whwther to add 40 link token or not 

![f31](https://user-images.githubusercontent.com/89090776/235697715-4522808d-77cd-48ca-ac00-2eb6e584dafd.jpg)
Figure25: at last 40 link token gets added to our account <br>

Now as we have link or Oracle gas, we are going to send our APi consumer contract<br>


![f32](https://user-images.githubusercontent.com/89090776/235840398-dcf74d4f-8daa-487f-8eae-0a06776b2c67.jpg)
Figure26: for that we will copy the address of API consumer contract <br>

![f33](https://user-images.githubusercontent.com/89090776/235840839-51660c7e-9637-4567-a37d-82af9abc6fb1.jpg)
Figure27: we will click the blue color ```Send``` button<br>

![f34](https://user-images.githubusercontent.com/89090776/235841126-2bfbda61-3e32-4f2c-877b-41187cc4f64c.jpg)
Figure28: We will paste the address and on the asset section we will click 40 link tokeen option<br>

![f35](https://user-images.githubusercontent.com/89090776/235842701-f31ba3b3-aef5-4d70-ba31-177b4df6ac7d.jpg)
Figure29: on ```Edit``` section at ```Amount``` part we will send 0.2 LINK out of 40 LINK<br>

![f36](https://user-images.githubusercontent.com/89090776/235843682-63280bc2-1dbf-48fd-8686-475d8c5b4e3b.jpg)
Figure30: Next we will hit the ```Confirm``` button


![f37](https://user-images.githubusercontent.com/89090776/235844342-a7b426d9-4d86-4d5e-9268-bd9a6324a43c.jpg)
Figure31: When we send LINK to tyhe contract we click the ```Volume``` button as our to target to get volume of last 24 hour of Ethereum asset<br>

![f38](https://user-images.githubusercontent.com/89090776/235844991-7b8a12fd-2e88-4ade-824b-28e4cd6d0aa4.jpg)
Figure32: If we click this link https://min-api.cryptocompare.com/data/pricemultifull?fsyms=ETH&tsyms=USD <br>
It is a link of API which actually we gonna make http get request.

![f39](https://user-images.githubusercontent.com/89090776/235849969-b3a1b623-ecb6-4aad-9418-f57f5e2e4650.jpg)

Figure33: We will see here a ton of raw data and we need to get only these "VOLUME24HOUR":195042.94238641"

Here in the code below

```solidity

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.7;

import "@chainlink/contracts/src/v0.8/ChainlinkClient.sol";
import "@chainlink/contracts/src/v0.8/ConfirmedOwner.sol";

/**
 * Request testnet LINK and ETH here: https://faucets.chain.link/
 * Find information on LINK Token Contracts and get the latest ETH and LINK faucets here: https://docs.chain.link/docs/link-token-contracts/
 */

/**
 * THIS IS AN EXAMPLE CONTRACT WHICH USES HARDCODED VALUES FOR CLARITY.
 * THIS EXAMPLE USES UN-AUDITED CODE.
 * DO NOT USE THIS CODE IN PRODUCTION.
 */

contract APIConsumer is ChainlinkClient, ConfirmedOwner {
    using Chainlink for Chainlink.Request;

    uint256 public volume;
    bytes32 private jobId;
    uint256 private fee;

    event RequestVolume(bytes32 indexed requestId, uint256 volume);

    /**
     * @notice Initialize the link token and target oracle
     *
     * Sepolia Testnet details:
     * Link Token: 0x779877A7B0D9E8603169DdbD7836e478b4624789
     * Oracle: 0x6090149792dAAeE9D1D568c9f9a6F6B46AA29eFD (Chainlink DevRel)
     * jobId: ca98366cc7314957b8c012c72f05aeeb
     *
     */
    constructor() ConfirmedOwner(msg.sender) {
        setChainlinkToken(0x779877A7B0D9E8603169DdbD7836e478b4624789);
        setChainlinkOracle(0x6090149792dAAeE9D1D568c9f9a6F6B46AA29eFD);
        jobId = "ca98366cc7314957b8c012c72f05aeeb";
        fee = (1 * LINK_DIVISIBILITY) / 10; // 0,1 * 10**18 (Varies by network and job)
    }

    /**
     * Create a Chainlink request to retrieve API response, find the target
     * data, then multiply by 1000000000000000000 (to remove decimal places from data).
     */
    function requestVolumeData() public returns (bytes32 requestId) {
        Chainlink.Request memory req = buildChainlinkRequest(
            jobId,
            address(this),
            this.fulfill.selector
        );

        // Set the URL to perform the GET request on
        req.add(
            "get",
            "https://min-api.cryptocompare.com/data/pricemultifull?fsyms=ETH&tsyms=USD"
        );

        // Set the path to find the desired data in the API response, where the response format is:
        // {"RAW":
        //   {"ETH":
        //    {"USD":
        //     {
        //      "VOLUME24HOUR": xxx.xxx,
        //     }
        //    }
        //   }
        //  }
        // request.add("path", "RAW.ETH.USD.VOLUME24HOUR"); // Chainlink nodes prior to 1.0.0 support this format
        req.add("path", "RAW,ETH,USD,VOLUME24HOUR"); // Chainlink nodes 1.0.0 and later support this format

        // Multiply the result by 1000000000000000000 to remove decimals
        int256 timesAmount = 10 ** 18;
        req.addInt("times", timesAmount);

        // Sends the request
        return sendChainlinkRequest(req, fee);
    }

    /**
     * Receive the response in the form of uint256
     */
    function fulfill(
        bytes32 _requestId,
        uint256 _volume
    ) public recordChainlinkFulfillment(_requestId) {
        emit RequestVolume(_requestId, _volume);
        volume = _volume;
    }

    /**
     * Allow withdraw of Link tokens from the contract
     */
    function withdrawLink() public onlyOwner {
        LinkTokenInterface link = LinkTokenInterface(chainlinkTokenAddress());
        require(
            link.transfer(msg.sender, link.balanceOf(address(this))),
            "Unable to transfer"
        );
    }
}

```

By this code ``` req.add("get","https://min-api.cryptocompare.com/data/pricemultifull?fsyms=ETH&tsyms=USD" );``` we gonna make request in one transaction<br>
And in the second transaction the chain link node is gonna return value and store it in this ```volume = _volume;``` variable in global scope



![f40](https://user-images.githubusercontent.com/89090776/235847761-bc270c7b-0457-4115-a56e-69aa24afc7bc.jpg)


Figure34:We will click on ```requestVolume``` button and metamsk window will pop up showing fee for transaction as it is a button due to a gas calling function<br>
Then we will click the ```Confirm``` button

![f41](https://user-images.githubusercontent.com/89090776/235848365-90884a87-adc0-4a3b-a2db-8c194c17c749.jpg)
Figure35: thus our transaction have successfully occured<br>


![f42](https://user-images.githubusercontent.com/89090776/235849304-d215cc4e-e188-4bae-96e0-5032ac2a243b.jpg)
Figure36: then when we click the volume button it has returned equavlent to that API thus it has successfully called the APUI to our contract
































