path\_na\_analysis
================

Understand the pathology reports yet to be completed
----------------------------------------------------

    ## Parsed with column specification:
    ## cols(
    ##   medrioid = col_integer(),
    ##   batch = col_character(),
    ##   siteid = col_character(),
    ##   cancer_type = col_character(),
    ##   formname = col_character(),
    ##   formstatusc = col_character(),
    ##   complete = col_character(),
    ##   incomplete_com = col_character(),
    ##   state = col_character(),
    ##   zip_code = col_integer(),
    ##   clean_zip = col_character(),
    ##   latitude = col_double(),
    ##   longitude = col_double()
    ## )

    ## [1] 3619

``` r
sum_na_cancer_type
```

    ## # A tibble: 156 x 7
    ##    total n_by_cancer_type cancer_type        variable n_missing percent
    ##    <int>            <int> <chr>              <chr>        <int>   <dbl>
    ##  1  5574             1685 breast             complete      1053    62.5
    ##  2  5574              694 prostate           complete       553    79.7
    ##  3  5574              333 uterine            complete       290    87.1
    ##  4  5574              350 colorectal         complete       233    66.6
    ##  5  5574              252 other,lymphoma,NA  complete       205    81.3
    ##  6  5574              606 lung               complete       193    31.8
    ##  7  5574              163 ovarian            complete       121    74.2
    ##  8  5574              175 renal              complete       119    68.0
    ##  9  5574              137 other,head/neck,NA complete        96    70.1
    ## 10  5574              127 esophageal         complete        92    72.4
    ## # ... with 146 more rows, and 1 more variable: n_missing_cum <int>

``` r
sum_na_crf
```

    ## # A tibble: 22 x 8
    ##    total n_by_path_form formname  variable n_missing percent n_missing_cum
    ##    <int>          <int> <chr>     <chr>        <int>   <dbl>         <int>
    ##  1  5574           1697 patholog… complete      1061    62.5          1061
    ##  2  5574            696 patholog… complete       555    79.7          1616
    ##  3  5574            339 patholog… complete       295    87.0          1911
    ##  4  5574            365 patholog… complete       244    66.8          2155
    ##  5  5574            257 patholog… complete       208    80.9          2363
    ##  6  5574            622 patholog… complete       200    32.2          2563
    ##  7  5574            206 patholog… complete       165    80.1          2728
    ##  8  5574            168 patholog… complete       126    75.0          2854
    ##  9  5574            180 patholog… complete       122    67.8          2976
    ## 10  5574            144 patholog… complete       102    70.8          3078
    ## # ... with 12 more rows, and 1 more variable: crf_f <fct>

``` r
#pander::pandoc.table(sum_na_crf)
p0
```

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-1-1.png)

``` r
p1
```

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-1-2.png)

    ## [1] 3619

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

    ## Warning: Removed 2 rows containing missing values (geom_point).

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-5-1.png)
