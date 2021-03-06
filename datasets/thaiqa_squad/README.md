---
annotations_creators:
- expert-generated
language_creators:
- found
languages:
- th
licenses:
- cc-by-nc-sa-3.0
multilinguality:
- monolingual
size_categories:
- 1K<n<10K
source_datasets:
- extended|other-thaiqa
task_categories:
- question-answering
task_ids:
- extractive-qa
- open-domain-qa
---

# Dataset Card for `thaiqa-squad`

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

- **Homepage:** http://github.com/pythainlp/thaiqa_squad (original `thaiqa` at https://aiforthai.in.th/)
- **Repository:** http://github.com/pythainlp/thaiqa_squad
- **Paper:**
- **Leaderboard:**
- **Point of Contact:**http://github.com/pythainlp/ (original `thaiqa` at https://aiforthai.in.th/)

### Dataset Summary

`thaiqa_squad` is an open-domain, extractive question answering dataset (4,000 questions in `train` and 74 questions in `dev`) in [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) format, originally created by [NECTEC](https://www.nectec.or.th/en/) from Wikipedia articles and adapted to [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) format by [PyThaiNLP](https://github.com/PyThaiNLP/).

### Supported Tasks and Leaderboards

extractive question answering

### Languages

Thai

## Dataset Structure

### Data Instances

```
{'answers': {'answer': ['???????????????????????????'], 'answer_begin_position': [528], 'answer_end_position': [537]}, 'article_id': 115035, 'context': '<doc id="115035" url="https://th.wikipedia.org/wiki?curid=115035" title="??????????????????">?????????????????? ?????????????????? () ?????????????????????????????????????????????????????????????????????????????????????????? ?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????? ????????????????????????????????? ?????? ??????????????? ???????????????????????????????????? 1970 ????????? 1980 ?????????????????????????????????????????????????????????????????? ???????????????????????????????????????????????? ?????????????????? ????????????????????????????????????????????????????????? ???????????????????????????????????????????????????????????? ??????????????????????????? ????????????????????????????????????????????? ???.???. 2517 ??????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????? ????????????????????????????????????????????????????????????????????? ????????????????????????????????????????????????????????????????????? ????????????????????? Benji\'s Theme (I Feel Love) ????????????????????? ?????????????????? ????????? ?????????????????????????????????????????????????????????????????????????????? ????????????????????? ??????????????????????????? (???.???. 2502 - ???.???. 2518) ??????????????????????????? 15 ????????????????????????????????????????????? ?????????????????????????????????????????????????????????????????????????????????????????? ???????????????????????????????????? ???.???. 2518????????????????????????????????????????????????????????????????????????????????????????????????. - ???.???. 2517, Benji (????????????????????????) - ???.???. 2520, For the Love of Benji (????????????????????????) - ???.???. 2521, Benji\'s Very Own Christmas Story (????????????????????????????????????????????????) - ???.???. 2523, Oh Heavenly Dog (????????????????????????) - ???.???. 2523, Benji at Work (????????????????????????????????????????????????) - ???.???. 2524, Benji Takes a Dive at Marineland (????????????????????????????????????????????????) - ???.???. 2526, Benji, Zax & the Alien Prince (??????????????????????????????????????????) - ???.???. 2530, Benji the Hunted (????????????????????????) - ???.???. 2547, Benji: Off the Leash! (????????????????????????) - ???.???. 2550, Benji: The Barkening (????????????????????????)</doc>\n', 'question': '?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????? Benji ??????????????????????????????????????? ???.???. 2517 ???????????????????????????????????????', 'question_id': 1}
{'answers': {'answer': ['?????????????????? ?????????'], 'answer_begin_position': [482], 'answer_end_position': [492]}, 'article_id': 115035, 'context': '<doc id="115035" url="https://th.wikipedia.org/wiki?curid=115035" title="??????????????????">?????????????????? ?????????????????? () ?????????????????????????????????????????????????????????????????????????????????????????? ?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????? ????????????????????????????????? ?????? ??????????????? ???????????????????????????????????? 1970 ????????? 1980 ?????????????????????????????????????????????????????????????????? ???????????????????????????????????????????????? ?????????????????? ????????????????????????????????????????????????????????? ???????????????????????????????????????????????????????????? ??????????????????????????? ????????????????????????????????????????????? ???.???. 2517 ??????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????? ????????????????????????????????????????????????????????????????????? ????????????????????????????????????????????????????????????????????? ????????????????????? Benji\'s Theme (I Feel Love) ????????????????????? ?????????????????? ????????? ?????????????????????????????????????????????????????????????????????????????? ????????????????????? ??????????????????????????? (???.???. 2502 - ???.???. 2518) ??????????????????????????? 15 ????????????????????????????????????????????? ?????????????????????????????????????????????????????????????????????????????????????????? ???????????????????????????????????? ???.???. 2518????????????????????????????????????????????????????????????????????????????????????????????????. - ???.???. 2517, Benji (????????????????????????) - ???.???. 2520, For the Love of Benji (????????????????????????) - ???.???. 2521, Benji\'s Very Own Christmas Story (????????????????????????????????????????????????) - ???.???. 2523, Oh Heavenly Dog (????????????????????????) - ???.???. 2523, Benji at Work (????????????????????????????????????????????????) - ???.???. 2524, Benji Takes a Dive at Marineland (????????????????????????????????????????????????) - ???.???. 2526, Benji, Zax & the Alien Prince (??????????????????????????????????????????) - ???.???. 2530, Benji the Hunted (????????????????????????) - ???.???. 2547, Benji: Off the Leash! (????????????????????????) - ???.???. 2550, Benji: The Barkening (????????????????????????)</doc>\n', 'question': "???????????? Benji's Theme ????????????????????????????????????????????????????????????????????? Benji ???????????????.???. 2517 ???????????????????????????????????????", 'question_id': 2035}
```

### Data Fields

```
{
    "question_id": question id
    "article_id": article id
    "context": article texts
    "question": question
    "answers":
        {
            "answer": answer text
            "answer_begin_position": answer beginning position
            "answer_end_position": answer exclusive upper bound position
        }
    ),
}
```

### Data Splits

|                         | train       | valid       |
|-------------------------|-------------|-------------|
| # questions             | 4000        | 74          |
| # avg words in context  | 1186.740750 | 1016.459459 |
| # avg words in question | 14.325500   | 12.743243   |
| # avg words in answer   | 3.279750    | 4.608108    |

## Dataset Creation

### Curation Rationale

[PyThaiNLP](https://github.com/PyThaiNLP/) created `thaiqa_squad` as a [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) version of [thaiqa](http://copycatch.in.th/thai-qa-task.html). [thaiqa](https://aiforthai.in.th/corpus.php) is part of [The 2nd Question answering program from Thai Wikipedia](http://copycatch.in.th/thai-qa-task.html) of [National Software Contest 2020](http://nsc.siit.tu.ac.th/GENA2/login.php).

### Source Data

#### Initial Data Collection and Normalization

[More Information Needed]

#### Who are the source language producers?

Wikipedia authors for contexts and [NECTEC](https://www.nectec.or.th/en/) for questions and answer annotations

### Annotations

#### Annotation process

[More Information Needed]

#### Who are the annotators?

[NECTEC](https://www.nectec.or.th/en/)

### Personal and Sensitive Information

All contents are from Wikipedia. No personal and sensitive information is expected to be included.

## Considerations for Using the Data

### Social Impact of Dataset

- open-domain, extractive question answering in Thai

### Discussion of Biases

[More Information Needed]

### Other Known Limitations

- The contexts include `<doc>` tags at start and at the end

## Additional Information

### Dataset Curators

[NECTEC](https://www.nectec.or.th/en/) for original [thaiqa](https://aiforthai.in.th/corpus.php). SQuAD formattting by [PyThaiNLP](https://github.com/PyThaiNLP/).

### Licensing Information

CC-BY-NC-SA 3.0

### Citation Information

[More Information Needed]

### Contributions

Thanks to [@cstorm125](https://github.com/cstorm125) for adding this dataset.