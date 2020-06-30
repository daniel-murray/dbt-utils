## dbt-utils v0.17.0
This release implements a new release process to better handle dbt-core version
changes (hence the version number change). It also implements a number of fixes
and features.

## Fixes
* Ensure surrogate key handles single arg (#242, fixes #241)
* Fix incorrect test behavior for the `unpivot` macro (#249 @avishalom)

## Features
* Throw a nice error when trying to use a macro that requires the information schema on an ephemeral model (#243)
* Add `unique_where` and `not_null_where` relationship tests (#250 @MartinGuindon)
* Add `distinct` argument to the `pivot` macro (#248 @DylanBaker)


## Quality of life
* Improve release process (#245)
* Replace BigQuery `__TABLES_SUMMARY__` with `INFORMATION_SCHEMA` (#247 @preston-hf)
