## `batchLASSO` for more easily performing ROC and PRC analysis with the LASSO
--------------------------------------------------------

`batchLASSO` is a minimalistic `R` package for creating ROCs and 
PRCs when applying the LASSO on binary data with multiple responses and multiple covariates (exposures). 

`batchlasso` can be used to rank the response-exposure pairs from most to least 'interesting'. Simply using the resulting regression coefficients
would be unwise, since the size of the coefficients cannot be compared
from model to model. Instead, we use the tuning parameter, `lambda`.

Each response variable in the given `response` matrix is regressed
on all exposures in the matrix `exposure`. We determine for each
exposure what the highest value of `lambda` for which that variable is included for the first time in the regression model (i.e., its
regression coefficient is non-zero). These `lambda`-values can be
compared across models.

See for the details `?batchLASSO`. 

### Acknowledgements

We gratefully acknowledge the financial support from the innovation fund (“Innovationsfonds”) of the Federal Joint Committee in Germany (grant number: 01VSF16020).

### Contact

Louis Dijkstra\
Leibniz Institute for Prevention Research & Epidemiology  
E-mail: dijkstra (at) leibniz-bips.de