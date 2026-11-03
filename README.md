# Данные для курса «Методы и алгоритмы цифровой обработки изображений»

Копии открытых наборов снимков и видео для учебных блокнотов курса: ключевые точки (теория №7 и практическая работа по сравнению детекторов и дескрипторов OpenCV) и анализ движения (теория №9 и практическая работа №9). Копии сделаны потому, что официальные серверы наборов бывают недоступны. Архивы снимков не изменялись, видео MOTChallenge собраны из исходных кадров (см. ниже); авторские права принадлежат авторам наборов, использование — по их условиям (исследования и обучение, некоммерческое использование).

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

## MOTChallenge: видео неподвижных камер с эталонными траекториями людей

Релиз [`motion`](../../releases/tag/motion): четыре последовательности из наборов MOT15 и MOT17 ([motchallenge.net](https://motchallenge.net/), лицензия [CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/)) для теории и практической работы по анализу движения. Кадры исходных последовательностей собраны в видео MP4 (H.264); эталонные рамки людей сохранены в CSV со столбцами `frame`, `id`, `x`, `y`, `w`, `h` в координатах видео. Для MOT17 оставлены только учитываемые рамки пешеходов (флаг учёта 1, класс 1).

| Файлы | Последовательность | Видео |
|---|---|---|
| `PETS09-S2L1.mp4`, `PETS09-S2L1_gt.csv` | MOT15 PETS09-S2L1 (PETS 2009) | 795 кадров, 768×576, 7 кадров/с |
| `MOT17-04.mp4`, `MOT17-04_gt.csv` | MOT17-04 | 1050 кадров, 960×540 (уменьшено с 1920×1080), 30 кадров/с |
| `MOT17-09.mp4`, `MOT17-09_gt.csv` | MOT17-09 | 525 кадров, 960×540, 30 кадров/с |
| `MOT17-02.mp4`, `MOT17-02_gt.csv` | MOT17-02 | 600 кадров, 960×540, 30 кадров/с |

Ссылки: L. Leal-Taixé, A. Milan, I. Reid, S. Roth, K. Schindler. MOTChallenge 2015: Towards a Benchmark for Multi-Target Tracking. arXiv:1504.01942, 2015; A. Milan, L. Leal-Taixé, I. Reid, S. Roth, K. Schindler. MOT16: A Benchmark for Multi-Object Tracking. arXiv:1603.00831, 2016; J. Ferryman, A. Shahrokni. PETS2009: Dataset and Challenge. PETS 2009.
