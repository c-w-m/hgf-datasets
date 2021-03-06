---
---

# Dataset Card for "clue"

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

- **Homepage:** [https://dc.cloud.alipay.com/index#/topic/data?id=8](https://dc.cloud.alipay.com/index#/topic/data?id=8)
- **Repository:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Paper:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Point of Contact:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Size of downloaded dataset files:** 189.48 MB
- **Size of the generated dataset:** 463.81 MB
- **Total amount of disk used:** 653.29 MB

### Dataset Summary

CLUE, A Chinese Language Understanding Evaluation Benchmark
(https://www.cluebenchmarks.com/) is a collection of resources for training,
evaluating, and analyzing Chinese language understanding systems.

### Supported Tasks

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Languages

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Dataset Structure

We show detailed information for up to 5 configurations of the dataset.

### Data Instances

#### afqmc

- **Size of downloaded dataset files:** 1.14 MB
- **Size of the generated dataset:** 4.01 MB
- **Total amount of disk used:** 5.15 MB

An example of 'validation' looks as follows.
```
{
    "idx": 0,
    "label": 0,
    "sentence1": "???????????????????????????",
    "sentence2": "????????????????????????"
}
```

#### c3

- **Size of downloaded dataset files:** 3.05 MB
- **Size of the generated dataset:** 14.96 MB
- **Total amount of disk used:** 18.02 MB

An example of 'train' looks as follows.
```
This example was too long and was cropped:

{
    "answer": "???????????????",
    "choice": ["??????????????????", "??????????????????", "??????????????????", "???????????????"],
    "context": "[\"??????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????...",
    "id": 1,
    "question": "????????????????????????????????????????????????????"
}
```

#### chid

- **Size of downloaded dataset files:** 127.15 MB
- **Size of the generated dataset:** 259.71 MB
- **Total amount of disk used:** 386.86 MB

An example of 'train' looks as follows.
```
This example was too long and was cropped:

{
    "answers": {
        "candidate_id": [3, 5, 6, 1, 7, 4, 0],
        "text": ["????????????", "????????????", "????????????", "????????????", "????????????", "????????????", "????????????"]
    },
    "candidates": "[\"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\", \"????????????\"]...",
    "content": "[\"????????????????????????????????????????????????????????????????????????????????????????????????90????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????#idiom0000...",
    "idx": 0
}
```

#### cluewsc2020

- **Size of downloaded dataset files:** 0.08 MB
- **Size of the generated dataset:** 0.41 MB
- **Total amount of disk used:** 0.49 MB

An example of 'train' looks as follows.
```
{
    "idx": 0,
    "label": 1,
    "target": {
        "span1_index": 3,
        "span1_text": "??????",
        "span2_index": 27,
        "span2_text": "??????"
    },
    "text": "??????????????????????????????????????????????????????????????????????????????????????????????????????"
}
```

#### cmnli

- **Size of downloaded dataset files:** 29.95 MB
- **Size of the generated dataset:** 68.78 MB
- **Total amount of disk used:** 98.73 MB

An example of 'train' looks as follows.
```
{
    "idx": 0,
    "label": 0,
    "sentence1": "???????????????????????????????????????????????????-??????????????????",
    "sentence2": "????????????????????????????????????????????????????????????"
}
```

### Data Fields

The data fields are the same among all splits.

#### afqmc
- `sentence1`: a `string` feature.
- `sentence2`: a `string` feature.
- `label`: a classification label, with possible values including `0` (0), `1` (1).
- `idx`: a `int32` feature.

#### c3
- `id`: a `int32` feature.
- `context`: a `list` of `string` features.
- `question`: a `string` feature.
- `choice`: a `list` of `string` features.
- `answer`: a `string` feature.

#### chid
- `idx`: a `int32` feature.
- `candidates`: a `list` of `string` features.
- `content`: a `list` of `string` features.
- `answers`: a dictionary feature containing:
  - `text`: a `string` feature.
  - `candidate_id`: a `int32` feature.

#### cluewsc2020
- `idx`: a `int32` feature.
- `text`: a `string` feature.
- `label`: a classification label, with possible values including `true` (0), `false` (1).
- `span1_text`: a `string` feature.
- `span2_text`: a `string` feature.
- `span1_index`: a `int32` feature.
- `span2_index`: a `int32` feature.

#### cmnli
- `sentence1`: a `string` feature.
- `sentence2`: a `string` feature.
- `label`: a classification label, with possible values including `neutral` (0), `entailment` (1), `contradiction` (2).
- `idx`: a `int32` feature.

### Data Splits Sample Size

|   name    |train |validation|test |
|-----------|-----:|---------:|----:|
|afqmc      | 34334|      4316| 3861|
|c3         | 11869|      3816| 3892|
|chid       | 84709|      3218| 3231|
|cluewsc2020|  1244|       304|  290|
|cmnli      |391783|     12241|13880|

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

@misc{xu2020clue,
    title={CLUE: A Chinese Language Understanding Evaluation Benchmark},
    author={Liang Xu and Xuanwei Zhang and Lu Li and Hai Hu and Chenjie Cao and Weitang Liu and Junyi Li and Yudong Li and Kai Sun and Yechen Xu and Yiming Cui and Cong Yu and Qianqian Dong and Yin Tian and Dian Yu and Bo Shi and Jun Zeng and Rongzhao Wang and Weijian Xie and Yanting Li and Yina Patterson and Zuoyu Tian and Yiwen Zhang and He Zhou and Shaoweihua Liu and Qipeng Zhao and Cong Yue and Xinrui Zhang and Zhengliang Yang and Zhenzhong Lan},
    year={2020},
    eprint={2004.05986},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}

```


### Contributions

Thanks to [@thomwolf](https://github.com/thomwolf), [@JetRunner](https://github.com/JetRunner) for adding this dataset.