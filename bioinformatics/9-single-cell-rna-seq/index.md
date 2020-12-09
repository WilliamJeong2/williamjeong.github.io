---
layout: post
title: Single-cell RNA-seq
subtitle: 왜 single-cell RNA-seq인가?
draft: true
type: Terms
bioinformatics: true
text: true
author: Jinwoo Jeong
post-header: false
order: 9
published: true
---

> 이 글은 Harvard Chan Bioinformatics Core의 [scRNA-seq 입문](https://hbctraining.github.io/scRNA-seq_online/lessons/01_intro_to_scRNA-seq.html)을 번역한 글입니다.  의역이 포함되어있습니다.



# 왜 single-cell RNA-seq인가?

인간의 조직에는 놀랍도록 다양한 cell type, states, interaction들이 있습니다. 이러한 조직과 세포 유형을 잘 이해하기 위해 single-cell RNA-seq (scRNA-seq)은 개별 세포 수준에서 어떤 유전자가 발현되고 있는지  볼 수 있습니다.

이 흥미롭고 첨단적인 방법을 사용하여 다음을 수행할 수 있습니다:

- 조직에 존재하는 세포 유형을 탐색
- 알려지지 않은/ 희귀 세포 유형이나 상태를 식별
- defferentiation(분화 과정), 시간, 상태에 따른 유전자 발현의 변화를 설명
- 치료나 질병에 대한 조건들간에 특정 세포 유형에서 차등발현하는 유전자 식별
- explore changes in expression among a cell type while incorporating spatial, regulatory, and/or protein information

보다 일반적으로 사용되는 몇 가지 방법은 다음과 같습니다:

![img](img/sc_analyses.png)



# scRNA-seq 분석의 과제

scRNA-seq 전에는 세포 <u>발현의 평균</u>을 비교하는 간단한 방법인 **bulk RNA-seq**을 사용하여 전사체 분석을 수행했었습니다. 이 방법은 전사체를 비교(다른 종에서 추출한 동일한 조직 sample)을 찾거나 질병 연구에서 발현 특질을 정량화하는데 사용됩니다. 또한 sample에서 세포의 이질성(heterogeneity)이 예상되지 않거나 고려되지 않는 경우 질병 바이오 마커 발견도 가능합니다.

bulk RNA-seq은 조건들(treatment or disease) 간의 유전자 발현 차이를 탐색할 수 있지만, 세포 level에서의 차이는 적절하게 감지되지 않습니다. 예를 들어 아래의 이미지를 보면, bulk RNA-seq으로 분석(왼쪽)하면 유전자 A와 유전자 B의 발현 간의 올바른 연관성을 찾을 수 없습니다. 그러나, 세포 유형별, 세포 상태별로 세포를 적절하게 그룹화하면 유전자 간의 올바른 상관관계를 볼 수 있게 됩니다.



<img src="img/sc_vs_bulk_cells.png" alt="img" style="zoom:50%;" />



scRNA-seq은 cellular(세포질) 수준에서 발현을 포착할 수 있음에도 샘플 제작과 라이브러리 준비 등의 비용이 많이 들고 분석은 훨씬 더 복잡하고 해석하기 어렵습니다.
scRNA-seq 데이터의 분석 복잡성은 아래가  포함됩니다:

- 대용량 데이터
- cell당 시퀀싱 depth가 낮음
- 세포/샘플들간의 기술적 가변성
- 세포/샘플들간의 생물학적 가변성

각 복잡성에 대해서 자세히 살펴보면 다음과 같습니다:

### 대용량 데이터

scRNA-seq 실험의 발현 데이터는 수천 개의 cell에 대한 수만, 수십만 개의 read를 나타냅니다.데이터 출력은 훨씬 더 크기 때문에 분석하는데 더 많은 양의 컴퓨터 메모리와 더 많은 저장공간을 요구합니다. 또한, 분석 소요시간의 증가도 필요로 합니다.

### cell당 시퀀싱 depth가 낮음

scRNA-seq의 droplet 기반의 방법론 경우, 시퀀싱의 depth가 낮아서 cell당 전사체(transcriptome)의 10~50%만 감지되는 경우가 많습니다. 이로 인해서 많은 유전자에서 0 카운트 값이 생성됩니다. 하지만 특정 세포에서, 유전자의 카운트 값이 0이면 유전자가 발현(expression)되지 않았거나 전사체(transcripts)이 검출되지 않았음을 의미할 수도 있습니다. 세포 전반적으로 발현 수준이 높은 유전자들은 0 카운트 값을 가지는 경향이 있습니다. 이러한 특징때문에, 많은 유전자들이 어떤 세포에서도 감지되지 않을 것이고 유전자 발현이 세포들 사이에서 매우 다양하게 됩니다.





---

###  Reference

- https://hbctraining.github.io/scRNA-seq_online/lessons/01_intro_to_scRNA-seq.html
- *Trapnell, C. Defining cell types and states with single-cell genomics, Genome Research 2015 (doi: https://dx.doi.org/10.1101/gr.190595.115*
- 

