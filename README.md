# Mixing of the Aldous-Fill crossover chain via random switching networks

Yitzchak Shmalo

Paper: [paper/main.pdf](paper/main.pdf) (LaTeX source in `paper/main.tex`). Archived at Zenodo,
[doi:10.5281/zenodo.24257131](https://doi.org/10.5281/zenodo.24257131).

Aldous and Fill (Reversible Markov Chains and Random Walks on Graphs, Section 12.1.11) consider a chain on K binary
words of length L: at each step the words are paired at random, and within each pair every letter position is
exchanged with probability 1/2. They prove that it mixes in O(K log L) steps and ask for O(log K · log L)
(Open Problem 12.5).

The paper proves:

1. The chain mixes in O(log K + log L) steps, uniformly in the column sums. Given the pairings, the letter positions
   evolve independently, each pushed through the same random switching network; Czumaj (STOC 2015) proved that almost
   every such network of logarithmic depth shuffles every 0-1 vector almost uniformly, and blocks of steps are combined
   with the Dobrushin contraction coefficient.
2. Lower bounds: log2 min(K, L) - 3 for all K and L, and, for fixed K >= 4, a constant times log L. So the bound has the
   right order for fixed K as L grows and for K <= L <= K^A.

Both results hold for the chain as Aldous and Fill define it and for the variant in which the new words keep the
labels of the old ones.

## Files

- `paper/main.tex`, `paper/main.pdf`: the paper.
- `SHA256SUMS.txt`: checksums of the paper files.
