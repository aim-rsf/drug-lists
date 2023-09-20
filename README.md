# AI-MLTC Drug Lists
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

[![CC BY 4.0][cc-by-shield]][cc-by]

This repository has been setup to share drug code lists across NIHR's AIM projects.
The drug code lists currently available are created in collaboration with AIM Consortium OPTIMAL based in Birmingham, using their Code Builder tool.
You can find all the drug lists created by OPTIMAL in [this repository]([https://github.com/aim-rsf/phenotypes/tree/main/Drug%20Codes](https://github.com/THINKINGGroup/phenotypes/tree/main/Drug%20Codes)).

## About the lists
There is variation in the classification terminology used for drugs and conditions in data sources. Further, lack of clarity in the methodology process for generating the code lists and decisions made to modify output code lists makes reusability and reproducibility difficult.

The drug lists created have been thus been stored on this repo, along with documentation on the different methods used to generate the lists to encourage reusability and reproducibility.

The two methods used to curate the lists are outlined below:
- **Method 1**: Involves manually curating a list of generic drug names using [BNF treatment summaries](https://bnf.nice.org.uk/treatment-summaries/), and searching for respective brand names on the [dm+d browser](https://services.nhsbsa.nhs.uk/dmd-browser/)
- **Method 2**: Involves the use of both the [`snomedizer`](https://github.com/ramses-antibiotics/snomedizer) `R` package and a dm+d tool implementation (downloading latest dm+d release from [NHS TRUD webpage](https://isd.digital.nhs.uk/trud/users/guest/filters/0/home)). 
  - this method is a substance-based approach and involves running through a list of substance 'children' in medicinal products through snomedizer R package.

The full methods for the creation of the lists can be found in the [generation-process folder](/generation-process) and the drug lists themselves in the [drug-lists folder](/drug-lists).

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JennyCooper1"><img src="https://avatars.githubusercontent.com/u/107427234?v=4?s=100" width="100px;" alt="JennyCooper1"/><br /><sub><b>JennyCooper1</b></sub></a><br /><a href="#content-JennyCooper1" title="Content">🖋</a> <a href="https://github.com/aim-rsf/drug-lists/commits?author=JennyCooper1" title="Documentation">📖</a> <a href="#ideas-JennyCooper1" title="Ideas, Planning, & Feedback">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Rainiefantasy"><img src="https://avatars.githubusercontent.com/u/43926907?v=4?s=100" width="100px;" alt="Mahwish M"/><br /><sub><b>Mahwish M</b></sub></a><br /><a href="#content-Rainiefantasy" title="Content">🖋</a> <a href="https://github.com/aim-rsf/drug-lists/commits?author=Rainiefantasy" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/eirini-zormpa"><img src="https://avatars.githubusercontent.com/u/30151074?v=4?s=100" width="100px;" alt="Eirini Zormpa"/><br /><sub><b>Eirini Zormpa</b></sub></a><br /><a href="https://github.com/aim-rsf/drug-lists/commits?author=eirini-zormpa" title="Documentation">📖</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Specifically, 🖋️ `content` refers to creation of drug lists, 📖 `documentation` refers to the documentation created in this repository, and 🤔 `Feedback` refers to clinical auditing of the lists.

If you would like to contribute to this repository, e.g. because you have found an error, or because you have a code list you would like to contribute, please [open an issue](https://github.com/aim-rsf/drug-lists/issues/new), or email Dr. Eirini Zormpa at [ezormpa@turing.ac.uk](mailto:ezormpa@turing.ac.uk).

## Licence
The materials in this repository are free to reuse under the conditions of the [Creative Commons Attribution 4.0 licence](http://creativecommons.org/licenses/by/4.0/).

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
