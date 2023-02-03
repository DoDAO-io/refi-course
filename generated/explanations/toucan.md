## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

 ---
 
 ## Toucan protocol
 
 **Traditional carbon credit market**        
### Carbon credits and current problems with the credit market

Companies can buy carbon credits to offset their carbon emissions. These carbon credits are not free passes for companies to pollute even more, but a way for companies to compensate for some of the unavoidable emissions that happen during production. So companies buy carbon credits (equivalent amounts of carbon removed / reduced in the atmosphere) in order to offset their “unavoidable emissions.”

Voluntary carbon markets exist today in the real world, but they have a couple of issues:

* **Legitimacy and relevance** of the credits are hard to verify. ( Since different standards of carbon offsetting exists, and they are not all equal)

* **Lack of transparency and unfair pricing**, since these dealings are done behind closed doors, it is hard to know the current market price of given carbon credits and thus makes for an uneven market with disproportionate prices.

* **Loss in value generation**, the dealings are not done directly to the end-user, the credits go through a multitude of middlemen who ultimately contribute to the further lack of transparency and loss in value generated for producer and end-user.

* **Lack of deep liquidity** Another major issue is that carbon credits are not all of the same value. This is because different carbon credits are given for different ways of carbon reduction / removal. Something like using solar energy would come under carbon reduction whereas forestation would come under removal. Clearly, these are vastly different applications whose respective carbon credits also range in their value. This further complicates the already opaque market and makes it even harder to evaluate the carbon credits and their value leading to lack of liquidity in the market. 
 **Carbon credits in DeFi**        
### Carbon Credits in DeFi

Web3, DeFi in particular, has features in place which are very well equipped to solve these issues. 

We are already familiar with the concept of tokenizing real world assets, for example real estate tokenization. Similarly, carbon credits can be tokenized and shifted on-chain to solve the issue of lack of transparency that the current carbon market is facing. With the help of tokenization, these carbon credits can be listed in markets, bought and sold with complete transparency and the user (company) has assurance over the price at which the carbon credits have been bought.
 

But this cannot directly be done. Because the bodies issuing carbon credits operate off-chain, in the physical world and it does not as of now make logistical sense to shift their operations on-chain. So the market needs an entity which can 

1. Tokenize these carbon credits issued by these regulatory bodies, and come up with a standard for the tokenization of carbon credits, and

2. A way to list these carbon credits on the market considering their inherent differences in value and utility. 

This is where protocols like the Toucan protocol come in, providing the much needed Web3 bridge that the aforementioned regulatory bodies lack and need. 
 **Toucan protocol**        
### Toucan protocol

The Toucan protocol is a Web3 infrastructure supporting Regenerative Finance (ReFi). Toucan protocol aims to tokenize carbon credits in order to solve the current issues with the carbon credit market and bring about a regenerative change in the DeFi ecosystem.

They solve the issues mentioned in the section discussed above in the following manner:

* They only tokenize the credit issued by select bodies (Verra is the only source registry as of now), this way the legitimacy of the carbon credits that they tokenize is maintained.

* The protocol is run on Polygon, an EVM compatible blockchain, which solidifies their promise of transparency and adds an additional layer of protection and security against the misuse of the carbon credits (example, double counting of credits).

* They have come up with a system of “Carbon Bridge” and “Carbon pools” to successfully tokenize the carbon credits from the source registry. 

Let us see how the Toucan protocol functions in the coming section.   
 **Working of Toucan**        
### Working

Carbon credits in the source registry are categorized on the basis of nationality, type of carbon offset and the standard on which they have been evaluated. So, each project in the source registry has a different set of parameters to be considered before shifting them on-chain.

There are a few issues that the users face when it comes to the traditional carbon credit market as mentioned above. Let us revisit those issues, and see how Toucan protocol aims to solve them.

1. **Lack of transparency:** Double counting and irregular pricing: The carbon credit market lacks transparency, this leaves the user in a situation where they could be sold a carbon credit that is double counted, or a carbon credit at a price far above its market value.

2. **Lack of liquidity:** The carbon credit market has too much variation. As mentioned earlier, there is difference in project, vintage, type of emission offset, country, etc. This means each carbon credit has a different value and it is very hard to create deep liquidity of any of these tokens because of their vast differences and incoherence in the existing market.

