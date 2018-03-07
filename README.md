# GENIE3-on-DREAM4

## Introduction
GENIE3 (Huynh-Thu et al.) uses random forest variable importance to recover gene regulatory networks, and was the best performer in the DREAM4 *In Silico Multifactorial* challenge. This project does the following:

**(1)** Implements the GENIE3 gene regulatory network algorithm using base R functions

**(2)** Analyses data from the DREAM4 In Silico Size 100 Multifactorial subchallenge

**(3)** Compares performance to that of the original GENIE3 algorithm which was the best performer in this subchallenge

**GENIE3 Publication link:** http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0012776

**DREAM4 Data link:** http://dreamchallenges.org/project/dream4-in-silico-network-challenge/

*In Progress* **(4)** Improving algorithm by accounting for indirect associations that may lead to spurious detections

## Running the Algorithm

R scripts are provided for both the original and new implementation of GENIE3. Just make sure that you change the "directory" object to match the directory where the data files are located. After that the script should run and save results to the same directory.

**genie3_original.R** Original implementation, directly from the creator

**genie3_spurgeon.R** New implementation

## Performance Assessment

I compare the original and Spurgeon implementations of Genie3 using precision vs recall (PR) curves. PR curves and the area underneath curve (AUC) are calculated for all 5 datasets - these results are plotted and saved in png files with names beginning with "Performance_PrecisionRecall_DREAM4_Dataset". The Spurgeon implementation has greater AUC in 4/5 datasets.
