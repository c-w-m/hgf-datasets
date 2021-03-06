---
annotations_creators:
- found
language_creators:
- found
languages:
  alignments:
  - ar
  - bg
  - de
  - es
  - fr
  - hr
  - hu
  - it
  - lt
  - mk
  - pl
  - pt
  - sq
  - sr
  - tr
  - vi
  crosslingual_bg:
  - bg
  crosslingual_hr:
  - hr
  crosslingual_hu:
  - hu
  crosslingual_it:
  - it
  crosslingual_mk:
  - mk
  crosslingual_pl:
  - pl
  crosslingual_pt:
  - pt
  crosslingual_sq:
  - sq
  crosslingual_sr:
  - sr
  crosslingual_test:
  - ar
  - bg
  - de
  - es
  - fr
  - hr
  - hu
  - it
  - lt
  - mk
  - pl
  - pt
  - sq
  - sr
  - tr
  - vi
  crosslingual_tr:
  - tr
  crosslingual_vi:
  - vi
  crosslingual_with_para_bg:
  - bg
  crosslingual_with_para_hr:
  - hr
  crosslingual_with_para_hu:
  - hu
  crosslingual_with_para_it:
  - it
  crosslingual_with_para_mk:
  - mk
  crosslingual_with_para_pl:
  - pl
  crosslingual_with_para_pt:
  - pt
  crosslingual_with_para_sq:
  - sq
  crosslingual_with_para_sr:
  - sr
  crosslingual_with_para_test:
  - ar
  - bg
  - de
  - es
  - fr
  - hr
  - hu
  - it
  - lt
  - mk
  - pl
  - pt
  - sq
  - sr
  - tr
  - vi
  crosslingual_with_para_tr:
  - tr
  crosslingual_with_para_vi:
  - vi
  multilingual:
  - ar
  - bg
  - de
  - es
  - fr
  - hr
  - hu
  - it
  - lt
  - mk
  - pl
  - pt
  - sq
  - sr
  - tr
  - vi
  multilingual_with_para:
  - ar
  - bg
  - de
  - es
  - fr
  - hr
  - hu
  - it
  - lt
  - mk
  - pl
  - pt
  - sq
  - sr
  - tr
  - vi
licenses:
- cc-by-sa-4.0
multilinguality:
  alignments:
  - multilingual
  crosslingual_bg:
  - monolingual
  crosslingual_hr:
  - monolingual
  crosslingual_hu:
  - monolingual
  crosslingual_it:
  - monolingual
  crosslingual_mk:
  - monolingual
  crosslingual_pl:
  - monolingual
  crosslingual_pt:
  - monolingual
  crosslingual_sq:
  - monolingual
  crosslingual_sr:
  - monolingual
  crosslingual_test:
  - multilingual
  crosslingual_tr:
  - monolingual
  crosslingual_vi:
  - monolingual
  crosslingual_with_para_bg:
  - monolingual
  crosslingual_with_para_hr:
  - monolingual
  crosslingual_with_para_hu:
  - monolingual
  crosslingual_with_para_it:
  - monolingual
  crosslingual_with_para_mk:
  - monolingual
  crosslingual_with_para_pl:
  - monolingual
  crosslingual_with_para_pt:
  - monolingual
  crosslingual_with_para_sq:
  - monolingual
  crosslingual_with_para_sr:
  - monolingual
  crosslingual_with_para_test:
  - multilingual
  crosslingual_with_para_tr:
  - monolingual
  crosslingual_with_para_vi:
  - monolingual
  multilingual:
  - multilingual
  multilingual_with_para:
  - multilingual