3. **Loss of value:** There are a multitude of middlemen in the system, who muddle the process and increase the intensity of issues 1 and 2. The existence of middlemen also reduces value created by the project and the end–user.

The Toucan protocol addresses these issues in the following manner,

1. The issue of double counting, lack of transparency, and unfair pricing could be solved by taking the carbon credit on-chain. This would mean that each credit is only counted once, and given the immutable and transparent nature of the blockchain, the user can be assured of the legitimacy, and fairness of a carbon credit transaction. The Toucan protocol takes the physical carbon credits present in the source registry to the blockchain using something called a **Carbon bridge**, explained in the coming section.

2. The issue of middlemen, unfair pricing and lack of liquidity could be solved by listing these tokenized carbon credits in the markets in a pooled fashion, where all the kinds of tokens present in the pool would be represented by a representative **pool token**. Toucan does this by using something called **Carbon pools**, explained in the following sections. This way, each set of tokens can achieve deeper liquidity, and the listing of tokens on the blockchain will readily remove the issue of middlemen and improve value generation for both end-user and producer. 

Now that we have understood what Toucan protocol employs to tackle the issues in the traditional carbon market, let us look at how they employ their methods in a little more detail. 
 **Carbon bridge**        
### Carbon bridge

Toucan brings the carbon credits from the source registry onto the blockchain using something called Carbon Bridge. It is a one way bridge which can transfer the credits from off-chain to on-chain and not vice versa, meaning bridging is an irreversible process. Before the tokens can be shifted on-chain, they need to be retired from the source directory, this is done so that the credits are not double counted (Exist both on-chain and off-chain, i.e counted twice). This way, burning the carbon credit on-chain will be equivalent to the token being retired off-chain.

In order to bridge, a few requirements are put in place:

1. Firstly, to transfer carbon credits to the blockchain, you need carbon credits in the real world. Currently, Toucan only performs carbon bridging for Verra registries. You also need to be able to retire those credits from the Verra registry, or someone who can do it for you.
           * The methodology applied in the project issuing the VCUs must not be included in the blocklist of methodologies.
           * The difference between the date of verification (vintage) and the date of issuance of the credits must be less than 10 years.


2. An Ethereum account controlled by your Metamask wallet, with the native token of the polygon blockchain.

The credits are bridged in a batched fashion and not one at a time. These batches are represented in the form of an NFT called BatchNFT. The user must create a link between the retired credits on the registry and the BatchNFT by including the unique identifier of the BatchNFT in the retirement note (specified under “Retirement Detail”)  of the credits. On retiring,  the user is provided with a serial number by the source registry. This serial number carries a lot of relevant information, including the number of offsets, certifying standard body, project identifier, country, monitoring period (vintage), and more. The next step is to update the BatchNFT metadata with this serial number, with that the credits will be successfully transferred on-chain. These steps are key because they ensure that double counting / double bridging of carbon offsets is not possible. 

The steps mentioned above are all part of the Carbon Bridge and are part of the Toucan protocol, not something the user does on their own, it has been explained in such a way in order to generalize the concept instead of providing a walkthrough of the bridging process.

Once the BatchNFT is updated with a serial number, it needs to be approved by a Toucan Verifier, a trusted member of the Toucan community. This step is required to protect against fraudulent inputs and is dependent on human action and trust, for now.

### Fractionalize

These BatchNFTs are ERC721 tokens which can be traded as NFTs but there is another way of dealing with the BatchNFTs. That is, fractionalization. These NFTs can be further fractionalized into its constituent carbon credits in the form of ERC20 tokens, called T20 tokens which can be traded. 1 TCO2 token represents 1 carbon credit with a value of 1 tCO2e. So, an NFT representing a batch of 100 credits can be fractionalized into 100 TCO2 tokens.

TCO2 token contracts still carry all the attributes and metadata of the NFT, making them specific to a given project and vintage. This is crucial because voluntary market carbon credits trade at very different price points due to credits of a certain type or with specific attributes being more sought-after than others. This system guarantees that a soil carbon project with additional certification can be priced higher than a large-scale renewable energy project.

Now the issue of credit markets arises, due to the wide variety of their categories and projects. Toucan aims to solve this issue using something called “Carbon Pools”, quite similar to liquidity pools in DeFi. 
 **Carbon pools**        
### Carbon pools

Before diving deep into Carbon pools, we need to understand the classification of these Carbon credits. 

