# README

    def switch_to_numbers(G, C):
        num_comm = len(C)
        a = []
        for c in range(num_comm):
            a.append([0])
        for i, node in enumerate(G.nodes()):
            for j in range(num_comm):
                if node in C[j]:
                    a[j].append(i)
        for c in range(num_comm):
            a[c] = a[c][1:]
        return a


The file dolphins.gml contains an undirected social network of frequent
associations between 62 dolphins in a community living off Doubtful Sound,
New Zealand, as compiled by Lusseau et al. (2003).  Please cite

  D. Lusseau, K. Schneider, O. J. Boisseau, P. Haase, E. Slooten, and
  S. M. Dawson, The bottlenose dolphin community of Doubtful Sound features
  a large proportion of long-lasting associations, Behavioral Ecology and
  Sociobiology 54, 396-405 (2003).

Additional information on the network can be found in

  D. Lusseau, The emergent properties of a dolphin social network,
  Proc. R. Soc. London B (suppl.) 270, S186-S188 (2003).

  D. Lusseau, Evidence for social role in a dolphin social network,
  Preprint q-bio/0607048 (http://arxiv.org/abs/q-bio.PE/0607048)
