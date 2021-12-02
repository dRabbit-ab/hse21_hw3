# hse21_hw3

## Colab

https://colab.research.google.com/drive/10YfFi6uByFQsqGzWqCuxyjaCbqQOF0Df?usp=sharing

# Часть 1
## MultiQC

![image](https://user-images.githubusercontent.com/79662580/144418472-6b476852-4dea-44cb-9a14-49f62e0a2c4c.png)
![fastqc_sequence_counts_plot](https://user-images.githubusercontent.com/79662580/144418511-32fc7ad5-17d3-4598-9e08-a4ee5f8804f0.png)
![fastqc_per_base_sequence_quality_plot](https://user-images.githubusercontent.com/79662580/144418605-165d2aa4-53ec-47c3-83d3-6060389f2e93.png)
![fastqc_per_sequence_quality_scores_plot](https://user-images.githubusercontent.com/79662580/144418632-e08c3229-930d-4850-a7b5-87a6a39c1f69.png)
![fastqc_per_sequence_gc_content_plot](https://user-images.githubusercontent.com/79662580/144418722-329cc736-5d53-499b-9b34-0a0d4555dc3b.png)
![fastqc_per_base_n_content_plot](https://user-images.githubusercontent.com/79662580/144418756-9836a152-ebe6-42dd-bcf6-909a074242a2.png)
![fastqc_sequence_duplication_levels_plot](https://user-images.githubusercontent.com/79662580/144418787-70c5b961-17d1-4634-a79f-784e441676f3.png)
![fastqc-status-check-heatmap](https://user-images.githubusercontent.com/79662580/144418805-09c58666-cc86-4683-aa1d-bf255a102d5d.png)

## Hisat (Таблица с общей статистикой в конце Части 1)
!cat SRR3414629.hisat
21106089 reads; of these:
  21106089 (100.00%) were unpaired; of these:
    595976 (2.82%) aligned 0 times
    18375888 (87.06%) aligned exactly 1 time
    2134225 (10.11%) aligned >1 times
97.18% overall alignment rate

!cat SRR3414630.hisat
15244711 reads; of these:
  15244711 (100.00%) were unpaired; of these:
    412031 (2.70%) aligned 0 times
    13186139 (86.50%) aligned exactly 1 time
    1646541 (10.80%) aligned >1 times
97.30% overall alignment rate

!cat SRR3414631.hisat
24244069 reads; of these:
  24244069 (100.00%) were unpaired; of these:
    696383 (2.87%) aligned 0 times
    20928945 (86.33%) aligned exactly 1 time
    2618741 (10.80%) aligned >1 times
97.13% overall alignment rate

!cat SRR3414635.hisat
20956475 reads; of these:
  20956475 (100.00%) were unpaired; of these:
    560610 (2.68%) aligned 0 times
    18428317 (87.94%) aligned exactly 1 time
    1967548 (9.39%) aligned >1 times
97.32% overall alignment rate

!cat SRR3414636.hisat
20307147 reads; of these:
  20307147 (100.00%) were unpaired; of these:
    550088 (2.71%) aligned 0 times
    17825380 (87.78%) aligned exactly 1 time
    1931679 (9.51%) aligned >1 times
97.29% overall alignment rate

!cat SRR3414637.hisat
20385570 reads; of these:
  20385570 (100.00%) were unpaired; of these:
    538279 (2.64%) aligned 0 times
    17844858 (87.54%) aligned exactly 1 time
    2002433 (9.82%) aligned >1 times
97.36% overall alignment rate

## Количество уникально откартированных чтений
![уникальные картированные чтения](https://user-images.githubusercontent.com/79662580/144419404-fdc41655-9781-4c13-bc6b-1ba06d2ef561.jpg)

## Количество чтений на генах
Общее число чтений, соответствующих хотя бы одному гену для SRR3414629: 16049609

Общее число чтений, соответствующих хотя бы одному гену для SRR3414630: 11465324 

Общее число чтений, соответствующих хотя бы одному гену для SRR3414631: 18408851 

Общее число чтений, соответствующих хотя бы одному гену для SRR3414635: 16275997 

Общее число чтений, соответствующих хотя бы одному гену для SRR3414636: 15757580 

Общее число чтений, соответствующих хотя бы одному гену для SRR3414637: 15736978 

## All.counts
![image](https://user-images.githubusercontent.com/79662580/144432591-c9b26f01-921e-41f8-b6db-27fdd7aabcc5.png)

## Таблица со статистикой по каждому из 6 образцов

| id          | Тип        |  Кол-во чтений| Кол-во откартированных чтений | Процент откартированных чтений | Количество уникальных откартированных чтений | Процент уникально откартированных чтений | Кол-во чтений на генах |
|    :----:   |    :----:   |     :----:    |    :----:   |    :----:   |     :----:    |    :----:    |    :----:    |
| SRR3414629      | r | 21106089 | 20510113 | 97.18% | 18375888 | 87.06% | 16049609 |
| SRR3414630   | r | 15244711 | 14832680 | 97.30% | 13186139 | 86.50% | 11465324 |
| SRR3414631      | r | 24244069 | 23547686 | 97.13% | 20928945 | 86.33% | 18408851 |
| SRR3414635   | c | 20956475 | 20395865 | 97.32% | 18428317 | 87.94% | 16275997 |
| SRR3414636      | c | 20307147 | 19757059 | 97.30% | 17825380 | 87.79% | 15757580 |
| SRR3414637   | c | 20385570 | 19847291 | 97.36% | 17844858 | 87.54% | 15736978 |

# Часть 2
## MA-plot
![image](https://user-images.githubusercontent.com/79662580/144433721-d57f0d9e-3caf-4e3b-a1ab-fff1d5d30fce.png)
## Heatmap
![image](https://user-images.githubusercontent.com/79662580/144433861-2643d702-b8fb-4de7-9f35-3d60f8769c5a.png)
## Дифференциально экспрессированные гены
ENSMUSG00000000303.12            |  ENSMUSG00000025608.9 | ENSMUSG00000045545.8 |
:-------------------------:|:-------------------------:|:-------------------------:|
  ![image](https://user-images.githubusercontent.com/79662580/144451594-f59be457-85f9-4e5c-a707-be57cdc76d26.png) |  ![image](https://user-images.githubusercontent.com/79662580/144451632-5e7e963e-1b96-4b3e-9e01-894a7d9f50aa.png) | ![image](https://user-images.githubusercontent.com/79662580/144451671-08ef0286-b9d2-466f-bfab-848fec122341.png) |
