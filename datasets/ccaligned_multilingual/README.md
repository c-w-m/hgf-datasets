---
annotations_creators:
- no-annotation
language_creators:
- found
languages:
- af
- ak
- am   
- ar
- as
- ay
- az
- be
- bg
- bm
- bn
- br
- bs   
- ca
- cb
- cs
- cx   
- cy
- de   
- dv
- el
- eo   
- es   
- fa
- ff
- fi
- fo
- fr   
- fy   
- ga
- gl
- gn
- gu   
- he
- hi
- hr
- hu
- id
- ig   
- is
- it   
- iu
- ja
- ka
- kg   
- kk
- km   
- kn   
- ko
- ku   
- ky   
- la   
- lg
- li
- ln
- lo   
- lt
- lv
- mg   
- mi   
- mk
- ml   
- mn   
- mr   
- ms
- mt
- my   
- my
- ne   
- nl
- no
- ns
- ny   
- om
- or
- pa   
- pl
- ps   
- pt
- qa   
- qd   
- rm
- ro
- ru   
- rw
- sc
- sd   
- se
- si   
- sk
- sl
- sn   
- so   
- sq
- sr
- ss
- st
- su   
- sv
- sw
- sy
- sz
- ta
- te   
- tg   
- th
- ti
- tl
- tn
- tr
- ts
- tt
- tz   
- ug
- uk
- ur
- uz
- ve
- vi
- wo
- wy
- xh   
- yi   
- yo   
- zh
- zh
- zu   
- zz
licenses:
- unknown
multilinguality:
- translation
size_categories:
- n<1K
- 1K<n<10K
- 10K<n<100K
- 100K<n<1M
- n>1M
source_datasets:
- original
task_categories:
- other
task_ids:
- other-other-translation
---

# Dataset Card for ccaligned_multilingual

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

- **Homepage:** http://www.statmt.org/cc-aligned/
- **Repository:** [Needs More Information]
- **Paper:** https://www.aclweb.org/anthology/2020.emnlp-main.480.pdf
- **Leaderboard:** [Needs More Information]
- **Point of Contact:** [Needs More Information]

### Dataset Summary

CCAligned consists of parallel or comparable web-document pairs in 137 languages aligned with English. These web-document pairs were constructed by performing language identification on raw web-documents, and ensuring corresponding language codes were corresponding in the URLs of web documents. This pattern matching approach yielded more than 100 million aligned documents paired with English. Recognizing that each English document was often aligned to mulitple documents in different target language, we can join on English documents to obtain aligned documents that directly pair two non-English documents (e.g., Arabic-French). This corpus was created from 68 Commoncrawl Snapshots.


To load a language which isn't part of the config, all you need to do is specify the language code. You can find the valid languages in http://www.statmt.org/cc-aligned/ E.g.
```
dataset = load_dataset("ccaligned_multilingual", language_code="fr_XX", type="documents")
```
or
```
dataset = load_dataset("ccaligned_multilingual", language_code="fr_XX", type="sentences")
```


### Supported Tasks and Leaderboards

[Needs More Information]

### Languages

The text in the dataset is in (137) multiple languages aligned with english.

## Dataset Structure

### Data Instances

An instance of `documents` type for language `ak_GH`:

