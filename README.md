# HarmonicCentralityLinkRecommendation
Harmonic centrality-aware link recommendation on unweighted graphs is a submodular function

## Introduction

Centrality-aware link recommendation is first formally described in [1].
That is, given a vertex v in a graph, we are allowed to recommend new k edges to v (or add new k edges between v and one vertex) for maximization of v's centrality.
How do we find out such k edges in a graph?

There are many centrality definitions for a node.
Under the common closeness centrality, [1] proves the centrality-aware link recommendation is NP-hard, and also provides a greedy algorithm whose expected approximation ratio is (1 - 1 / e).
The approximation ratio is guaranteed by proving the problem as a submodular function.

Harmonic centrality is another centrality definition, whose formulation is based on the shortest path distance between two nodes, like closeness centrality.
In 2014, I proved that the link recommendation greedy algorithm under harmonic centrality is also a submodular function.
If using harmonic centrality instead of closeness centrality in the greedy algorithm, then we are guarateed the same (1 - 1 / e) approximiation ratio.

Maybe I am not the first one to prove the property of harmonic centrality, but my proof is uploaded here for future references.

## References

[1] Parotsidis, Nikos, Evaggelia Pitoura, and Panayiotis Tsaparas. "Centrality-aware link recommendations." Proceedings of the Ninth ACM International Conference on Web Search and Data Mining. ACM, 2016.
