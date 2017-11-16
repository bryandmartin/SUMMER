## Test environments
* local OS X install, R 3.4.2
* ubuntu 12.04 (on travis-ci), R 3.4.2
* win-builder (devel and release)

## R CMD check results
There were no ERRORs or WARNINGs. There was 3 NOTEs:

* Maintainer: ‘Bryan D Martin <bmartin6@uw.edu>’

New submission

Suggests or Enhances not in mainstream repositories:
  INLA 
 Availability using Additional_repositories specification:
  INLA   yes   https://www.math.ntnu.no/inla/R/stable
  
The first part does not seem to be an issue. For the latter, the INLA repository is included in Additional_repositories.

* Files ‘README.md’ or ‘NEWS.md’ cannot be checked without ‘pandoc’ being installed.

I can remove this NOTE by adding README.md file to .Rbuildignore, but I don't think I should do this.

* Possibly mis-spelled words in DESCRIPTION:
  Spatio (3:8)
  spatio (9:63)
  
The word spatio is not misspelled. It is part of the hyphenated word spatio-temporal.
