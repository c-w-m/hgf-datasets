---
---

# Dataset Card for "xnli"

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks](#supported-tasks)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-fields)
  - [Data Splits Sample Size](#data-splits-sample-size)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)
  - [Contributions](#contributions)

## Dataset Description

- **Homepage:** [https://www.nyu.edu/projects/bowman/xnli/](https://www.nyu.edu/projects/bowman/xnli/)
- **Repository:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Paper:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Point of Contact:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Size of downloaded dataset files:** 7384.70 MB
- **Size of the generated dataset:** 3076.99 MB
- **Total amount of disk used:** 10461.69 MB

### Dataset Summary

XNLI is a subset of a few thousand examples from MNLI which has been translated
into a 14 different languages (some low-ish resource). As with MNLI, the goal is
to predict textual entailment (does sentence A imply/contradict/neither sentence
B) and is a classification task (given two sentences, predict one of three
labels).

### Supported Tasks

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Languages

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Dataset Structure

We show detailed information for up to 5 configurations of the dataset.

### Data Instances

#### all_languages

- **Size of downloaded dataset files:** 461.54 MB
- **Size of the generated dataset:** 1535.82 MB
- **Total amount of disk used:** 1997.37 MB

An example of 'train' looks as follows.
```
This example was too long and was cropped:

{
    "hypothesis": "{\"language\": [\"ar\", \"bg\", \"de\", \"el\", \"en\", \"es\", \"fr\", \"hi\", \"ru\", \"sw\", \"th\", \"tr\", \"ur\", \"vi\", \"zh\"], \"translation\": [\"?????? ????...",
    "label": 0,
    "premise": "{\"ar\": \"?????????? ???? ???????????? ?????????? ???????????? ???????????????? ???????? ?????? ??????\", \"bg\": \"???????? ???? ???????????? ???????????? ???? ???? ???????? ???????????????????? .\", \"de\": \"Eine ..."
}
```

#### ar

- **Size of downloaded dataset files:** 461.54 MB
- **Size of the generated dataset:** 104.26 MB
- **Total amount of disk used:** 565.81 MB

An example of 'validation' looks as follows.
```
{
    "hypothesis": "???????? ???????? ?????????? ???????????? ?????????? ????????????????.",
    "label": 1,
    "premise": "?????????? ?????????? ?????? ?????? ????????????."
}
```

#### bg

- **Size of downloaded dataset files:** 461.54 MB
- **Size of the generated dataset:** 122.38 MB
- **Total amount of disk used:** 583.92 MB

An example of 'train' looks as follows.
```
This example was too long and was cropped:

{
    "hypothesis": "\"?????????? ???????????? ???? ???????????????? ???????? , ?????? ???????????? ???? ?????????????????? .\"...",
    "label": 0,
    "premise": "\"???? ?????????? ???? ???????????? ?? ?????????????????????? , ???? ???? ???????????? ???????? ???? ???? ?????????????? ???? ???????????????????? ???????? , ?????? ???? ?????????? ???? ???? ?????????????????? ???????????? ???? ..."
}
```

#### de

- **Size of downloaded dataset files:** 461.54 MB
- **Size of the generated dataset:** 82.18 MB
- **Total amount of disk used:** 543.73 MB

An example of 'train' looks as follows.
```
This example was too long and was cropped:

{
    "hypothesis": "Man verliert die Dinge auf die folgende Ebene , wenn sich die Leute erinnern .",
    "label": 0,
    "premise": "\"Du wei??t , w??hrend der Saison und ich sch??tze , auf deiner Ebene verlierst du sie auf die n??chste Ebene , wenn sie sich entschl..."
}
```

#### el

- **Size of downloaded dataset files:** 461.54 MB
- **Size of the generated dataset:** 135.71 MB
- **Total amount of disk used:** 597.25 MB

An example of 'validation' looks as follows.
```
This example was too long and was cropped:

{
    "hypothesis": "\"???????????????????? ?????? ???????? ?????? ?????????? ???? ?????????????? ?????????????????? ?????? ??????????.\"...",
    "label": 1,
    "premise": "?????? ????????, ????????, ???????????? ?????? ??????????."
}
```

### Data Fields

The data fields are the same among all splits.

#### all_languages
- `premise`: a multilingual `string` variable, with possible languages including `ar`, `bg`, `de`, `el`, `en`.
- `hypothesis`: a multilingual `string` variable, with possible languages including `ar`, `bg`, `de`, `el`, `en`.
- `label`: a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2).

#### ar
- `premise`: a `string` feature.
- `hypothesis`: a `string` feature.
- `label`: a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2).

#### bg
- `premise`: a `string` feature.
- `hypothesis`: a `string` feature.
- `label`: a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2).

#### de
- `premise`: a `string` feature.
- `hypothesis`: a `string` feature.
- `label`: a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2).

#### el
- `premise`: a `string` feature.
- `hypothesis`: a `string` feature.
- `label`: a classification label, with possible values including `entailment` (0), `neutral` (1), `contradiction` (2).

### Data Splits Sample Size

|    name     |train |validation|test|
|-------------|-----:|---------:|---:|
|all_languages|392702|      2490|5010|
|ar           |392702|      2490|5010|
|bg           |392702|      2490|5010|
|de           |392702|      2490|5010|
|el           |392702|      2490|5010|

## Dataset Creation

### Curation Rationale

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Source Data

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Annotations

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Personal and Sensitive Information

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Considerations for Using the Data

### Social Impact of Dataset

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Discussion of Biases

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Other Known Limitations

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Additional Information

### Dataset Curators

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Licensing Information

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Citation Information

```
@InProceedings{conneau2018xnli,
  author = {Conneau, Alexis
                 and Rinott, Ruty
                 and Lample, Guillaume
                 and Williams, Adina
                 and Bowman, Samuel R.
                 and Schwenk, Holger
                 and Stoyanov, Veselin},
  title = {XNLI: Evaluating Cross-lingual Sentence Representations},
  booktitle = {Proceedings of the 2018 Conference on Empirical Methods
               in Natural Language Processing},
  year = {2018},
  publisher = {Association for Computational Linguistics},
  location = {Brussels, Belgium},
}
```


### Contributions

Thanks to [@lewtun](https://github.com/lewtun), [@mariamabarham](https://github.com/mariamabarham), [@thomwolf](https://github.com/thomwolf), [@lhoestq](https://github.com/lhoestq), [@patrickvonplaten](https://github.com/patrickvonplaten) for adding this dataset.