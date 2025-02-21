# GFA: Graphical Fragment Assembly (GFA) Format Specification

We are developing the specification of the Graphical Fragment Assembly (GFA) format. Your contribution is welcome. Please open up issues or submit pull requests.

+ GFA 2.0 is at [GFA2.md](GFA2.md)
+ GFA 1.0 is at [GFA1.md](GFA1.md)
+ GFA 1.1 is at [GFA1.md#gfa-11](GFA1.md#gfa-11)
+ GFA 1.2 is at [GFA1.md#gfa-11](GFA1.md#j-jump-line-since-v12)

# Implementations

## GFA 2

+ [ABySS](https://github.com/bcgsc/abyss)
+ [Cuttlefish](https://github.com/COMBINE-lab/cuttlefish)
+ [dsh-bio](https://github.com/heuermh/dishevelled-bio)
+ [gfakluge](https://github.com/edawson/gfakluge)
+ [gfalint](https://github.com/sjackman/gfalint)
+ [GfaPy](https://github.com/ggonnella/gfapy)
+ [GfaViz](https://github.com/ggonnella/gfaviz)

## GFA 1

+ [ABySS](https://github.com/bcgsc/abyss)
+ [Assembly Cytoscape3 App](http://apps.cytoscape.org/apps/assembly)
+ [Bandage](https://rrwick.github.io/Bandage/)
+ [bcalm2](https://github.com/GATB/bcalm)
+ [bfgraph](https://github.com/pmelsted/bfgraph)
+ [Canu](https://github.com/marbl/canu)
+ [Cuttlefish](https://github.com/COMBINE-lab/cuttlefish)
+ [dsh-bio](https://github.com/heuermh/dishevelled-bio)
+ [fermi mag2gfa](https://github.com/lh3/mag2gfa)
+ [gfabase](https://github.com/mlin/gfabase)
+ [gfakluge](https://github.com/edawson/gfakluge)
+ [GfaPy](https://github.com/ggonnella/gfapy)
+ [GfaViz](https://github.com/ggonnella/gfaviz)
+ [jts/DALIGNER](https://github.com/jts/daligner)
+ [lh3/gfa1](https://github.com/lh3/gfa1)
+ [lh3/gfatools](https://github.com/lh3/gfatools)
+ [lmrodriguezr/gfa](https://github.com/lmrodriguezr/gfa)
+ [McCortex](https://github.com/mcveanlab/mccortex)
+ [miniasm](https://github.com/lh3/miniasm)
+ [RGFA](https://github.com/ggonnella/RGFA)
+ [SPAdes](http://cab.spbu.ru/software/spades/)
+ [TwoPaCo](https://github.com/medvedevgroup/TwoPaCo)
+ [Unicycler](https://github.com/rrwick/Unicycler)
+ [vg](https://github.com/ekg/vg)
+ [w2rap](https://github.com/bioinfologics/w2rap-contigger)

## GFA 1.1

+ [vg](https://github.com/ekg/vg)
+ [gbwt](https://github.com/jltsiren/gbwt)
+ [cactus pangenome pipeline](https://github.com/ComparativeGenomicsToolkit/cactus/blob/master/doc/pangenome.md)

## GFA 1.2

+ [gfastats](https://github.com/vgl-hub/gfastats)

# Resources

+ [Examples](https://github.com/sjackman/assembly-graph) of sequence overlap graphs (assembly graphs) in a variety of formats

# GFA 2.0: Graphical Fragment Assembly (GFA2) Format Specification 2.0

Jason Chin, Richard Durbin, and myself (Gene Myers) found ourselves together at a workshop
meeting in Dagstuhl Germany and hammered out an initial proposal for an assembly format.
We started with [GFA 1](GFA1.md) and proceeded to build a
more comprehensive design around it.  After extensive revision and discussion on Github with
the GFA group including Shaun Jackman, Heng Li, and Giorgio Gonnella, we arrived at
[GFA 2.0](GFA2.md). The standard is an evolving effort, and your contribution is welcome. Please open up issues or submit pull requests.

The basic reason for having a standard format is that we find that
in general, *different* development teams build assemblers, visualizers, and editors because
of the complexity and distinct nature of the three tasks.  While these tools should certainly
use tailored encodings internally for efficiency, the nexus between the three efforts
benefits from a standard encoding format that would make them all interoperable.

![Fig. 1](images/READ.Fig1.png)

# GFA 1.0

GFA 1 was first suggested in a [blog post](http://lh3.github.io/2014/07/19/a-proposal-of-the-grapical-fragment-assembly-format) by Heng Li (@lh3) and further developed in a [second post](http://lh3.github.io/2014/07/23/first-update-on-gfa).

# GFA 1.1

W-lines were suggeseted by Heng Li (@lh3) as an extension to GFA 1 for representing haplotype information in pangenome graphs.  

# GFA 1.2

J-lines were suggested by Sergey Nurk and Giulio Formenti as an extension to GFA 1.1 to represent jumps in graphs such as gaps in assembly scaffolds.