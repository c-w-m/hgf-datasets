---
annotations_creators:
- found
language_creators:
- found
multilinguality:
- multilingual
languages:
- en
- vi
licenses:
- unknown
size_categories:
- 100K<n<1M
source_datasets:
- original
task_categories:
- conditional-text-generation
task_ids:
- machine-translation
---

# Dataset Card for mt_eng_vietnamese

## Table of Contents
- [Dataset Card for mt_eng_vietnamese](#dataset-card-for-mt_eng_vietnamese)
  - [Table of Contents](#table-of-contents)
  - [Dataset Description](#dataset-description)
    - [Dataset Summary](#dataset-summary)
    - [Supported Tasks and Leaderboards](#supported-tasks-and-leaderboards)
    - [Languages](#languages)
  - [Dataset Structure](#dataset-structure)
    - [Data Instances](#data-instances)
    - [Data Fields](#data-fields)
    - [Data Splits](#data-splits)
  - [Dataset Creation](#dataset-creation)
    - [Curation Rationale](#curation-rationale)
    - [Source Data](#source-data)
      - [Initial Data Collection and Normalization](#initial-data-collection-and-normalization)
      - [Who are the source language producers?](#who-are-the-source-language-producers)
    - [Annotations](#annotations)
      - [Annotation process](#annotation-process)
      - [Who are the annotators?](#who-are-the-annotators)
    - [Personal and Sensitive Information](#personal-and-sensitive-information)
  - [Considerations for Using the Data](#considerations-for-using-the-data)
    - [Social Impact of Dataset](#social-impact-of-dataset)
    - [Discussion of Biases](#discussion-of-biases)
    - [Other Known Limitations](#other-known-limitations)
  - [Additional Information](#additional-information)
    - [Dataset Curators](#dataset-curators)
    - [Licensing Information](#licensing-information)
    - [Citation Information](#citation-information)

## Dataset Description

- **Homepage:** https://nlp.stanford.edu/projects/nmt/data/iwslt15.en-vi/
- **Repository:** [Needs More Information]
- **Paper:** [Needs More Information]
- **Leaderboard:** [Needs More Information]
- **Point of Contact:** [Needs More Information]

### Dataset Summary

Preprocessed Dataset from IWSLT'15 English-Vietnamese machine translation: English-Vietnamese.

### Supported Tasks and Leaderboards

Machine Translation 

### Languages

English, Vietnamese

## Dataset Structure

### Data Instances

An example from the dataset:
```
{
  'translation': {
    'en': 'In 4 minutes , atmospheric chemist Rachel Pike provides a glimpse of the massive scientific effort behind the bold headlines on climate change , with her team -- one of thousands who contributed -- taking a risky flight over the rainforest in pursuit of data on a key molecule .', 
    'vi': 'Trong 4 ph??t , chuy??n gia ho?? h???c kh?? quy???n Rachel Pike gi???i thi???u s?? l?????c v??? nh???ng n??? l???c khoa h???c mi???t m??i ?????ng sau nh???ng ti??u ????? t??o b???o v??? bi???n ?????i kh?? h???u , c??ng v???i ??o??n nghi??n c???u c???a m??nh -- h??ng ng??n ng?????i ???? c???ng hi???n cho d??? ??n n??y -- m???t chuy???n bay m???o hi???m qua r???ng gi?? ????? t??m ki???m th??ng tin v??? m???t ph??n t??? then ch???t .'
    }
}
```


### Data Fields

- translation:
  - en: text in english
  - vi: text in vietnamese


### Data Splits

train: 133318, validation: 1269, test: 1269

## Dataset Creation

### Curation Rationale

[More Information Needed]

### Source Data

#### Initial Data Collection and Normalization

[More Information Needed]

#### Who are the source language producers?

[More Information Needed]

### Annotations

#### Annotation process

[More Information Needed]

#### Who are the annotators?

[More Information Needed]

### Personal and Sensitive Information

[More Information Needed]

## Considerations for Using the Data

### Social Impact of Dataset

[More Information Needed]

### Discussion of Biases

[More Information Needed]

### Other Known Limitations

[More Information Needed]

## Additional Information

### Dataset Curators

[More Information Needed]

### Licensing Information

[More Information Needed]

### Citation Information

```
@inproceedings{Luong-Manning:iwslt15,
        Address = {Da Nang, Vietnam}
        Author = {Luong, Minh-Thang  and Manning, Christopher D.},
        Booktitle = {International Workshop on Spoken Language Translation},
        Title = {Stanford Neural Machine Translation Systems for Spoken Language Domain},
        Year = {2015}}

```

### Contributions

Thanks to [@Nilanshrajput](https://github.com/Nilanshrajput) for adding this dataset.