```
{'Domain': 'islamhouse.com', 'Source_URL': 'https://islamhouse.com/en/audios/373088/', 'Target_URL': 'https://islamhouse.com/ak/audios/373088/', 'translation': {'ak_GH': "Ntwatiaa / w??ab?? no t??fa w?? mu no te ase ma Umrah - Arab kasa|Islamhouse.com|Follow us:|facebook|twitter|taepe|Titles All|Fie wibesite|kasa nyina|Buukuu edi adanse ma prente|Nhyehy??mu|Nyim/sua Islam|Curriculums|Nyina nde??ma|Nyina nde??ma (295)|Buukuu/ nwoma (2)|sini / muuvi (31)|??dio (262)|A??n websideNew!|K?? wura kramosom mu seisei|Ebio|figa/kaas??|Farebae|AKAkan|Kratafa titriw|kasa interface( anyimu) : Akan|Kasa ma no mu-ns??m : Arab kasa|??dio|Ntwatiaa / w??ab?? no t??fa w?? mu no te ase ma Umrah|play|pause|stop|mute|unmute|max volume|Kasakyer?? ni :|Farebae:|17 / 11 / 1432 , 15/10/2011|Nhyehy??mu:|Jurisprudence/ Esum Nimdea|Som|Hajj na Umrah|Jurisprudence/ Esum Nimdea|Som|Hajj na Umrah|Mmira ma Hajj na Umrah|nkyer??mu|kasamu /s??nt??ns ma te ase na Umrah w?? ... mu no hann ma no Quran na Sunnah na te ase ma no nana na no kasamu /s??nt??ns ma bi ma no emerging yi adu obusuani|Akenkane we ye di ko kasa bi su (36)|Afar - Qaf??r afa|Akan|Amhari ne - ????????????|Arab kasa - ????????|Assamese - ??????????????????|Bengali - ???????????????|Maldive - ????????????|Greek - ????????????????|English ( brofo kasa) - English|Persian - ??????????|Fula - pulla|French - Fran??ais|Hausa - Hausa|Kurdish - ?????????? ????????????|Uganda ne - Oluganda|Mandinka - Mandinko|Malayalam - ??????????????????|Nepali - ??????????????????|Portuguese - Portugu??s|Russian - ??????????????|Sango - Sango|Sinhalese - ???????????????|Somali - Soomaali|Albania ne - Shqip|Swahili - Kiswahili|Telugu - ?????????????????? ??????????????????|Tajik - ????????????|Thai - ?????????|Tagalog - Tagalog|Turkish - T??rk??e|Uyghur - ????????????????|Urdu - ????????|Uzbeck ne - ?????????? ????????|Vietnamese - Vi???t Nam|Wolof - Wolof|Chine ne - ??????|Soma k?? bi kyer?? adwen k?? w??b ebusuapanin|Soma k?? ne k?? hom adamfo|Soma k?? bi kyer?? adwen k?? w??b ebusuapanin|Ns??wso fael (1)|1|???????????? ???? ?????? ????????????|MP3 14.7 MB|Enoumah ebatahu|Rituals/Esom ajomadie ewu Hajji mmire .. 1434 AH [01] no fapemso Enum|Fiidbak/ Ye hiya wu jun kyiri|Lenke de y??e|k??ntakt y??n|A??n webside|Qura'an Kro kronkrom|Balagh|w?? mfinimfin Dowload faele|Y?? atuu bra Islam mu afei|Tsin de y??e ewu|Anaa bomu/combine h??n melin liste|?? Islamhouse Website/ Islam dan webi site|??|??|Yi mu kasa|", 'en_XX': 'SUMMARY in the jurisprudence of Umrah - Arabic - Abdul Aziz Bin Marzooq Al-Turaifi|Islamhouse.com|Follow us:|facebook|twitter|QuranEnc.com|HadeethEnc.com|Type|Titles All|Home Page|All Languages|Categories|Know about Islam|All items|All items (4057)|Books (701)|Articles (548)|Fatawa (370)|Videos (1853)|Audios (416)|Posters (98)|Greeting cards (22)|Favorites (25)|Applications (21)|Desktop Applications (3)|To convert to Islam now !|More|Figures|Sources|Curriculums|Our Services|QuranEnc.com|HadeethEnc.com|ENEnglish|Main Page|Interface Language : English|Language of the content : Arabic|Audios|?????????? ?????????? ????????????|SUMMARY in the jurisprudence of Umrah|play|pause|stop|mute|unmute|max volume|Lecturer : Abdul Aziz Bin Marzooq Al-Turaifi|Sources:|AlRaya Islamic Recoding in Riyadh|17 / 11 / 1432 , 15/10/2011|Categories:|Islamic Fiqh|Fiqh of Worship|Hajj and Umrah|Islamic Fiqh|Fiqh of Worship|Hajj and Umrah|Pilgrimage and Umrah|Description|SUMMARY in jurisprudence of Umrah: A statement of jurisprudence and Umrah in the light of the Quran and Sunnah and understanding of the Ancestors and the statement of some of the emerging issues related to them.|This page translated into (36)|Afar - Qaf??r afa|Akane - Akan|Amharic - ????????????|Arabic - ????????|Assamese - ??????????????????|Bengali - ???????????????|Maldivi - ????????????|Greek - ????????????????|English|Persian - ??????????|Fula - pulla|French - Fran??ais|Hausa - Hausa|kurdish - ?????????? ????????????|Ugandan - Oluganda|Mandinka - Mandinko|Malayalam - ??????????????????|Nepali - ??????????????????|Portuguese - Portugu??s|Russian - ??????????????|Sango - Yanga ti Sango|Sinhalese - ???????????????|Somali - Soomaali|Albanian - Shqip|Swahili - Kiswahili|Telugu - ??????????????????|Tajik - ????????????|Thai - ?????????|Tagalog - Tagalog|Turkish - T??rk??e|Uyghur - ????????????????|Urdu - ????????|Uzbek - ?????????? ????????|Vietnamese - Vi???t Nam|Wolof - Wolof|Chinese - ??????|Send a comment to Webmaster|Send to a friend?|Send a comment to Webmaster|Attachments (1)|1|???????????? ???? ?????? ????????????|MP3 14.7 MB|The relevant Material|The rituals of the pilgrimage season .. 1434 AH [ 01] the fifth pillar|The Quality of the Accepted Hajj (Piligrimage) and Its Limitations|Easy Path to the Rules of the Rites of Hajj|A Call to the Pilgrims of the Scared House of Allah|More|feedback|Important links|Contact us|Privacy policy|Islam Q&A|Learning Arabic Language|About Us|Convert To Islam|Noble Quran encyclopedia|IslamHouse.com Reader|Encyclopedia of Translated Prophetic Hadiths|Our Services|The Quran|Balagh|Center for downloading files|To embrace Islam now...|Follow us through|Or join our mailing list.|?? Islamhouse Website|??|??|Choose language|'}}
```

