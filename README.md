# Pytorch implementation for Adversarial Structure Matching for Structured Prediction Tasks

Pytorch implementation of : [Adversarial Structure Matching for Structured Prediction Tasks](http://openaccess.thecvf.com/content_CVPR_2019/papers/Hwang_Adversarial_Structure_Matching_for_Structured_Prediction_Tasks_CVPR_2019_paper.pdf). Due to my limited time and computation resources, I only perform several toy experiments on the Weizmann horse figure ground segmentation task.




## Table of Contents

- [Introduction](#introduction)
- [Install](#install)
- [Usage](#usage)
	- [Generator](#generator)
- [Badge](#badge)
- [Example Readmes](#example-readmes)
- [Related Efforts](#related-efforts)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Introduction

ASM (Adversarial Structure Matching for Structured Prediction Tasks) is a  new framework for structured prediction task which is proposed by Jyh-Jing Hwang et al, in CVPR2019.

ASM  trains a structure analyzer that provides the supervisory signals, the ASM loss. The structure analyzer is trained to maximize the ASM loss, or to emphasize recurring multi-
scale hard negative structural mistakes among co-occurring patterns. On the contrary, the structured prediction network is trained to reduce those mistakes and is thus enabled to distinguish fine-grained structures. As a result, training structured prediction networks using ASM reduces contextual confusion among objects and improves boundary localization.

![Results Visualization in Paper](C:\Users\19119\Desktop\用户手册\experiments.png)

## Dependencies

- Python3
- torch
- torchvision
- numpy
- opencv
- Pillow
- progress

## Usage

For training with only Structured Prediction Net and IID loss (in this project , BCE loss):
```sh
$ python main.py 
# Prints out the standard-readme spec
```

### Generator

To use the generator, look at [generator-standard-readme](https://github.com/RichardLitt/generator-standard-readme). There is a global executable to run the generator in that package, aliased as `standard-readme`.

## Badge

If your README is compliant with Standard-Readme and you're on GitHub, it would be great if you could add the badge. This allows people to link back to this Spec, and helps adoption of the README. The badge is **not required**.

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)

To add in Markdown format, use this code:

```
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
```

## Example Readmes

To see how the specification has been applied, see the [example-readmes](example-readmes/).

## Related Efforts

- [Art of Readme](https://github.com/noffle/art-of-readme) - 💌 Learn the art of writing quality READMEs.
- [open-source-template](https://github.com/davidbgk/open-source-template/) - A README template to encourage open-source contributions.

## Maintainers

[@RichardLitt](https://github.com/RichardLitt).

## Contributing

Feel free to dive in! [Open an issue](https://github.com/RichardLitt/standard-readme/issues/new) or submit PRs.

Standard Readme follows the [Contributor Covenant](http://contributor-covenant.org/version/1/3/0/) Code of Conduct.

### Contributors

This project exists thanks to all the people who contribute. 
<a href="graphs/contributors"><img src="https://opencollective.com/standard-readme/contributors.svg?width=890&button=false" /></a>


## License

[MIT](LICENSE) © Richard Littauer
