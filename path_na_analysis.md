Understand the pathology reports that need to be completed
----------------------------------------------------------

    source(here("R", "01_get_data.R"))

    ## Parsed with column specification:
    ## cols(
    ##   `Medrio ID` = col_integer(),
    ##   Batch = col_character(),
    ##   `Site ID` = col_character(),
    ##   `Cancer Type` = col_character(),
    ##   Sex = col_character(),
    ##   Age = col_integer(),
    ##   `Method of Tissue Collection` = col_character(),
    ##   `Date of Clinical Procedure` = col_character(),
    ##   `Complete?` = col_character(),
    ##   `Which data is incomplete?` = col_character(),
    ##   `Additional pathology report needed` = col_character(),
    ##   `Name of Pathology CRF` = col_character(),
    ##   `Path eCRF SDV'd` = col_character(),
    ##   `MD draft query text` = col_character(),
    ##   `Query Message` = col_character(),
    ##   `CDM Action` = col_character(),
    ##   `Site Response` = col_character(),
    ##   `Additional Notes` = col_character()
    ## )

    source(here("R", "02_na_summary.R"))

    ## Parsed with column specification:
    ## cols(
    ##   medrio_id = col_integer(),
    ##   batch = col_character(),
    ##   site_id = col_character(),
    ##   cancer_type = col_character(),
    ##   sex = col_character(),
    ##   age = col_integer(),
    ##   method_of_tissue_collection = col_character(),
    ##   date_of_clinical_procedure = col_character(),
    ##   complete = col_character(),
    ##   name_of_pathology_crf = col_character()
    ## )

R Markdown
----------

This is an R Markdown document. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document. You can embed an R code chunk like this:

    summary(cars)

    ##      speed           dist       
    ##  Min.   : 4.0   Min.   :  2.00  
    ##  1st Qu.:12.0   1st Qu.: 26.00  
    ##  Median :15.0   Median : 36.00  
    ##  Mean   :15.4   Mean   : 42.98  
    ##  3rd Qu.:19.0   3rd Qu.: 56.00  
    ##  Max.   :25.0   Max.   :120.00

Including Plots
---------------

You can also embed plots, for example:

![](path_na_analysis_files/figure-markdown_strict/pressure-1.png)

Note that the `echo = FALSE` parameter was added to the code chunk to
prevent printing of the R code that generated the plot.
