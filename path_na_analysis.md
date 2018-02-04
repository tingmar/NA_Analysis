path\_na\_analysis
================

Understand the pathology reports yet to be completed
----------------------------------------------------

    ## Parsed with column specification:
    ## cols(
    ##   medrio_id = col_integer(),
    ##   batch = col_character(),
    ##   siteid = col_character(),
    ##   cancer_type = col_character(),
    ##   sex = col_character(),
    ##   age = col_integer(),
    ##   method_of_tissue_collection = col_character(),
    ##   date_of_clinical_procedure = col_character(),
    ##   complete = col_character(),
    ##   name_of_pathology_crf = col_character(),
    ##   state = col_character(),
    ##   zip_code = col_integer(),
    ##   clean_zip = col_character(),
    ##   latitude = col_double(),
    ##   longitude = col_double()
    ## )

    ## [1] "total"                 "name_of_pathology_crf" "variable"             
    ## [4] "n_missing"             "percent"               "n_missing_cum"

    ## [1] 464

``` r
sum_na_cancer_type
```

    ## # A tibble: 20 x 6
    ##    total cancer_type              variable n_missing percent n_missing_cum
    ##    <int> <chr>                    <chr>        <int>   <dbl>         <int>
    ##  1  2388 Breast,                  complete       150  19.2             150
    ##  2  2388 Prostate,                complete       120  46.0             270
    ##  3  2388 Lung,                    complete        55  12.6             325
    ##  4  2388 Colorectal,              complete        36  23.5             361
    ##  5  2388 Uterine,                 complete        36  45.6             397
    ##  6  2388 Esophageal,              complete        19  35.2             416
    ##  7  2388 Renal,                   complete        12  17.6             428
    ##  8  2388 Pancreas,                complete         9  14.1             437
    ##  9  2388 Melanoma,                complete         8  18.2             445
    ## 10  2388 Ovarian,                 complete         8  16.0             453
    ## 11  2388 Ovarian,Uterine,         complete         2 100               455
    ## 12  2388 Other,                   complete         1   0.420           456
    ## 13  2388 Melanoma,Other,squamous… complete         1 100               457
    ## 14  2388 Lung,Other,              complete         1  11.1             458
    ## 15  2388 Lung,Pancreas,           complete         1  50.0             459
    ## 16  2388 Melanoma,Other,BCC       complete         1 100               460
    ## 17  2388 Breast,Other,            complete         1 100               461
    ## 18  2388 Prostate,Renal,          complete         1 100               462
    ## 19  2388 Ovarian,Other,parietal … complete         1 100               463
    ## 20  2388 Melanoma,Other,Basal Ce… complete         1 100               464

``` r
sum_na_crf
```

    ## # A tibble: 12 x 7
    ##    total name_of_pathology… variable n_missing percent n_missing_cum crf_f
    ##    <int> <chr>              <chr>        <int>   <dbl>         <int> <fct>
    ##  1  2388 pbr                complete       151   19.2            151 pbr  
    ##  2  2388 ppr                complete       120   46.0            271 ppr  
    ##  3  2388 plu                complete        56   12.5            327 plu  
    ##  4  2388 put                complete        37   45.7            364 put  
    ##  5  2388 pco                complete        36   22.9            400 pco  
    ##  6  2388 pes                complete        19   35.2            419 pes  
    ##  7  2388 pre                complete        13   18.3            432 pre  
    ##  8  2388 pme                complete        11   22.9            443 pme  
    ##  9  2388 pov                complete        10   19.2            453 pov  
    ## 10  2388 ppa                complete         9   13.6            462 ppa  
    ## 11  2388 phn                complete         1    2.33           463 phn  
    ## 12  2388 pcc                complete         1    3.33           464 pcc

``` r
#pander::pandoc.table(sum_na_crf)
p1
```

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-1-1.png)

    ## [1] 464

``` r
p2
```

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-3-1.png)

    ## 
    ## Attaching package: 'maps'

    ## The following object is masked from 'package:purrr':
    ## 
    ##     map

``` r
usamap
```

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-5-1.png)