size_categories:
  alignments:
  - 10K<n<100K
  crosslingual_bg:
  - 1K<n<10K
  crosslingual_hr:
  - 1K<n<10K
  crosslingual_hu:
  - 1K<n<10K
  crosslingual_it:
  - 1K<n<10K
  crosslingual_mk:
  - 1K<n<10K
  crosslingual_pl:
  - 1K<n<10K
  crosslingual_pt:
  - n<1K
  crosslingual_sq:
  - 1K<n<10K
  crosslingual_sr:
  - 1K<n<10K
  crosslingual_test:
  - 10K<n<100K
  crosslingual_tr:
  - 1K<n<10K
  crosslingual_vi:
  - 1K<n<10K
  crosslingual_with_para_bg:
  - 1K<n<10K
  crosslingual_with_para_hr:
  - 1K<n<10K
  crosslingual_with_para_hu:
  - 1K<n<10K
  crosslingual_with_para_it:
  - 1K<n<10K
  crosslingual_with_para_mk:
  - 1K<n<10K
  crosslingual_with_para_pl:
  - 1K<n<10K
  crosslingual_with_para_pt:
  - n<1K
  crosslingual_with_para_sq:
  - 1K<n<10K
  crosslingual_with_para_sr:
  - 1K<n<10K
  crosslingual_with_para_test:
  - 10K<n<100K
  crosslingual_with_para_tr:
  - 1K<n<10K
  crosslingual_with_para_vi:
  - 1K<n<10K
  multilingual:
  - 10K<n<100K
  multilingual_with_para:
  - 10K<n<100K
source_datasets:
- original
task_categories:
- question-answering
task_ids:
- multiple-choice-qa
---

