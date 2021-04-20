# Energy efficient system for detection of elephants with Machine Learning

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This repository contains files that were created while writing my Master's thesis, as well as presentation files for thesis defence.

Final version of the thesis is available in `final_thesis_pdf` folder, as well as in Digital library of University of Maribor, available [here](https://dk.um.si/IzpisGradiva.php?id=78319&lang=slv).

## Abstract

Human-Elephant Conflicts are a major problem in terms of elephant conservation.
According to WILDLABS, an average of 400 people and 100 elephants are killed every year in India alone because of them. 
Early warning systems replace the role of human watchers and warn local communities of nearby, potentially life threatening, elephants, thus minimising the Human-Elephant Conflicts.

In this Master's thesis we present the structure of an early warning system, which consists of several low-power embedded systems equipped with thermal cameras and a single gateway.
To detect elephants from captured thermal images we used Machine Learning methods, specifically Convolutional Neural Networks.
The main focus of this thesis was the design, implementation and evaluation of Machine Learning models running on microcontrollers under low-power conditions.
We designed and trained several accurate image classification models, optimised them for on-device deployment and compared them against models trained with commercial software in terms of accuracy, inference speed and size.
While writing firmware, we ported a part of the TensorFlow library and created our own build system, suitable for the libopencm3 platform. 
We also implemented reporting of inference results over the LoRaWAN network and described a possible server-size solution.
We finally a constructed fully functional embedded system from various development and evaluation boards, and evaluated its performance in terms of power consumption.
We show that embedded systems with Machine Learning capabilities are a viable solution to many real life problems.

## Generating a pdf file

This section assumes that user is using the Ubuntu's distribution of Linux. Thesis was written in Latex. In order to successfully build pdf document from the latex source files following packages need to be installed.

```bash
sudo apt install xdotool
sudo apt install latexmk
sudo apt install texlive-latex-extra
```

To edit and build latex source files I used [Vim](https://github.com/vim/vim) and plug-in [vimtex](https://github.com/lervag/vimtex). To view generated pdf file [Zathura](https://pwmt.org/projects/zathura/) was used.

## Related repositories

* [MicroML](https://github.com/MarkoSagadin/MicroML) Small framework that combines TensorFlow and libopencm3 to quick start ML embedded projects.

## Licensing

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
