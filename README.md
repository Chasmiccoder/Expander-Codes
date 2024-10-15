# Expander-Codes
Implementation of expander codes and their erasure decoding in Julia

### Flow

1. Start with an ($n,d,\lambda$)-Ramanujan Graph (Say $g$)
2. Find the double-cover of $g$ (Say $g'$)
3. Find the edge-incidence graph of $g'$ (Say $G$)
4. Choose a code $C_0$ with block length $d$
5. The set $T = (G, C_0)$ forms our expander code with expander graph $G$ and inner code $C_0$
6. Pick a codeword in $T$. For now pick $0$
7. Pass the codeword through the erasure channel
8. Decode this erasure using the $UniqueDecode$ algorithm
