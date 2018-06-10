# Our Blockchain Parameters.

## Bulwark Specifications at a Glance

\ref{ref_a_table}

---------------------------------------------------------------------------
Specification 				Descriptor				
--------------      		------------------------------------------		
Ticker						BWK

Algorithm					NIST5

RPC Port 					52541

P2P Port 					52543

Block Spacing				90 Seconds

Difficulty Algorithm		Dark Gravity Wave v3.0

Block Size					1MB

Mined/Minted Maturity		67 Blocks (~100 Minutes)

Confirmation				6 Blocks (~9 Minutes)

Circulation (1 Year) 		14,505,720 BWK

Circulation (5 Years)		27,668,220 BWK

PoW Period					\textit{nHeight} $\leq$ 182,700

PoS Period					\textit{nHeight} $\geq$ 182,701

Protocol Support			IPV4, IPV6, TOR

PoS 						Blackcoin v3.0 PoS, PIVX SeeSaw rewards.

---------------------------------------------------------------------------

Table: At a glance specifications for Bulwark \label{ref_a_table}

\newpage

## SlowStart

Our fair start is provided with the following code snippet (Credit: ZCash).  
```C++

		int64_t nSlowSubsidy = 50 * COIN;

		if (nHeight < 960 / 2) {		// If block height less than 480,
           nSlowSubsidy /= 960;			// Set nSubsidy to .05208333
           nSlowSubsidy *= nHeight;		// Multiply present height by .05208333
        } else if (nHeight < 960 {		// ex: Block 200, BR will be 10.41666600
            nSlowSubsidy /= 960;		// Credits: ZCASH Team
            nSlowSubsidy *= nHeight;
```
The slow start period averages at 25 coins per block at block 960.

## Dark Gravity Wave 3.0

Dark Gravity Wave is employed by Bulwark from the start as a method of retargeting PoW difficulty. It uses a simple moving average that can respond to large nethash increases or drop-offs in just a few blocks. This alleviates the "stuck block effect" often caused by multipools and prevents one person adding a substantial amount of computing power from instantly solving more than a few blocks.