# Dataset Card for [Dataset Name]

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-instances)
  - [Data Splits](#data-instances)
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

- **Repository:** [EXAMS github repository](https://github.com/mhardalov/exams-qa)
- **Paper:** [EXAMS: A Multi-Subject High School Examinations Dataset for Cross-Lingual and Multilingual Question Answering](https://arxiv.org/abs/2011.03080)
- **Point of Contact:** [hardalov@@fmi.uni-sofia.bg](hardalov@@fmi.uni-sofia.bg)

### Dataset Summary

E??????s is a benchmark dataset for multilingual and cross-lingual question answering from high school examinations. It consists of more than 24,000 high-quality high school exam questions in 16 languages, covering 8 language families and 24 school subjects from Natural Sciences and Social Sciences, among others.

### Supported Tasks and Leaderboards

[More Information Needed]

### Languages

[More Information Needed]

## Dataset Structure

### Data Instances

An example of a data instance (with support paragraphs, in Bulgarian) is:
```
{'answerKey': 'C',
 'id': '35dd6b52-7e71-11ea-9eb1-54bef70b159e',
 'info': {'grade': 12, 'language': 'Bulgarian', 'subject': 'Biology'},
 'question': {'choices': {'label': ['A', 'B', 'C', 'D'],
   'para': ['???????? ???????? ???? ???????????????????????? ?????????????????? ?????????? ??????????????????????. ?????????????????????????????? ?????????????? ???? ????????????????????????. ??????????????, ???????????? ?? ???????????????? ???????? ???? ???????????????????? ???? ???????????? ???? ???????????????? ???? ???????????????? ?????????????? ?? ???????????????? ?? ???????????????? ???? ???????????????????????? ??????????????????. ???????? ????????????????, ???????????? ??????????????????, ???? ???? ????????????????????????. ???? ???? ?? ?????????? ???????????????????????? ???????? ?? ??????????. ???? ???? ???????? ???????????????????????? ?????????????? ?? ???????????????????? ????????????????????????. ?????????????????? ???? ??????????????????????, ????????????????????, ?????????????? (????????????????????????) ?? ????????????????????. ???????? ???? ?????????????????? 800 ??????????????????. ???? ???????????? ???????????????????????? ???????????????? ???? ?????????????????????? ???? ????????????, ??.??. ?????????????????????? ???????????????????????? ??????????????, ?????????? ?????????? ???? ??????????????, ???? ??????????. ???????? ???????????????????????? ??????????????????. ???????????????? ???? ?????? ???? ???????????????????????? ?? ???? ???????????????? ???? ??????????????????????. ???????????????? ???????????? ???? ???????????????????? ???? ???????????????? ???????????????????????? ???????? ?? ??????????????????????. ???????? 1509 ??. ???????????????????????? ???? ?????????????????? ???? ???????????????????????? ???????????????? ??????????????. ?????????????????? ???????????????? ???????????? ???????????????????????? ???? ???????????????????? ???? ??????????????????????????? ???????????????? ???????????????????. ?????????????????? ???????????????? ???????????? ???????????????????????? ???? ???????????????????? ???? ??????????????????????????? ???????????????? ???????????????????. ?????????????? ???? ???????????????? ???????????????????????? ????????????, ???? ????-?????????? ???????????? ?????????????? ????????????????????????. ?????????????????? ???? ???? ???????????????????????? ?? ???? ???????????????? ?? ?????????????? ???? ??????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ????????????????. ?? ???? ?????????????????? ?????????????????? ?? ???????????????? ????????. ???? ?????????? ???? ?????????????? ???????? ???????????????????????? ??????????????????. ?????????????????? ???? ???????????????????? ?? ?????????? ?? ??????????????. ?????????? ?????????? ???????????????????????? ??????????????. ?????????? ?????????? ???????????????????????? ??????????????. ?????????????????? ????????????????, ?????????????????????? ?? ?????????????????????? ???????????????? ???? ???????????????????????? ?? ?????? ?????????? ??????????????????.',
    '???????????????????? ?????????????????????????????? ???? ???????????????????????? ?????????????????? ???????????????? ?? ???? ???????????????????? ??????????????????. ???? ???? ???????????? ?????????? ???? ?????????????????????? ???? ????????????, ???????? ?? ???? ?????????????????????????? ???? ???????????????????????? ?????????????????? ?????????? ?????????????? ??????????. ???????? ?????????????????? ???? ?????????????? ????-????????. ????????????????????????, ?????? ???????????????????? ??????????????????. ???????????????? ???????????? ?????? ??????????????????. ???????? ?????????????? ???????????????? ???? ?????????????? ?????????????????? ?? ?????????????????????????? ????????????, ???????????? ???? ?? ?????????????????? ?? ?????????????????????? ?? ?????????????????? ??????????????????. ?????????????????????????? ???????????? ???? ?????????????????????????? ?????? ???????????????? ??????????????????: ???????????????????? ???? ?? ?????????????? ?????????????????? ?? ??????????????. ?????????????? ???? ?????????????????? ?? ???????????????????? ?????? ????????????. ?????? ???? ?????????????????????? ?? ???????????????????????? ???????????????????????? ??????????????????. ???????? ???? ?????????????????? 800 ??????????????????. ?????????????????????? ???? ???????????????????? ???????????????????? ??????????????????. ?????? ?????????????????? ???? ???????????????? ?????????????????? ?????? ?????????????????????????????? ??????????. ???????????? ???? ?? ?????????????????????????? ?????????????????? ?? ?????????????????? ??????????????????. ?????????? ?????????????? ???? ?????????? ???? ?????????????????? ???????????? 1143.4. ?????????????? ???? ???????????????????? ?? ???????????????????? ?????????????????? ???? ?????????????????? ??????????????. ???? ?????????????????? ?? ???????????????? ?? ???????????? ??????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ????????????????. ???? ?????????? ???? ?????????????? ???????? ???????????????????????? ??????????????????. ???????????????? ?????????????????? ?????????????????????? ?????????????????? ?????????????? ????????. ?????????????????? ???????????????????? ?????????????????? ?? ?????????????????????? ??????????????. ????-?????????? ?????? ???????????????????? ???????? ??????????????????. ?????????????????? ???????????????????? ?????????????????? ?? ?????????????????????? ??????????????. ???????????????????? ???????????????? ?????????????????? ???????? ???????????????? ????????????????????. ???????????????????????????? ?????????????????? ?? ???????????????? ?????? ??????????????????.',
    '?????????????????????????? ???? ????????????????. ???????? ?????????????? ???? ????????????????. ?? ?????????????????? ???????????? ???????? ?????????????????????? ???? ????????????????. ???????????? ???????????? ???????????? ???? ???????????????? ?? ????????????????. ?????????? ???? ?????????????????? ???? ???????????????? ?? ?????????????????? ?? ???????? ?????? ??????????????????????. ?????? ?? ?????????????????? ?????? ???????????? ????????, ???? ???? ???????????????? ?? ?????????? ?????? ?????????????????? . ???????? ???? ?????????????????? 800 ??????????????????. ???????????????????????????????????????? ?? ?????????????????????? ???? ???????????????? ???? "????????????????", ?????? ?????????? ?????????????????????????????????? ???? ?????????????????????? ???????? ???????????????????? ?????? ????????????????. ?????????????? ?????????????????? ?? ???????????????? ???? ???????????????????????? ?????????????? ???? ???? ????????????????, ???????? ?????????????? ?? ?? ???????????????????? ????????????????. ?????????????? ???? ????????????-???????????? ?? ?????????????? ???????????? ???? ???????????????? (?????????????? ???? ???????????? ?? ?????????????? ???? ???????????? ???? ????????????). ???????????????????????? ?????????????? ?? ?????? ??????????, ?? ???????????????????? ???? ???????????? ?? ?????????????????????????????????? ???? ??????????????????????????:\n\n?????????????? ?????? ?????????? ???? ????????????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ????????????????. ?? ???? ?????????????????? ?????????????????? ?? ???????????????? ????????. ???? ?????????? ???? ?????????????? ???????? ???????????????????????? ??????????????????. ?????????????????? ???? ???????????????????? ?? ?????????? ?? ??????????????. ???????????????? ?????????????? ?????????????? ???? ???? ???????????????????????? ???????????????????? ??????????????????. ?????????????????? ???? ?????????????????? ?? ?? ?????????????????? ???? ????????????????. ???????? ?????????????????? ???? ?????????????? ???????? ???????????????? 1878 ????????????. ???????????????????? ?????????????????? ???? ?????????????? ???????? ???????????? 2009 ????????????. ?? ?????????????? ???? ???????????????????????? ?????????????????????? ???? ?????????????? ?????????? ??????????????????. ???????????????????? ?????????????????? ???? ?? ???????? ???? ?????????????? ???????????????? ??????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ?????????????????? ?? ??????????????????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ?????????????????? ?? ??????????????????????. ?????????????? ???? ?????????????????? ?? ?????????????????????????? ???? ?????????????????? ?? ??????????????????????. ???????????????????? ?????????????????????????????? ???? ???????????????????????? ?????????????????? ???????????????? ?? ???? ???????????????????? ??????????????????.',
    '?????????????????? ?????????????? ???? ?????????? ???????????????? ??????????????. ???????????????????????? ?? ???????????????? ???? ???????????????? ???????????? ?????????? ????????????????. ???? ?????????? ???????? ?????????? ???????????????? ???????????? ?????????????????????? ???? ??????????????. ???????????????????? ???????????? ???????????????? ?????????????????? ?????????? ???????????????? ?? ?? ???????????????? ????????????. ???????????????? ???????????????????????????? ???? ??????????????????????? ???? ??????????????? ?????????????? ???????????????????? ?????????? ????????????????. ???????????????????? ???? ?????????????? ???????? ?????????? ???????????????? ?? ???????????? ?????????????????? ?????????? ????????????????. ???????????????????????? ???????????????? ???? ?? ???????????????? ???????????? ?? ?????????? ???????????????? ?? ???? ???????????????? ?????? ?????????????????? ?????????????????? ?? ??????????????????, ?? ???????????????????????????? ???? ???????????????????????? ???? ??????????????, ?????????? ?????????????????? ???????? ????????????, ?????????????????????? ???? ??????????????, ???????????? ?????????????????? ?? ????. ???????? ?????????????????? ????????????????. ???????????? ???? ?????????? ???? ???????????????????????? ???????????? ???? ?????????????????? ???????????? ???????????????????????? ???? ?????????????????? ?????????????????? ?????????? ????????????????. ???????? ???????????????????????????????? ???? ???????? ???????????? ?????? ??????????, ?????????????????????? ???? ?????????????????????????? ???? ???????????? ?????????????????? ?????????? ????????????????. ???? ???????? ???????????????????? ????????????????. ???? ???????? ?????????????????????????? ????????????????. ?????????????????????????????? ???? ?????????????? ???????? ???????????????????? ?????? ?????????? ????????????????, ???????????? ?????????????? ???????????? ?????????????????????? ???? ???????????????????? ???? ????????. ???????????????? ???????? ???????????????????? ?????????????????????????? ????????????????. ???????? ??????-?????????? ???????????????? ????????????????. ?????????????????? ???????? ???????????????? ?????????????????????????? ????????????????. ?????????? ???? ?????? ???????? ?????????????????????? ????????????????. ???????? ???????????????? ???????? ??????????????, ???????????????????? ????????????????. ???? ???????? ?????????????? ?????? ?????????????? ????????????????. ???????????????????? ?????????????????????????? ?????????? ???????? ???????????????? ????????????????. ?????????? ???????? ?????????????????????? ???????????????? (??????????????, ??????????). ?????????? ?? ???????????????????????????? ???????? ???????????????????????? ????????????????. ???????????????????? ?????????????? ???????? ?????????? ???? ???????????? ?????????????????????? ???? ???????????????????????????? ??????????????, ?????????????? ?????????????????? ?????????? ???????? ???????????? ????????????????. ?????????? ???????????????????? ???????? ???????? ?????????????????????????? ????????????????, ???????????? ?????????? ???????? ?????????????????????? ????????????. ?????????????? ???? ???????????? ???????? ????-???????????????? ????????????????.'],
   'text': ['???????????? ???? ???? ?????????????????? ??????????????????',
    '???????? ?????????? ????????????????',
    '???? ????????????????????????',
    '???? ????????????????']},
  'stem': '?????????????????????? ??????????????????:'}}
```

### Data Fields

A data instance contains the following fields:
- `id`: A question ID, unique across the dataset
- `question`: the question contains the following:
  - `stem`: a stemmed representation of the question textual
  - `choices`: a set of 3 to 5 candidate answers, which each have:
    - `text`: the text of the answers
    - `label`: a label in `['A', 'B', 'C', 'D', 'E']` used to match to the `answerKey`
    - `para`: (optional) a supported paragraph from Wikipedia in the same language as the question and answer
- `answerKey`: the key corresponding to the right answer's `label`
- `info`: some additional information on the question including:
  - `grade`: the school grade for the exam this question was taken from
  - `subject`: a free text description of the academic subject
  - `language`: the English name of the language for this question

### Data Splits

[More Information Needed]

## Dataset Creation

### Curation Rationale

[More Information Needed]

### Source Data

#### Initial Data Collection and Normalization

E??????s was collected from official state exams prepared by the ministries of education of various countries. These exams are taken by students graduating from high school, and often require knowledge learned through the entire course.

The questions cover a large variety of subjects and material based on the country???s education system. They cover major school subjects such as Biology, Chemistry, Geography, History, and Physics, but we also  highly specialized ones such as Agriculture, Geology, Informatics, as well as some applied and profiled studies.

Some countries allow students to take official examinations in several languages. This dataset rprovides 9,857 parallel question pairs spread across seven languages coming from Croatia (Croatian, Serbian, Italian, Hungarian), Hungary (Hungarian, German, French, Spanish, Croatian, Serbian, Italian), and North Macedonia (Macedonian, Albanian, Turkish).

For all languages in the dataset, the first step in the process of data collection was to download the PDF files per year, per subject, and per language (when parallel languages were available in the same source), convert the PDF files to text, and select those that were well formatted and followed the document structure.

Then, Regular Expressions (RegEx) were used to parse the questions, their corresponding choices and the correct answer choice. In order to ensure that all our questions are answerable using textual input only, questions that contained visual information were removed, as selected by using curated list of words such as map, table, picture, graph, etc., in the corresponding language.

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

The dataset, which contains paragraphs from Wikipedia, is licensed under CC-BY-SA 4.0. The code in this repository is licensed according the [LICENSE file](https://raw.githubusercontent.com/mhardalov/exams-qa/main/LICENSE).

### Citation Information

```
@article{hardalov2020exams,
  title={EXAMS: A Multi-subject High School Examinations Dataset for Cross-lingual and Multilingual Question Answering},
  author={Hardalov, Momchil and Mihaylov, Todor and Dimitrina Zlatkova and Yoan Dinkov and Ivan Koychev and Preslav Nvakov},
  journal={arXiv preprint arXiv:2011.03080},
  year={2020}
}
```

### Contributions

Thanks to [@yjernite](https://github.com/yjernite) for adding this dataset.