The carbon credits can be classified as removal (Carbon removed from atmosphere) credits and reduction (Avoiding / reducing the carbon emitted) credits. Apart from this, they are further classified based on,

* **Project type -** Different approaches to reducing greenhouse gasses in the atmosphere are more or less effective and their value changes accordingly.

* **Country -** Project costs are higher in some countries than others, plus credits from some countries may be perceived as higher-quality than from other countries.

* **Carbon standard -** Some standards are more rigorous than others.

* **Co-benefits -** Some projects seek additional certification from standards like the Climate, Community and Biodiversity Standards (CCB Standards), which certifies additional benefits like an increase in biodiversity or specific Sustainable Development Goals (SDGs).

This results in a scenario where the credits are sold as individual products and not commodity. Also, the lack of transparency of these carbon markets means that the prices of these credits are unknown to the broader market, creating an uncertain scenario for the user who is buying credits without knowing if it is a fair price or not.

In order to commoditize these carbon credits, Toucan aims to pool similar types of Carbon credits together in order to produce a transparent price signal to the market. These standardized carbon tokens can be traded on DEXs (decentralized exchanges) with much deeper liquidity than a single project's credits ever could. 

**Overview*

Basically, the user can deposit their credits to the Carbon pools which have a set of criteria that the T20 token must pass, once passed, the token will be locked in the pool and a pool token of equivalent value will be sent to the user regardless of the difference between the projects as long as they are in the same pool. The pool token can then be redeemed at any given moment by the user, following a few guidelines explained later.

**Pool logic**

Each pool has a unique configuration and carries a certain logic that dictates which TCO2 tokens can be deposited into it. This logic is based on two filters: If the deposited token is a TCO2 token. If the deposited TCO2 token satisfies the pool requirements. For example, could create a carbon reduction pool, with a token called CRedT (carbon reduction tonne). This specific pool would only carry one defining attribute: type = reduction. In this case, the carbon reduction reference token could be called CRedT.

**Current Carbon pools**
Currently there are two carbon pools in the Toucan protocol, BCT and NCT. As mentioned earlier, these pools have their own inclusion and exclusion criteria in order to better segregate similar kinds of carbon credits together. These segregation criteria are important to make sure that the different tokens present in each of these pools are of similar value, if not equivalent value.


* **BCT**

BCT includes projects dealing with all Verra approved methodologies except “Decomposition of fluoroform (HFC-23) waste streams”, meaning most projects registered under the Verra registry are eligible to be listed in the BCT pool.

* **NCT**

NCT includes projects dealing with forestation and ecosystem conversion in general. For example, the carbon credits produced by a project involved in increasing the number of trees in a forest, reviving a dead ecosystem etc. would come under consideration to be listed in the NCT pool.

**Deposit**

To deposit into a carbon pool, a TCO2 token must successfully pass the logic filter. If it does, the token gets locked inside the pool, and a carbon reference token (like a BCT token) is created and sent to the depositor's wallet. Carbon reference tokens are fungible ERC20 tokens — every carbon reference token is backed by a carbon credit that has the attributes gating that pool.

**Redeem**

At any point, the holder of a carbon reference token can redeem it for an underlying project-specific TCO2 token. This burns the carbon reference token and sends the underlying tokens to the user.

This opens up arbitrage opportunities if a particular TCO2 could be deposited into multiple pools, and guarantees the creation of a price floor for on-chain carbon reference tokens.

It's important to note that when redeeming, you can:

* auto redeem (which gives you the lowest ranked TCO2s)

* selectively redeem (which gives you the TCO2s you specify and costs a fee)


**Burn**

This action is equivalent to retiring the credit in the traditional market. Once burnt, the pool token and its underlying token will be taken out of circulation. Once the end-user receives the tokens and wants to use them to offset their carbon emissions, it would be burnt. 

**Adding new pools**

A Toucan Pool Party is the participatory process for launching a new Carbon Pool. A Pool Party brings together a multidisciplinary set of stakeholders who represent different interest groups who want to see the pool succeed and thrive. Over the course of several weeks, they discuss gating criteria, threats, risks, and launch plan and alignment forms. 
 **References**        
### Resources:

https://docs.klimadao.finance/blogs/about-carbon-offsets

https://docs.toucan.earth/toucan/introduction/overview 
 
