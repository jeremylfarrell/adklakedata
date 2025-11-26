## Test environments
* R-hub windows-x86_64-devel (r-devel)
* Local Windows 11, R 4.4.1
* win-builder (devel and release)

## R CMD check results
0 errors | 0 warnings | 0 notes

## Submission comments
This is a **resubmission/rescue** of the package 'adklakedata' (formerly archived). 

I, Jeremy Farrell, am taking over maintenance as the previous maintainer has moved on from the project.

Key changes in this version (0.6.2):
* Assumed the role of maintainer and updated the Authors@R field.
* Fixed critical dependency issues (Imports for `httr`, `rappdirs`, `tibble`) that caused previous archival and check failures.
* Ensured explicit namespace calls (`pkg::fun()`) throughout the codebase to satisfy modern check requirements.
* Bumped version to 0.6.2.
