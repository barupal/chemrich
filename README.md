# ChemRICH

Chemical Similarity Enrichment analysis of metabolomics datasets. 

Assuming a statistical independence among metabolites is incorrect for metabolomics datasets because of the existence of 1) metabolic pathways 2) same origin 3) genetic regulation of metabolism and 4) chemical similarity among metabolites. Therefore, any p-value adjustment approach to correct for the multiple hypothesis testing of the raw entity level p-values causes false negative results, leading to missed biological insights from metabolomics datasets. 

Classical pathway analyses provide a narrowed intepretation for metabolomics datasets for two major reasons - 1) biochemical databases are incomplete for metabolomics so we are biased towards only a handful for selected compounds 2) a hypergeometric test relies on a background database which does not exist for metabolomics datasets.  

Alternatively, we can define data-driven and chemistry-driven compounds sets. Those sets can be used by a background database independent test such as the Kolmogorov–Smirnov test [KS-Test](https://en.wikipedia.org/wiki/Kolmogorov%E2%80%93Smirnov_test) to obtain the set-level significance. There could be several other ways to define chemical sets including chemical ontologies such as MeSH. 

ChemRICH is an approach that defines chemical classes for metabolites and then runs a KS test to obtain the set-level p-values. It uses chemical similarity against the MeSH database to obtain chemical classes, but users can also provide their own chemical classes to run the KS-test. Underlying hypothesis is that "P-values under the null hypothesis are uniformly distributed between 0 and 1" (  
 https://www.mv.helsinki.fi/home/mjxpirin/GWAS_course/material/GWAS2.html ) 

A new version of ChemRICH has been developed in R (version 4.0).  

## Visit the new ChemRICH site at [ChemRICH.idsl.me](http://chemrich.idsl.me) (updated August 2020)

ChemRICH is maintained and developed by the Integrated Data Science Laboratory for Metabolomics and Exposomics (IDSL.ME)

