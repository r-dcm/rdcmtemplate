# Tables and Figures

## Tables

Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus
ex sapien vitae pellentesque sem placerat. In id cursus mi pretium
tellus duis convallis. Tempus leo eu aenean sed diam urna tempor.
Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis
massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper
vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra
inceptos himenaeos.

``` r
library(kableExtra)

head(penguins) |>
  kbl(
    caption = "Here is a table caption"
  )
```

| species | island    | bill_len | bill_dep | flipper_len | body_mass | sex    | year |
|:--------|:----------|---------:|---------:|------------:|----------:|:-------|-----:|
| Adelie  | Torgersen |     39.1 |     18.7 |         181 |      3750 | male   | 2007 |
| Adelie  | Torgersen |     39.5 |     17.4 |         186 |      3800 | female | 2007 |
| Adelie  | Torgersen |     40.3 |     18.0 |         195 |      3250 | female | 2007 |
| Adelie  | Torgersen |       NA |       NA |          NA |        NA | NA     | 2007 |
| Adelie  | Torgersen |     36.7 |     19.3 |         193 |      3450 | female | 2007 |
| Adelie  | Torgersen |     39.3 |     20.6 |         190 |      3650 | male   | 2007 |

Here is a table caption

Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus
ex sapien vitae pellentesque sem placerat. In id cursus mi pretium
tellus duis convallis. Tempus leo eu aenean sed diam urna tempor.
Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis
massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper
vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra
inceptos himenaeos.

## Figures

Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus
ex sapien vitae pellentesque sem placerat. In id cursus mi pretium
tellus duis convallis. Tempus leo eu aenean sed diam urna tempor.
Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis
massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper
vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra
inceptos himenaeos.

``` r
library(ggplot2)

ggplot(penguins, aes(x = flipper_len, y = bill_len)) +
  geom_point(aes(shape = species, color = species)) +
  geom_smooth(method = "lm", se = FALSE, aes(color = species))
```

![Here is a figure
caption](tables-figures_files/figure-html/penguin-figure-1.png)

Here is a figure caption

Lorem ipsum dolor sit amet consectetur adipiscing elit. Quisque faucibus
ex sapien vitae pellentesque sem placerat. In id cursus mi pretium
tellus duis convallis. Tempus leo eu aenean sed diam urna tempor.
Pulvinar vivamus fringilla lacus nec metus bibendum egestas. Iaculis
massa nisl malesuada lacinia integer nunc posuere. Ut hendrerit semper
vel class aptent taciti sociosqu. Ad litora torquent per conubia nostra
inceptos himenaeos.
