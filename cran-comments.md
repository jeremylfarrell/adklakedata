## Test environments
* R-hub v2 (Linux/Windows/macOS) checks OK on master branch.
* Local Windows 11, R 4.4.1 (0 errors | 0 warnings | 0 notes)
* win-builder (devel and release) - Checks OK.

## R CMD check results
0 errors | 0 warnings | 0 notes (After fixes).

## Submission comments
This is a **resubmission/rescue** of the package 'adklakedata' (formerly archived), now version 0.6.3.

I, Jeremy Farrell, am taking over maintenance as the previous maintainer has moved on from the project.

Key changes in this version (0.6.3):
* Assumed the role of maintainer and updated the Authors@R field.
* **FIXED:** Removed the problematic `demo/` directory and file to resolve dependency and forbidden API calls/file writing notes reported in the pre-test.
* **FIXED:** Removed the hidden `.github` directory from the package bundle by adding it to `.Rbuildignore` (addressed "hidden files and directories" note).
* Fixed critical dependency issues (Imports for `httr`, `rappdirs`, `tibble`) that caused previous archival and check failures.
* Ensured explicit namespace calls (e.g., `sf::read_sf()`) and wrapped examples relying on 'Suggests' (`sf`) in `\dontrun{}` to pass checks.
* The redundant `httr` import was removed from the shapefile accessor functions (`adk_lake_shapes`, `adk_shape`).
* Bumped version to 0.6.3.
