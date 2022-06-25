# Web3 Development

## Traditional Finances (TradFi)
	Is characterized, control, adn exceclusion of ratail investros from many
	financial services
		Ex:
		- Banks
		- Funds
		- Brokesrs
		- Fintech
		- Exchanges

	Type of Financial Intruments

	1. Cash Instrument
		- Securities
		- Deposit
		- Loans
		- Bonds
	
	2. Derivative Instrument
		- Forward
		- Future and Options
		- Interest Rate Swap
	
	3. Foreign Exchange

	4. Commodities
		- Soft Comodities... Agriculture
		- Hard Commodities... Natural Resources

### Cons
	What is wrong with TradFi?
	1. Slow System
	2. High Fees
	3. Systems can be Hacked
	4. Systems have downtime
	5. Small groups control everithing

## Decentralized Finances (DeFi)
	It Offers financial intruments without relying on
	intermediaries such as brokerages, exchanges,
	or banks by using SMART CONTRACTS on a blockchain

### Objectives
	1. Reduce transaction time
	2. Reduce transaction fee
	3. Decentralization
	4. Increse access to financial services
	5. Remove intermediaries

### DeFi Fundamental Elements
	1. Cryptography
	2. Smart Contracts
	3. BlockChain

### DeFi Benefits
	1. Permissionless
	2. Decentralization
	3. Trustless
	4. Transparent
	5. Censorship Resistant
	6. Programable

### DeFi Use Cases
	1. Payments
	2. Trading
	3. Lending
	4. Borrowing
	5. Saving for the future
	6. Providing Liquidity
	7. Insurance
	8. Derivatives

## Cryptocurrencies
	A digital currency in wich transactions and records are
	verified and maintained by a decentralized system, instead
	of a centralized authority.
	
	Importante Characteristics:
	1. Launch dates
	2. Launch price
	3. Number of coins in circulation
	4. Actual Price
	5. Market capitalization

## Tokenomics
	It covers all aspects involving a coin's creation management
	and sometimes romoval from a network.

	
	Tokenomics determine two things about a crypto economy
	1. The incentives that set out how the token will be 
		distributed
	2. The utility of the token that influence its demand

### Main developer-defined variables that affect tokenomics
	1. Mining and Stacking
	2. Yields
	3. Token Burn
	4. Limited vs unlimited suplies
	5. Token allocations and vesting periods

## Stablecoins
	Is a cyptocurrency that's linked to one or more undelying
	assets in order to minimize volatility
	
	Benefits:
	1. Low fee
	2. Secured Stability
	3. Faster Speed
	4. Transparency
	5. Programmable

### Staiblecoin Types
	1. Fiat-collateralized Stablecoin- Baked by fiat currency,
		they are 1:1 ratio backing. Dai, Tether, USDC, Parrallel

	2. Commodity-backed Stablecoins- Baked by different types of
		interchangable assets such as precious metals. Digix Gold,
		Palladium Coin
	
	3. Crypto-backed Stablecoins- Offer better decentralization
		in comparison to fiat-collateralized stablecoins. In 
		addition, stablecoins are over-collateralized for 
		absorbing price fluctuations as collateral. WBTC
	
	4. Algorithmic Stable Coins- Algoritm for controlling the
		stable coin supply. Such a type of approach is 
		also known as seigniorage shares. With the raise in 
		demand, new stablecoins will be created by reduce the
		price reducing circulating supply. UST(Luna), Magic
		Internet Money

## Centralized Exchanges
	Benefits:
	1. Easy to use
	2. Advanced tools
	3. High Liquidity
	4. Customer Service

	Disadvantages:
	1. They control your funds
	2. Require your personal information (KYC), takes time.
	3. Apps can be hacked, or servers can fail.
	4. High-cost fees for transactions.

## Decentralized Exchanges (DEX)
	Cryptocurrency exchange which allows for direct
	peer-to-peer cryptocurrencu transactions to take place
	online securely and witout the need for an intermediary.

	Benefits:
	1. The user controls the coin.
	2. Totally anonymous
	3. Less likely to be downtime
	4. Transactions fees may be lower
	5. Access to new projects

	Disadvantage:
	1. Not that easy to use
	2. Basic tools
	3. Low liquidity
	4. There is no customer service
	5. There are many scams.

### Liquidity Pools
	A liquidity pool regers to a pool of tokens that are
	loked in a smart contract, wich is a self-executing program
	based on the agreements between th ebuyer and seller.

### Impermanent Losses
	Is a a unique risk involved wiht providiong liquidity
	to duel-asset pools in DeFi protocols. Simply put, 
	impremanent loss in the difference between holding tokens 
	in AMM and holding the in your wallet.

	Places to Look for "Good" Liquidity Pools

	Defi Pulse & DefiLlama

### Things to consider before using DeFi projects

	1. Has the Project's code Been Audited?
	2. Does it hace a use case>
	3. Does it provides relevant documentation?
	4. Is there a team behind the project
	5. Does the DeFi project have reputable backers?
	6. Does it have an active community?
	7. Tokenomics

## Bridges
	A bridge or cross-chain bridge is a system that tranfers
	information between two or more blockchains and between
	second-level scaling solutions

## ERC-20 Tokens

	A token can represent virtually anithing in a Blockchain.

	The ERC-20 introduces the standard for Fungible Tokens

### What are ERC-20 tokens
	1. ERC stands for Ethereum Request for Comments.
	2. ERC-20 is a "token standard" for creating Eth token 
		contracts
	3. Any token contract that adheres to specificatio
		follows ERC-20

### Methods (functions)
	1. Name:
		Returns the name of a token
		ex:
			function name() pyblic view returns(string)
	2. Symbol:
		Returns the simbol of a token. E.g. "HIX"
		ex:
			fucntion symbol() public view returns (string)
	3. Decimals:
		Returns the number of decimals the token uses. 8, means
		to divide the token amount by 100000000 to get it user 
		reptesentation
		ex:
			function decimals() public view reutrns(uint8)
	4. Total Sypply:
		Returns the total token supply.
		ex:
			fucntion totalSupp;y() public view returns (uint256)
	5. Balance of:
		Returns the account balance of another accoun
		with address _owner.
		ex:
			function balanceOf(address_owner) public view returns
			(uint256 balance)
	6. Tansfer:
		Transers_value amoutn of tokens to address_to, and MUST
		fire the transfer event. The function SHOULD thwow if the message
		callers account balance does not hace enough tokens to spend
		ex:
			function transfer(address_to, uint256_value) public returns (bool success)
	
	7. Approve:
		Returns the amount which_spender is still allowed to withdraw form_owner
		ex:
			functions approve(address_spender, uint256_value) public returns(bool success)

	8. Allowance:
		Returns the amount wich_spender is still allowed to withdraw from_owner
		ex:
			function allowance(address_owner, address_pender) public view returns (uint256
			remaining)

### Methods vs Events

	A method or function is a basically a group of code that can be reused anyware in
	the program.

	Event notify the applications about the change made to de contracts and
	applications wich can be used to execute the dependent logic. They are
	used to inform the calling application about the current state of the contract, with
	the help of the logging facility of ENV

	1. Event- Transef:
		Must trigger when tokens are transferred, including zero values transfers.
		A token contract wich creates new tokens SHOULD trigger a Transer
		event with the_form address set to 0x0 when tokens are created.
		ex:
			event Transfer(address indexed_form, address indexed_to, uint256_value)

	2. Event Approval
		Must trigger on anny successfull call to appove(address_spender, uint256_value).
		ex:
			event Approval(address indexed_owner, address indexed_spender, uint256_value)
	