An instance of `sentences` type for language `ak_GH`:

```
{'LASER_similarity': 1.4549942016601562, 'translation': {'ak_GH': 'Salah (nyamefere) ye Mmerebeia', 'en_XX': 'What he dislikes when fasting (10)'}}
```

### Data Fields

For `documents` type:

- `Domain`: a `string` feature containing the domain.
- `Source_URL`: a `string` feature containing the source URL.
- `Target_URL`: a `string` feature containing the target URL.
- `translation`: a `dictionary` feature with two keys :
  - `en_XX`: a `string` feature containing the content in English.
  - <language_code>: a `string` feature containing the content in the `language_code` specified.

For `sentences` type:

- `LASER_similarity`: a `float32` feature representing the LASER similarity score.
- `translation`: a `dictionary` feature with two keys :
  - `en_XX`: a `string` feature containing the content in English.
  - <language_code>: a `string` feature containing the content in the `language_code` specified.

### Data Splits

[Needs More Information]

## Dataset Creation

### Curation Rationale

[Needs More Information]

### Source Data

#### Initial Data Collection and Normalization

[Needs More Information]

#### Who are the source language producers?

[Needs More Information]

### Annotations

#### Annotation process

[Needs More Information]

#### Who are the annotators?

[Needs More Information]

### Personal and Sensitive Information

[Needs More Information]

## Considerations for Using the Data

### Social Impact of Dataset

[Needs More Information]

### Discussion of Biases

[Needs More Information]

### Other Known Limitations

[Needs More Information]

## Additional Information

### Dataset Curators

[Needs More Information]

### Licensing Information

[Needs More Information]

### Citation Information

```
@inproceedings{elkishky_ccaligned_2020,
 author = {El-Kishky, Ahmed and Chaudhary, Vishrav and Guzm{\'a}n, Francisco and Koehn, Philipp},
 booktitle = {Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP 2020)},
 month = {November},
 title = {{CCAligned}: A Massive Collection of Cross-lingual Web-Document Pairs},
 year = {2020}
 address = "Online",
 publisher = "Association for Computational Linguistics",
 url = "https://www.aclweb.org/anthology/2020.emnlp-main.480",
 doi = "10.18653/v1/2020.emnlp-main.480",
 pages = "5960--5969"
}
```

### Contributions

Thanks to [@gchhablani](https://github.com/gchhablani) for adding this dataset.