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

    ## 
    ## ---------------------------------------------------------------
    ##          cancer_type            variable   n_missing   percent 
    ## ------------------------------ ---------- ----------- ---------
    ##            Breast,              complete      150       19.18  
    ## 
    ##           Prostate,             complete      120       45.98  
    ## 
    ##             Lung,               complete      55        12.56  
    ## 
    ##          Colorectal,            complete      36        23.53  
    ## 
    ##            Uterine,             complete      36        45.57  
    ## 
    ##          Esophageal,            complete      19        35.19  
    ## 
    ##             Renal,              complete      12        17.65  
    ## 
    ##           Pancreas,             complete       9        14.06  
    ## 
    ##           Melanoma,             complete       8        18.18  
    ## 
    ##            Ovarian,             complete       8         16    
    ## 
    ##        Ovarian,Uterine,         complete       2         100   
    ## 
    ##             Other,              complete       1       0.4202  
    ## 
    ##  Melanoma,Other,squamous cell   complete       1         100   
    ##       carcinoma in situ                                        
    ## 
    ##          Lung,Other,            complete       1        11.11  
    ## 
    ##         Lung,Pancreas,          complete       1         50    
    ## 
    ##       Melanoma,Other,BCC        complete       1         100   
    ## 
    ##         Breast,Other,           complete       1         100   
    ## 
    ##        Prostate,Renal,          complete       1         100   
    ## 
    ##     Ovarian,Other,parietal      complete       1         100   
    ##           peritoneum                                           
    ## 
    ##   Melanoma,Other,Basal Cell     complete       1         100   
    ##           Carcinoma                                            
    ## ---------------------------------------------------------------

![](path_na_analysis_files/figure-markdown_github/tfl-1.png)

    ## [1] 464

![](path_na_analysis_files/figure-markdown_github/tfl-2.png)

    ## 
    ## Attaching package: 'maps'

    ## The following object is masked from 'package:purrr':
    ## 
    ##     map

![](path_na_analysis_files/figure-markdown_github/unnamed-chunk-1-1.png)

    ## Saving 7 x 5 in image
