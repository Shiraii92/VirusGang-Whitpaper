# CAKE Tokenomics

###  <a href="emission-rate" id="emission-rate"></a>

###  <a href="per-block" id="per-block"></a>

\*Effective Emission is in fact slightly below this amount: an additional 45,000 CAKE per day is diverted from the amount allocated to the lottery, and burned (PID 137 - Details below).

In addition to the above, a dynamic amount of CAKE is also [minted to the Dev address](https://bscscan.com/address/0xceba60280fb0ecd9a5a26a1552b90944770a4a0e#tokentxns) at a rate of 9.09%. This means that if 100 CAKE are harvested, then 9.09 CAKE is minted in addition and sent to the Dev Address.

All CAKE minted to the Dev address is burned in the weekly burn and never enters circulation.

As such, we haven't included it in the above emission rate.

###  <a href="distribution" id="distribution"></a>

Reward/block (% of emission)

Reward/block (total CAKE)

of which diverted and burned

Total Daily CAKE Emission

###  <a href="other-deflationary-mechanics" id="other-deflationary-mechanics"></a>

As well as the above, CAKE is also burned in the following ways:

* 0.05% of every trade made on PancakeSwap V2
* 100% of CAKE sent to the Dev address
* 100% of CAKE raised in IFOs
* 100% of CAKE spent on Profile Creation and NFT minting
* 100% of CAKE bid during Farm Auctions
* 20% of CAKE spent on lottery tickets
* 45,000 CAKE per day (historically assigned to the lottery) (The CAKE for this is generated by a farm - PID 137)
* 3% of every Prediction markets round is used to buy CAKE for burning
* 2% of every yield harvest in the Auto CAKE Pool
* 2% of every NFT sale on the NFT Market is used to buy CAKE for burning

###  <a href="why-is-the-cake-burn-manual" id="why-is-the-cake-burn-manual"></a>

To hit the ground running, PancakeSwap launched as an MVP (minimum viable product) with the MasterChef contract emitting 40 CAKE per block. For that reason, the early team didn't add additional functions such as the ability to customize the CAKE minting logic. As migrating to a new MasterChef would require a lot of time and effort, the team opted to reduce CAKE emissions instead through a manual burn process by creating two pools:

* Legacy Lottery Pool (PID - 137) - burned CAKE from the lottery
* Burn Pool (PID - 138) - burned CAKE per block

These pools work similarly to the farms, where the Chefs can adjust the percentage of the 40 CAKE per block allocated to it after each CAKE emission reduction vote.

On the day of the burn, the supply shown on the homepage might suddenly jump by several million CAKE.

Don't worry - THIS CAKE NEVER ACTUALLY ENTERS CIRCULATION:

This apparent jump is just because of how all the CAKE that's allocated for the burn is stored during the week.

The CAKE sent to both pools PID-137 and PID-138 are harvested before completing the weekly token burns, and this makes the Total Supply shown on the site jumping by \~6M. This is because pending CAKE isn???t registered in the Total Supply until it's harvested on the burn day. Once the token burn transaction is completed, the \~6M is shown in the Burned to Date.

###  <a href="how-to-confirm-cake-supply-for-yourself" id="how-to-confirm-cake-supply-for-yourself"></a>

To confirm that the circulating CAKE supply shown on the PancakeSwap homepage is correct,

1. Then, subtract this burned amount from the "Total Supply" that BscScan shows.
2. This gives you the actual CAKE supply.

####  <a href="read-more-about-cakes-deflationary-mechanics-on-the-next-page" id="read-more-about-cakes-deflationary-mechanics-on-the-next-page"></a>
