# PhyloSeqExtractTwo
# Language: R
# Input: TXT (keyword-value pairs)
# Output: PREFIX
# Tested with: PluMA 1.1, R 4.0.0
# Dependency: microbiome_1.12.0, phyloseq_1.34.0

Extract samples from two categories from PhyloSeq (McMurdie et al, 2013) input.

You may want to extract two categories if you are doing downstream differential analysis between those categories.

The input file is a parameters TXT file of tab-delimited keyword-value pairs:
OTU: Taxa abundances
TAX: Taxonomy
META: Metadata
FILTER1: Category 1
FILTER2: Category 2
column: Column name in metadata corresponding to category

Output abundance, taxonomy and metadata will be generated for the reduced set of samples, using the user-specified PREFIX.

