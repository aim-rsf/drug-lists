# AI-MLTC Drug Lists

This repository has been setup to share drug lists across NIHR's AIM projects.
Currently, the drug lists come from the AIM Consortium OPTIMAL, based in Birmingham.

## About the lists
There is variation in how different systems approach the classification and mapping of various drugs, and it has been noted that there is a lack of single data consistency. 

The drug lists have been created using different methods to find a more efficient process to integrate as part of the Code Builder tool:

- **Method 1**: Involved manually curating a list of generic drug names on the BNF, and searching for respective brand names on the dm+d browser
- **Method 2**: Involves the use of both the [`snomedizer`](https://github.com/ramses-antibiotics/snomedizer) `R` package and a dm+d tool implementation (downloading latest dm+d distribution from NHS [Technology Reference Update Distribution TRUD webpage](https://isd.digital.nhs.uk/trud/users/guest/filters/0/home)). It's in the pipeline to create a self-contained wrapper for this process.
  - this method is a substance-based approach and involves running through a list of IDs for medicinal products.
 
## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
