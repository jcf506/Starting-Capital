# StartingCapital

## Summary
Harold would like to raise 10 Ether and with that Ether lend it out so it continually earns interest while borrowing only 10% of the dollar value of 10 Ether. With that amount (1Ether), he knows he can fund the integral parts of his startup business over the next 12 months. While the debt is held, it is assumed the interest rate received from lending the Ether will outweigh the interest payments on the USDC, effectively growing the amount of Ether in the pool. When Harold and his team have built their product and have sufficient revenue, they will pay back the debt and return Ether back to the Crowdsale depositors with interest accrued from the pool. The team will also receive payments in $COMP, a "compound.finance" native governance token generated as a result of the activity of borrowing and lending on the "compound.finance" debt-swap platform. This token can be converted into Ether to pay for gas costs associated with returning the investors’ investments.

Essentially, on the "compound.finance" platform, Harold’s team is able to use 10 Ether raised from the Crowdsale to mint cETH which earns a rate of 0.58% APR.  The team then uses the minted cETH as collateral to borrow 10% of the net dollar value in the form of USDC, a US Dollar stablecoin on Ethereum.  Since the USDC is borrowed, Harold is charged 2.14% APR.  Because the amount borrowed is only 10% of the amount of loaned Ether, there is a net spread of 0.4% added to the collateral pool per annum.  This compounded interest and the 10 Ether of principal is returned to the Crowdsale participants (investors) as ROI.  The 1 ETH worth of USDC that is borrowed from the pool of Crowdsale funds is used as operating capital by Harold’s team to generate earnings to repay the USDC debt.


## Requirements
* Crowdsale Contract
* Deployment Contract
* ERC20, ERC20 Detailed, ERC20 Mintable Contracts
* Compound Interaction Contract

## Inner Workings
* Conduct Crowdsale (raise 10 Ether)
* Mint cETH using 100 Ether and Compound.finance
* Borrow USDC agasint the minted cETH
* Transfer USDC to team wallet

## Important Addresses and Contract Addresses
* Harold's Address (Deploys Contract and Receives USDC): 0xf7171695A9B0B9E01423420F53419D36479515cf
* Crowdsale Contract Deployment Address: 
* cETH Address: 0x41b5844f4680a8c38fbb695b7f9cfd1f64474a72
* USDC ERC20 Address: 0xb7a4f3e9097c08da09517b5ab877f7a917224ede
* COMP ERC20 Address: 0x61460874a7196d6a22d1ee4922473664b3e95270
* Comptroller Address: 0x5eae89dc1c671724a672ff0630122ee834098657
* Price Oracle Address: 0xbBdE93962Ca9fe39537eeA7380550ca6845F8db7
* cUSDC Address: 0x4a92e71227d294f041bd82dd8f78591b75140d63

## Process
* CapitalTokenSaleDeployer (3 arguments)
* Grab sct_sale_address from contract, use it for At Address, deploy Starting Capital
* Use 1 for value box and ether to get 1 token
* Grab token address from token_address to add token to metamask

## Important Links
* https://github.com/compound-developers
* https://compound.finance/docs
* https://medium.com/compound-finance/supplying-assets-to-the-compound-protocol-ec2cf5df5aa
* https://medium.com/compound-finance/borrowing-assets-from-compound-quick-start-guide-f5e69af4b8f4
