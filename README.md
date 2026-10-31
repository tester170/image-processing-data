# Данные для курса «Методы и алгоритмы цифровой обработки изображений»

Копии открытых наборов снимков для учебных блокнотов о ключевых точках (теория №7 и проектная работа по сравнению детекторов и дескрипторов OpenCV). Копии сделаны потому, что официальные серверы наборов бывают недоступны. Файлы не изменялись; авторские права принадлежат авторам наборов, использование — по их условиям (исследования и обучение, некоммерческое использование).

Файлы лежат в релизе [`datasets`](../../releases/tag/datasets) и скачиваются по адресу
`https://github.com/tester170/image-processing-data/releases/download/datasets/<имя файла>`.

## Oxford Affine (Affine Covariant Regions)

Visual Geometry Group, University of Oxford. 8 серий по 6 снимков одной плоской сцены с нарастающим искажением и эталонными гомографиями `H1to2p` … `H1to6p`.

| Файл | Искажение |
|---|---|
| `graf.tar.gz`, `wall.tar.gz` | смена ракурса |
| `boat.tar.gz`, `bark.tar.gz` | масштаб и поворот |
| `bikes.tar.gz`, `trees.tar.gz` | размытие |
| `leuven.tar.gz` | освещение |
| `ubc.tar.gz` | сжатие JPEG |

Источник: https://www.robots.ox.ac.uk/~vgg/research/affine/ (архивы — https://thor.robots.ox.ac.uk/datasets/affine/).
Ссылка: K. Mikolajczyk, T. Tuytelaars, C. Schmid, A. Zisserman, J. Matas, F. Schaffalitzky, T. Kadir, L. Van Gool. A Comparison of Affine Region Detectors. IJCV, 65(1/2), 2005.

## FIRE — Fundus Image Registration Dataset

FORTH-ICS, Papageorgiou Hospital, Aristotle University of Thessaloniki. 134 пары снимков глазного дна 2912×2912 пикселей (группы S, P, A) и по 10 эталонных точек на пару. Файл `FIRE.7z`.

Источник: https://projects.ics.forth.gr/cvrl/fire/
Ссылка: C. Hernandez-Matas, X. Zabulis, A. Triantafyllou, P. Anyfanti, S. Douma, A. A. Argyros. FIRE: Fundus Image Registration Dataset. Journal for Modeling in Ophthalmology, 1(4), 2017.

## Контрольные суммы SHA-256

```
f631c09a0f43fc1e092203f32f8f27e2e43e59b524918255d45474c50c91ea4f  bark.tar.gz
3b95c49accadfd71e63c2fa0f7602abcbadd87d7f53ff54eb1efb15210d19e0c  bikes.tar.gz
6e5721f37fbf9c3e974fd05935a42c1670f3e71aa3e5b218807ea046a068c603  boat.tar.gz
999871b945ee968a00a0d5f9af957d1382fb9dae1511cdee9553366817b53b5b  graf.tar.gz
9b1ade6e64e5b27eee43463ff8f9ad2bd2f9c6911666e93de2634f3a5c0fe5dc  leuven.tar.gz
04a39f201bffbc5035a560136fb37d2b36ecaa1532113eebfb113c90b5327f5d  trees.tar.gz
26ab4ac94c8d0b2ded66c3bfaeb3f12589ec33005e5b4d5fcba4639f5b6e5414  ubc.tar.gz
3cb3df75f40471f093adf6647d13df6a9f4312f7a222fc591d03f6c08e086344  wall.tar.gz
4f164d89a572d88a5f46bf7fe433813a21561163c83481d6e101573621f79700  FIRE.7z
```
