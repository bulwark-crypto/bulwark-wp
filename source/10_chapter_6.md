# NIST5 Hashing

## Why NIST5

Popularized by TalkCoin in 2014, the NIST5 hashing algorithm has seen modest mainstream usage. NIST5 can be mined on a wide array of consumer-grade hardware including CPUs, as well as AMD and Nvidia GPUs. NIST5 is not as ASIC resistant as some other memory hard algorithms, but we believe the trade-off is acceptable to improve system stability and reduce power consumption relative to those memory hard algorithms.

## The Five Finalists (NIST SHA-3 Competition)

The five hashing algorithms that make up NIST5 are the finalists from the NIST Hashing Competition [@NIST]. They are (in the order that blocks are hashed):

**Blake** [@Blake], **Grøstl** [@Grostl], **JH** [@JH], **Keccak** [@Keccak], and **Skein** [@Skein]

\newpage

## The new SHA-3 Standard

Keccak eventually passed the final round to be named the new SHA-3 hashing function, while the other four algorithms (despite being considered cryptographically secure) lost a few points from the judges for some minor technicalities. We believe the combination of the new SHA-3 standard along with the other finalist choices provide a quick, secure, and established hashing algorithm.

## Mining Software Available

At the time of writing, there are several options for miners

-------------------------------------------------------------------
Name           Platform         Link
-------------- ---------------- -----------------------------------
SGMiner-5.0    OpenCL           \href{https://github.com/genesismining/sgminer-gm}{GitHub}

ccminer-2.2.2  CUDA             \href{https://github.com/tpruvot/ccminer}{GitHub}

cpuminer-opt   CPU              \href{https://github.com/tpruvot/cpuminer-multi}{GitHub}

-------------------------------------------------------------------
