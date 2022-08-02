# Comparative-transcriptome-analysis-implied-a-ZEP-paralog-was-a-key-gene-involved-in-carotenoid-accum

논문을 읽고 RNA-seq 및 DEG 분석의 전반적인 흐름을 이해할 수 있었다.
분석한 결과를 통해 어떻게 생물학적 의미를 끌어올 수 있는 지 위주로 읽고자 했다.

https://pubmed.ncbi.nlm.nih.gov/34545178/


## 요약


노란색 과육 고구마 품종의 카로티노이드 축적 메커니즘은 명확하지 않다. 이 연구에서는 노란색 과육 품종인 Beniharuka(BH)와 자연적인 흰 과육 돌연변이(WH2 및 WH3) 두 가지의 전사체 profile을 비교하여 노란색 과육과 관련된 유전자를 밝혀냈다.


RNA-seq 결과, 총 185개의 차등 발현 유전자(differentially expressed genes,DEG)가 BH에 비해 WH2 및 WH3에서 일반적으로 검출되었다. 

제아잔틴 에폭시다제(ZEP)의 paralog인 g1103.t1은 저장 뿌리에서 카로티노이드 생합성에 관여하는 것으로 간주되는 38개의 유전자 중 WH2 및 WH3에만 공통적인 DEG였다. 

g1103.t1의 발현 수준은 5개의 노란색 과육 품종보다 5개의 흰 과육 품종에서 상당히 낮았다. 저장뿌리의 카로티노이드 구성 분석은 에폭시화 카로티노이드가 WH2와 WH3 모두에서 크게 감소했음을 보여주었다. 

따라서 본 연구에서는 고구마에서 beta-카로틴과 beta-크립토잔틴의 에폭시화를 통해 ZEP paralog g1103.t1이 카로티노이드 축적에 관여할 수 있다고 제안했다.


## BH, WH2 및 WH3 저장 뿌리의 전사체 프로파일링 

- Illumina NovaSeq 6000을 사용하여 3개의 생물학적 복제물이 있는 BH, WH2 및 WH3 저장 뿌리의 RNA-seq 데이터를 생성했다. 

- 평균적으로 낮은 품질의 read와 Illumina adaptor sequence를 제거한 후, 4,400만 개의 read를 얻었다.

- WH2와 WH3에서 차등 발현 유전자(DEG)를 확인하기 위해 featureCounts 및 edgeR을 사용하여 BH와 WH2, BH와 WH3 간의 유전자 발현을 비교했다. 

- |log2(FC)|>=2, 평균 logCPM>=1 및 FDR<=0.01로 filtering한 후, WH2 및 WH3에서 각각 249개, 906개의 DEG가 감지되었다. 

![SmartSelectImage_2022-08-02-10-45-09](https://user-images.githubusercontent.com/110142232/182274000-4c87888e-5fb3-4943-a678-2cccf25a3f48.png)

- Upregulated된 DEG 중 85개는 WH2 및 WH3에 공통적
- Downregulated된 DEG중 100개는 WH2 및 WH3에 공통적

-----------------
- DEG의 기능을 추정하기 위해 UniProtKB 데이터베이스에 대한 서열 유사성 검색을 통해 annotation을 달았다. (https://ipomoea-genome.org/)

- annotation이 된 38,788개 유전자 중 19,272개(49.7%), 32,095개(82.7%), 30,017개(77.4%) 유전자가 생물학적 과정, 세포 구성 요소 및 분자 기능에서 각각 gene onthology(GO)에 할당되었다. 

- DEG 수는 WH2와 WH3 간에 차이가 있었지만, 각 범주로 분류된 DEG의 비율은 비슷했다. 세포 성분 범주에서는 대부분 세포, 소기관, 막 및 막 부분으로 분류되었고, 분자 기능 범주에서 DEG는 주로 촉매 활성 및 결합에 있었다. 생물학적 과정의 범주에서 대사 경로는 WH2 및 WH3 DEG의 대표적인 부류였다.

----------------------
- 흰색 과육 돌연변이를 일으키는 유전자를 밝히기 위해 이전에 알려진 카로티노이드 생합성 유전자에 초점을 맞추었다. UniProtKB 및 GO의 기능적 annotation을 기반으로 카로티노이드 생합성 경로에 관여하는 유전자 69개가 확인되었다.
