
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rdcmtemplate <a href="https://rdcmtemplate.r-dcm.org"><img src="man/figures/logo.png" align="right" height="138" alt="Package hex logo" /></a>

<!-- badges: start -->

[![R-CMD-check](https://github.com/r-dcm/rdcmtemplate/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/r-dcm/rdcmtemplate/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

## Overview

rdcmtemplate provides a custom [pkgdown](https://pkgdown.r-lib.org)
template for r-dcm packages. Please don’t use it for your own package.

## Templates

For all sites, ensure that `DESCRIPTION` contains:

    Config/Needs/website: r-dcm/rdcmtemplate

### r-dcm

``` yaml
template:
  package: rdcmtemplate
  bootstrap: 5
  
  includes:
    after_body: >
      <script data-goatcounter="https://{YOUR DOMAIN}.goatcounter.com/count" async src="https://gc.zgo.at/count.js"></script>
      
development:
  mode: auto
```

Ping Jake on teams to get your site added to goat counter.

### Updating

If you’re updating from a previous pkgdown config, use the following
checklist to make sure everything is up to date:

``` md
* [ ] `usethis::use_pkgdown_github_pages()`
* [ ] Ensure Author includes University of Kansas as copyright holder and funder
* [ ] Update `DESCRIPTION` to include `Config/Needs/website: r-dcm/rdcmtemplate`
* [ ] Update `_pkgdown.yml` with appropriate template above.
* [ ] Ping Jake to add goat counter record
* [ ] Remove `strip_header: true`
* [ ] Remove algolia search, if used
* [ ] Eliminate superseded navbar customisation (`home: ~`, article re-ordering)
* [ ] Update `news` structure if needed
* [ ] Remove any author info for r-dcm folks (since now included in template)
```
