
<!-- README.md is generated from README.Rmd. Please edit that file -->

# mitocarta

<!-- badges: start -->

<!-- badges: end -->

This package contains the updated [`mitocarta` 3.0 dataset](https://www.broadinstitute.org/mitocarta/mitocarta30-inventory-mammalian-mitochondrial-proteins-and-pathways). This package
also contains some utility functions for simple analyses.

It was forked from and inspired by https://github.com/matthewhirschey/mitocarta

## Installation

``` r
install.packages("mitocarta")
```

So in the meantime, use the development version from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("dsanmiguel/mitocarta")
```

## Example

This is how to take a `glimpse` into the mitocarta dataset:

``` r
library(mitocarta)
glimpse(mitocarta)
#> Observations: 19,244
#> Variables: 43
#> $ training_dataset                          <chr> "Tnon_mito", "Tnon_mit…
#> $ human_gene_id                             <dbl> 1, 2, 9, 10, 12, 13, 1…
#> $ mouse_ortholog_gene_id                    <dbl> 117586, 232345, 17961,…
#> $ symbol                                    <chr> "A1BG", "A2M", "NAT1",…
#> $ synonyms                                  <chr> "A1B|ABG|GAB|HYST2477|…
#> $ description                               <chr> "alpha-1-B glycoprotei…
#> $ ensembl_gene_id                           <chr> "ENSG00000121410", "EN…
#> $ protein_length                            <dbl> 495, 1474, 352, 290, 4…
#> $ target_p_score                            <dbl> NA, NA, NA, NA, NA, NA…
#> $ mito_domain_score                         <chr> NA, "NonMitoDomain", "…
#> $ coexpression_gnf_n50_score                <dbl> NA, 0, 4, NA, 1, 7, 3,…
#> $ pgc_induction_score                       <dbl> NA, NA, -0.28, NA, NA,…
#> $ yeast_mito_homolog_score                  <chr> "NoMitoHomolog", "NoMi…
#> $ rickettsia_homolog_score                  <chr> "NoHomolog", "NoHomolo…
#> $ msms_score                                <chr> "50-75ambig", "50-75am…
#> $ mcarta2_score                             <dbl> -1.4533, -4.0790, -10.…
#> $ mcarta2_fdr                               <dbl> 0.459, 0.679, 0.883, 0…
#> $ mcarta2_list                              <dbl> 0, 0, 0, 0, 0, 0, 0, 0…
#> $ mcarta2_evidence                          <chr> NA, NA, NA, NA, NA, NA…
#> $ hg19_chromosome                           <chr> "chr19", "chr12", "chr…
#> $ hg19_start                                <dbl> 58858171, 9220303, 180…
#> $ hg19_stop                                 <dbl> 58864865, 9268558, 180…
#> $ msms_num_tissues                          <dbl> 1, 1, NA, NA, NA, 1, N…
#> $ msms_num_peptides_unique                  <dbl> 24, 67, NA, NA, NA, 9,…
#> $ msms_num_spectra                          <dbl> 153, 326, NA, NA, NA, …
#> $ msms_total_intensity                      <dbl> 8.11e+09, 6.93e+09, NA…
#> $ msms_percent_coverage                     <dbl> 60, 55, NA, NA, NA, 33…
#> $ tissues                                   <chr> "placenta", "placenta"…
#> $ cerebrum_total_peak_intensity_log10       <dbl> NA, NA, NA, NA, NA, NA…
#> $ cerebellum_total_peak_intensity_log10     <dbl> NA, NA, NA, NA, NA, NA…
#> $ brainstem_total_peak_intensity_log10      <dbl> NA, NA, NA, NA, NA, NA…
#> $ spinalcord_total_peak_intensity_log10     <dbl> NA, NA, NA, NA, NA, NA…
#> $ kidney_total_peak_intensity_log10         <dbl> NA, NA, NA, NA, NA, NA…
#> $ liver_total_peak_intensity_log10          <dbl> NA, NA, NA, NA, NA, 8.…
#> $ heart_total_peak_intensity_log10          <dbl> NA, NA, NA, NA, NA, NA…
#> $ skeletalmuscle_total_peak_intensity_log10 <dbl> NA, NA, NA, NA, NA, NA…
#> $ adipose_total_peak_intensity_log10        <dbl> NA, NA, NA, NA, NA, NA…
#> $ smallintestine_total_peak_intensity_log10 <dbl> NA, NA, NA, NA, NA, NA…
#> $ largeintestine_total_peak_intensity_log10 <dbl> NA, NA, NA, NA, NA, NA…
#> $ stomach_total_peak_intensity_log10        <dbl> NA, NA, NA, NA, NA, NA…
#> $ placenta_total_peak_intensity_log10       <dbl> 9.9, 9.8, NA, NA, NA, …
#> $ testis_total_peak_intensity_log10         <dbl> NA, NA, NA, NA, NA, NA…
#> $ hpa_primary_subcellular_localization_2015 <chr> NA, "Nucleus (APE, Unc…
```
