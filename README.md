
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Dog and owner characteristics predict training success

This repository provides the reproducible research materials for our
project that investigates the characteristics of dogs, owners, and their
interaction that predict dog training success. This includes the
following:

-   Data
-   R script for data analysis
-   R Markdown file for the manuscript
-   R Markdown file for supplementary materials

# Citation

If you use any of these materials, please cite:

Stevens, J. R., Wolff, L. M., Bosworth, M., & Morstad, J. (2021). Dog
and owner characteristics predict training success. *Animal Cognition*.
<https://doi.org/10.1007/s10071-020-01458-0>.

# Summary

We collected survey, behavioral, and hormonal data from 99 dog/owner
pairs from the Prairie Skies Dog Training Canine Good Citizen classes
from Jan 2018 − Oct 2019. We generated three data files: one for the
primary survey, behavioral, and hormonal measures for each dog/owner
pair, one with the survey item responses for calculating internal
consistency reliability, and one with the behavioral data scores for
calculating inter-rater reliability. For the primary analysis data file,
each row represents all of a single participant’s responses. For the
survey item data file, each row represents a participant’s responses to
a particular survey. For the behavioral task data, each row represents a
dog’s responses for a single session.

# License

All materials presented here are released under the Creative Commons
Attribution 4.0 International Public License (CC BY 4.0). You are free
to:

-   Share — copy and redistribute the material in any medium or format
-   Adapt — remix, transform, and build upon the material for any
    purpose, even commercially. Under the following terms:
-   Attribution — You must give appropriate credit, provide a link to
    the license, and indicate if changes were made. You may do so in any
    reasonable manner, but not in any way that suggests the licensor
    endorses you or your use.

No additional restrictions — You may not apply legal terms or
technological measures that legally restrict others from doing anything
the license permits.

# Files

## Data files

`stevens_etal_data1.csv` (primary behavioral, cognitive, and cortisol
data set)

-   id - Dog id number
-   date - Date owner completed survey
-   class - Obedience training class
-   dog\_age - Age of dog in years
-   dog\_sex - Sex of dog
-   dog\_neutered - Neuter status (neutered/spayed = Yes, intact = No)
-   owner\_gender - Gender of owner
-   time\_train\_dog\_weekly\_num - Number of hours per week spent
    training
-   dog\_behavior\_bennett\_disobedient\_score - Disobedience subscale
    of Bennett & Rohlf behavior scale
-   dog\_behavior\_bennett\_aggressive\_score - Aggression subscale of
    Bennett & Rohlf behavior scale
-   dog\_behavior\_bennett\_nervous\_score - Nervousness subscale of
    Bennett & Rohlf behavior scale
-   dog\_behavior\_bennett\_destructive\_score - Destructiveness
    subscale of Bennett & Rohlf behavior scale
-   dog\_behavior\_bennett\_excitable\_score - Excitability subscale of
    Bennett & Rohlf behavior scale
-   dog\_behavior\_bennett\_overall\_score - Overall score of Bennett &
    Rohlf behavior scale
-   dog\_problematic\_behaviors\_hiby\_score - Problematic behavior
    score of Hiby et al.
-   dog\_obedience\_hiby\_score - Obedience score of Hiby et al.
-   dias\_behavioral\_regulation\_score - Behavioral regulation subscale
    of DIAS from Wright et al.
-   dias\_aggression\_score - Aggression subscale of DIAS from Wright et
    al.
-   dias\_responsiveness\_score - Responsiveness subscale of DIAS from
    Wright et al.
-   dias\_overall\_score - Overall score for DIAS from Wright et al.
-   mdors\_score - Monash Dog Owner Relationship Scale score
-   personality\_extraversion\_score - Extraversion score from brief
    Big-Five personality scale Gosling et al.
-   personality\_agreeableness\_score - Agreeableness score from brief
    Big-Five personality scale Gosling et al.
-   personality\_conscientiousness\_score - Conscientiousness score from
    brief Big-Five personality scale Gosling et al.
-   personality\_stability\_score - Stability score from brief Big-Five
    personality scale Gosling et al.
-   personality\_openness\_score - Openness score from brief Big-Five
    personality scale Gosling et al.
-   lotr\_score - Life Orientation Test Revised score from Scheier et
    al.
-   pss\_score - Perceived Stress Scale score from Cohen et al.
-   crt\_score - Cognitive Reflection Task score from Frederick
-   numeracy\_score - Berlin Numeracy Test score from Cokely et al.
-   latency\_sit\_mean - Mean latency between command and sit behavior
    (in seconds)
-   latency\_down\_mean - Mean latency between command and down behavior
    (in seconds)
-   cort1 - Cortisol levels before first class meeting (in ug/dL)
-   cort2 - Cortisol levels after first class meeting (in ug/dL)
-   cort3 - Cortisol levels before last class meeting (in ug/dL)
-   cort4 - Cortisol levels after last class meeting (in ug/dL)
-   cgc\_test - Success in completing Canine Good Citizen test
    (Pass/Fail)

`stevens_etal_data2.csv` (item-specific data for calculating internal
consistency reliability)

-   survey - name of survey
-   item\_1 - item\_13 - individual items (surveys differ on number of
    items, so NAs represent no items)

`stevens_etal_data3.csv` (behavioral (sit/down) data for calculating
inter-rater reliability)

-   block - Replication block (1, 2, or 3)
-   coder - Coder ID
-   date - Date of behavioral data collection
-   id - Dog ID
-   latency\_sit - Latency between command and sit behavior (in seconds)
-   latency\_down - Latency between command and down behavior (in
    seconds)

## R code

`stevens_etal_2021_rcode.R` - code for running computations and
generating figures

## R Markdown documents

`stevens_etal_2021.Rmd` - R Markdown document with R code embedded for
main manuscript `stevens_etal_2021_SM.Rmd` - R Markdown document with R
code embedded for supplementary materials

# Installation

To reproduce these results, first clone the repository. Then, open
`stevens_etal_2021_rcode.R` and ensure that all packages mentioned at
the top of the script are installed. Once all packages are installed,
run the script in R using `source("stevens_etal_2021_rcode.R")`.

Once the script runs without errors, you can compile the R Markdown
document `stevens_etal_2021.Rmd.` Open this file in RStudio and ensure
that you have packages {knitr} and {rmarkdown} installed. Once
installed, use knitr to compile the document (control-shift-k). Use the
same process to compile `stevens_etal_2021_SM.Rmd`.