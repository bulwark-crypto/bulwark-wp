# Feature Set

## Masternodes

Masternodes are, essentially, a decentralized web of computers that serve the Bulwark network. Masternodes perform important network functions and receive part of the block rewards. They serve the Bulwark ecosystem by stabilizing coin supply, processing transactions, and securing the network. Masternodes require 5000 BWK and modest technical knowledge to operate. Any wallet controlling 5000 BWK can set up a masternode.

## Obfuscation / Coin Mixing

Bulwark features Obfuscation, based on CoinJoin but with various improvements over the original, and done via coin mixing in a decentralized fashion facilitated by the network of masternodes. This provides an additional layer of privacy in transactions. While not perfectly anonymous, Obfuscation via node mixing it is far better than the standard Bitcoin transaction. For example, all Bitcoin transactions are transparent. For Bulwark, a nefarious actor would need to control 50% of the operating masternodes to have less than 0.5% chance of de-anonymizing a single transaction that was mixed with 8 rounds of Obfuscation [@PrivateSend]. This important feature provides a high-level of anonymity for BWK users that elect to obfuscate their transactions.

## SwiftTX

SwiftTX provides masternodes with locking and consensus authority for transactions. When a transaction is submitted to the network, a group of masternodes will validate the transaction. If those masternodes reach consensus on the transaction’s validity it will be locked for later introduction into the blockchain, greatly increasing transaction speed compared to conventional systems (like Bitcoin’s 10 minute block times with multiple confirmations). SwiftTX makes it possible for multiple transactions to take place before a block on the network is mined with the same inputs. This system is based on Dash's InstantSend. [@InstantSend].

## Sporks

The Bulwark network employs the multi-phased fork mechanism known as “sporking”. This will enable the BWK network to implement new features while minimizing the chances of an unintended network fork during rollout. Spork changes are deployable via the network and can be turned on and off as necessary without requiring node software updates [@Sporks]. This feature is extremely useful and allows the network to react quickly to security vulnerabilities.

## TOR & IPV6 Masternodes

Bulwark allows the user to run their full node or masternode from either an onion address or an IPV6 address. We have been working to add full TOR nodes to both strengthen the TOR network itself, and the Bulwark user experience operating in TOR only mode. A unique feature of TOR masternode support is being able to operate your masternode as a TOR hidden service. TOR nodes enable users with stable internet connections to operate masternodes out of their home network without the privacy implications of revealing their location or the dangers of exposing their home network to the potential for attack or compromise.

## Community Importance and the Governance System

The Bulwark community is the most important factor behind the long-term success of the project, and their ability to meaningfully influence the future of the coin is paramount. As such, at the end of our first year, at block 345,601, we intend to activate budget superblocks on the network. These superblocks, paid monthly, will enable the community to exert meaningful control over all aspects of Bulwark's development, brand presence, and community affairs. Delaying the activation of this system will give us time to develop the underlying framework necessary for a positive user experience, and maximize block rewards available to miners and masternodes. 

We will utilize a multi-phase process for creating and submitting proposals. Each step will need to be fully completed. Failure to complete the steps outlined will likely result in a proposal not being activated. A basic outline of these steps are as follows:

- Start in our Discord chat, and talk with some of the seasoned users. Gauge interest and if the response is positive, move to the next phase.
- Utilize multiple social media platforms to discuss and get feedback. Remember that Bulwark has a diverse userbase and differing levels of governance participation, reaching a portion of the userbase will often require some footwork. Take note of these discussions and be able to cite them in the formal pre-proposal. The more citations provided, the better.
- Be open to suggestions from the community and developers. Be flexible and willing to incorporate external ideas and suggestions in your proposal.
- Create a formal pre-proposal on the Governance->Pre-Proposal section of our website. Provide citations for all discussions that occurred from the previous step. Treat your pre-proposal as if it is what will be submitted to the blockchain for voting.
- Upon completion of these steps, you will submit your proposal to the blockchain. Be prepared for two fees, one at the time of submission and a ballot fee paid to the developer that activates your proposal on the blockchain. The submission fee is non-refundable, and the balloting fee will only be paid upon approval and activation of your proposal.
- Everyone is free to adjust their proposal to include the reimbursement cost of these two fees. Please make sure in your formal proposal you state that you are adding reimbursement to the stipend requested.
- Be sure to get back in touch with everyone you spoke with so your idea will be voted on. For a proposal to be paid out, 10% of the eligible masternodes must vote 'yes' on your proposal. This process of getting a 10% consensus can be much harder than it sounds, so be diligent, informative, and respectful in procuring the votes necessary for your proposal to be paid.

## SeeSaw PoS/Masternode Rewards
We have decided to utilize the SeeSaw reward system popularized by PIVX [@PIVX]. The SeeSaw reward system begins with a 9:1 block reward ratio (favoring masternodes), and smoothly adjusts the ratio of reward between staking and node operators until around 41.5% of coins in circulation are locked into masternodes, at which time staking rewards reach a slight advantage over masternode rewards on a coin-by-coin basis. The reason we have the SeeSaw slightly favoring staking rewards is because we want to avoid the problems - like significant price volatility and low liquidity - that impact coins with very-high percentages of their circulating supply locked in nodes. This strategy will mitigate user frustration over access to coin supply and maintains the relevance of our robust network. With one of our goals being a well-supported platform for anonymous commerce, transactability is of the utmost importance to those accepting Bulwark and those holding Bulwark.
![Figure 3. SeeSaw rewards \label{ref_c_figure}](source/figures/fig.png){ width=100% }

\newpage

## Open Source Stance
The Bulwark team is a strong proponent of open source development. All works, present and future, will always be made open source to the community. Cryptocurrency is a massively growing technological endeavor and we strongly believe that proprietary and closed source developments hinder advancement and innovation. Scripts, toolsets, and codebases for all Bulwark projects are free for others to use under the appropriate open source license. 
