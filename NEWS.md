# serocalculator 1.1.0

* Renamed `llik()` function and replaced by `log_likelihood()`

* Renamed `fdev()` function and replaced by `f_dev()`

* Renamed `df.to.array()` function and replaced by `df_to_array()`

* Renamed `getAdditionalData()` function and replaced by `get_additional_data()`

* Removed `clean_pop_data()` function

* Remove `clean_pop_data()` dependency functions documentation examples

* Added `age`, `value`, `id` and `standardize` arguments to `load_pop_data()`

* Added the following methods to `pop_data` class:

  - `set_age()`
  - `set_value()`
  - `set_id()`
  - `get_age()`
  - `get_value()`
  - `get_id()`
  - `get_age_var()`
  - `get_value_var()`
  - `get_id_var()`
  
* Added additional warnings to `load_pop_data()`

* Added `scales::pseudo_log_trans()` to `autoplot.pop_data()` to avoid log 0

* Added `test-est.incidence-status.R` test to check output when `standardize` option is FALSE on `load_pop_data()`

* Replaced column name comparison on `check_pop_data()` to use attribute name on `pop_data` class

# serocalculator 1.0.1

* added `n_points` argument to `plot_curve_params_one_ab()`
* Added `type = "age-scatter"` option for `autoplot.pop_data()`

## serocalculator 1.0.0

* Moved underlying methods to `serocalculator` vignette

## serocalculator 0.5.0

* Spell-checking of function documentation and tutorial articles.

* Added functions and methods:

  - `load_pop_data()`
  - `check_pop_data()`
  - `summary.pop_data()`
  - `autoplot.pop_data()`
  - `load_curve_params()`

* Renamed `graph.decay.curves.by()` to `autoplot.curve_params()`

## serocalculator 0.4.0

* `plot()` methods have been renamed to `autoplot()`, matching general convention for `ggplot2`-based graphics.

* added visualization of curve parameters

* `sim.cs()` now has `format` argument to specify long or wide format for output.

### serocalculator 0.3.2

Fixed bug in passing `antigen_isos` from `est.incidence.by()` to `est.incidence()`.

### serocalculator 0.3.1

Rolled back required R version from 4.2 to 4.1

## serocalculator 0.3.0

* Fixed stability and documentation-clarity issues after initial tester feedback.

## serocalculator 0.2.0 (never formally incremented in DESCRIPTION)

* Added new vignettes.

## serocalculator 0.1.0

Forking from the seroincidence package and adding Teunis et al 2020 approach.
