---
layout: post
title: "Bioinformatics 기본 개념 정리"
subtitle: "Bioinformatics Series #1"
draft : true
type: "Bioinformatics"
blog: true
text: true
author: "Jinwoo Jeong"
post-header: false
post-header: ""
order: 2
---

> 최근 NGS(Next-Generation Sequencing)이 널리 활용됨에 따라 바이오 빅데이터가 홍수처럼 넘치고 있다. 이에 따라 현대 생물학은 변화를 맞이하고 있다. 방대한 규모의 바이오 빅데이터 안에서 생물학적으로 의미있는 정보들을 얻어내기 위해 전산학과 통계학접 접근법이 필요하게 되었고, 그 결과 생물정보학이라는 학문이 탄생하였다.[^1]

## Bioinformatics의 정의

Bio(생물)과 informatics(정보과학, 전산학)의 합성어다. Bioinformatics는 전산학, 통계학적인 기술들을 이용하여 대량으로 생산되는 생물학 관련 데이터를 분석하는 분야이다.



## 유전학에 관련된 용어들

우리 몸은 세포로 이루어져 있다. 세포에는 핵이, 핵에는 염색체가, 염색체에는 DNA가 있다.

DNA는 뉴클레오티드(Nucleotide)라는 단위로 구성되어 있으며, DNA 체인인 유전자를 이룬다.

뉴클레오티드는 **당**, **염기**, **인산**으로 이루어져 있는데 이 염기에 우리가 아는 서열이 나오게 된다. C/G/A/T 즉, 시토신, 구아닌, 아데닌, 티민으로 이루어져 있으며 아데닌, 구아닌은 퓨린으로 시토신과 우라실, 티민은 피리미딘으로 나누어진다.

![](img/1.jpeg)

---

### DNA

![](img/2.gif)

간단한 설명 : 암호화된 유전정보를 가지고 있는 화합물.

복잡한 설명 : 뉴클레오타이드의 중합체인 두 개의 긴 가닥이 서로 꼬여있는 잉중나선 구조로 되어있는 고분자화합물. DNA는 시토신(사이토신), 구아닌, 아데닌, 티민이라는 4종류의 가득으로 뉴클레오타이드의 중합체를 연결하고 있다. 이는 핵염기로 구분되기 때문에 DNA 염기서열이라고 부른다. DNA 염기서열이 모두 유전정보를 나타내지는 않는다. 유전자 구간은 유전정보를 설명하지만 그렇지 않은 '비부호화 DNA' 구간도 존재한다. 과거에 기능을 가진 유전자였더라도 돌연변이를 통해 기능을 상실한 슈도진[^2]이 되면 비부호화 DNA가 된다.

---

### RNA

![](img/3.jpg)

간단한 설명 : DNA를 이루는 핵산의 일종.

복잡한 설명 : 5탄당의 일종인 리보스를 기반으로 염기와 인산으로 된 고분자화합물. 분자구조와 생물학적 기능에 따라 크게 다섯가지로 구분된다.

- rRNA : 리보솜을 구성하는 RNA
- mRNA : DNA의 유전정보가 복사된 청사진 역할. 이를 기본으로 하여 리보솜에서 단백질을 구성
- tRNA : 안티코돈을 가지고 있으며, 그에 대응하는 특정 아미노산을 꼬리쪽에 달고 있는 RNA
- miRNA : 생물의 유전자 발현을 제어하는 역할
- siRNA : 특정 단백질의 생산을 방해해 유전자 발현을 억제











[^1]: [생물정보학 연구실](http://biosci.snu.ac.kr/baeklab/aboutus) 의 연구실 소개 인용.
[^2]: 세포의 유전자 발현이나 단백질 합성에 관여하지 않는 DNA 염기서열



### Reference

http://www.incodom.kr/RNA
https://ko.wikipedia.org/wiki/RNA
http://ko.experiments.wikidok.net/wp-d/59d05f520966ec85478c0be5/Viewhttps://www.expii.com/t/dna-vs-rna-10205
