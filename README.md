# Resolving References in Visually-Grounded Dialogue via Text Generation

🚧 **NOTE**: We are in the process of adding the material described in our paper to this repo. Our annotations for "[A Game Of Sorts](https://github.com/willemsenbram/a-game-of-sorts)" are already available.

Repository for the paper "[Resolving References in Visually-Grounded Dialogue via Text Generation](https://sigdialinlg2023.github.io/static/papers/sigdial/122_Paper.pdf)" presented at [SIGDIAL 2023](https://2023.sigdial.org/). 
Please cite the following work if you use anything from this repository or from our paper:

```bibtex
@inproceedings{willemsen-etal-2023-resolving,
    title = "Resolving References in Visually-Grounded Dialogue via Text Generation",
    author = "Willemsen, Bram  and
      Qian, Livia  and
      Skantze, Gabriel",
    booktitle = "Proceedings of the 24th Annual Meeting of the Special Interest Group on Discourse and Dialogue",
    month = sep,
    year = "2023",
    address = "Prague, Czech Republic",
    publisher = "Association for Computational Linguistics"
}
```

***

## :scroll: Overview

- [:telescope: The Task](#the-task)
- [:page_facing_up: The Data](#the-data)
  - [A Game Of Sorts](#a-game-of-sorts)
  - [Our Annotations](#our-annotations)
- [:spaghetti: The Code](#the-code)
- [:books: Supplementary Material](#supplementary-material)

***

## <a name="the-task"></a> :telescope: The Task

***

## <a name="the-data"></a> :page_facing_up: The Data

### <a name="a-game-of-sorts"></a> A Game Of Sorts

The data that were used for the fine-tuning and evaluation of our approach came from the collaborative image ranking task "[A Game Of Sorts](https://github.com/willemsenbram/a-game-of-sorts)".
For information about this task, we refer the reader to the "[Collecting Visually-Grounded Dialogue with A Game Of Sorts](https://aclanthology.org/2022.lrec-1.242/)" paper.


In order to reproduce our work and make effective use of our annotations, you will need the "[A Game Of Sorts](https://github.com/willemsenbram/a-game-of-sorts)" data:

```
git clone https://github.com/willemsenbram/a-game-of-sorts.git
```


In order to download the images, in the `./a-game-of-sorts/dataset/` directory, run:
```
bash get_images.sh
```
The images will be downloaded to `./a-game-of-sorts/dataset/images`.


### <a name="our-annotations"></a> Our Annotations

Span-based mention annotations aligned with the images they denote can be found in the `./annotations/data` directory.

The referent descriptions from the various sources as discussed in the paper, including the manually constructed "ground truth" labels that have been used for fine-tuning and evaluation, can be found in the `./descriptions/data` directory.

***

## <a name="the-code"></a> :spaghetti: The Code

***

## <a name="supplementary-material"></a> :books: Supplementary Material

The supplementary material (`supplementary_material.pdf`) covers additional details about our human evaluation as well as hyperparameters used for model fine-tuning.
