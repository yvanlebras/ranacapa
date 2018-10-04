## Step 1- Explore sequencing depth

An important point to keep in mind when interpreting results from eDNA metabarcoding studies is that our estimate of species diversity in a community can depend a lot on how "deeply" we sequence the DNA extracted. If we extract DNA from a given sample and sequence 100 randomly selected DNA fragments from it, we might estimate that there are only 5 species in the community- but if we were to sequence 100000 randomly DNA fragments, we might find out that there is actually DNA from 50 species in the same sample.

In eDNA sequencing, such variation in how deeply a given sample is sequenced can happen for a variety for reasons- PCR amplification may have been more successful in one sample than an other, the sequencing machine may have worked less efficiently on certain samples than others, etc. This makes comparison between samples difficult- as in the example above, you might find more species in one sample than another simply because it has been sequenced more deeply than others.

One approach in this scenario is to 'rarefy' your samples by subsampling a defined number of sequences from each sample. You can choose a specific depth to rarefy to, or can choose to rarefy down to the minimum number of reads sequenced in any single sample (e.g. if you have 50000 reads in the least well-sequenced sample, all samples will be subsampled down to 50000 reads. Replicating this subsampling many times allows us to have better estimates of the diversity in the rarefied samples.

We note that there has been considerable discussion regarding the best way of dealing with unequal sampling. eDNA is an evolving field, and the scientific community has not reached consensus on this topic. We refer users to  [Weiss et al. 2017, Microbiome](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-017-0237-y), and to [McMurdie & Holmes 2014, PLoS Comp. Biol](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003531). We have not yet implemented alternative options to rarefying in `ranacapa`, but you are welcome to continue without rarefying the samples by selecting the "none" option on the left. 


