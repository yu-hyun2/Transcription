# 🧠Brain MRI segmentation
[Kaggle Link](https://www.kaggle.com/datasets/mateuszbuda/lgg-mri-segmentation)

[UNet 필사 원본 링크](https://www.kaggle.com/code/tejasurya/unet-from-scratch-segmentation-tumour/notebook)

### About Dataset
LGG Segmentation Dataset
Dataset used in:

Mateusz Buda, AshirbaniSaha, Maciej A. Mazurowski "Association of genomic subtypes of lower-grade gliomas with shape features automatically extracted by a deep learning algorithm." Computers in Biology and Medicine, 2019.

and

Maciej A. Mazurowski, Kal Clark, Nicholas M. Czarnek, Parisa Shamsesfandabadi, Katherine B. Peters, Ashirbani Saha "Radiogenomics of lower-grade glioma: algorithmically-assessed tumor shape is associated with tumor genomic subtypes and patient outcomes in a multi-institutional study with The Cancer Genome Atlas data." Journal of Neuro-Oncology, 2017.

This dataset contains brain MR images together with manual FLAIR abnormality segmentation masks.
The images were obtained from The Cancer Imaging Archive (TCIA).
They correspond to 110 patients included in The Cancer Genome Atlas (TCGA) lower-grade glioma collection with at least fluid-attenuated inversion recovery (FLAIR) sequence and genomic cluster data available.
Tumor genomic clusters and patient data is provided in data.csv file.



### 📊데이터 세트 정보
LGG 세분화 데이터 세트


- 이 데이터 세트에는 수동 FLAIR 이상 분할 마스크와 함께 뇌 MR 이미지가 포함되어 있습니다.
- 이미지는 암 영상 아카이브(TCIA)에서 가져온 것입니다.
- 이 데이터는 암 게놈 아틀라스(TCGA)의 저등급 신경교종 컬렉션에 포함된 110명의 환자에 해당하며, 최소 유체 감쇠 반전 복구(FLAIR) 서열 및 게놈 클러스터 데이터를 사용할 수 있습니다.
- 종양 게놈 클러스터와 환자 데이터는 data.csv 파일로 제공됩니다.

### ✅Feature
  
- Patient: 환자 ID
- RNASeqCluster: RNA 시퀀싱 데이터 기반 군집화(cluster) 정보
- MethylationCluster: DNA 메틸레이션 데이터 기반 군집화 정보
- miRNACluster: 마이크로 RNA 데이터 기반 군집화 정보
- CNCluster: 염색체 변이 데이터 기반 군집화 정보
- RPPACluster: 복구 인자(prognostic factor) 데이터 기반 군집화 정보
- OncosignCluster: 종양 신호 데이터 기반 군집화 정보
- COCCluster: COC(cancer of unknown primary) 데이터 기반 군집화 정보
- histological_type: 조직학적 유형
- neoplasm_histologic_grade: 종양 조직학적 학점
- tumor_tissue_site: 종양 조직 사이트
- laterality: 좌우 대칭성 정보
- tumor_location: 종양 위치
- gender: 성별
- age_at_initial_pathologic: 초기 병리학적 진단 시 나이
- race: 인종
- ethnicity: 민족성
- death01: 1년 이내 사망 여부 (0: 생존, 1: 사망)

RNASeqCluster, MethylationCluster, miRNACluster, CNCluster 등은 분자 수준에서 **유전자** 발현, 메틸화, microRNA 등을 분석하여 유전적인 변화와 연관된 클러스터를 나타내는 변수입니다. 이들은 유전적인 요인이 치매 발생과 관련이 있는지를 확인할 수 있습니다.

또한 RPPACluster, OncosignCluster, COCCluster 등은 **종양학**적인 특성을 나타내는 변수입니다. 치매와 종양학적인 요인들이 연관이 있는지를 확인할 수 있습니다.

또한 histological_type, neoplasm_histologic_grade, tumor_tissue_site, laterality, tumor_location 등은 **종양 조직학**적 특성과 관련된 변수입니다. 이들은 종양이 어디서 발생했는지, 어떤 종류의 종양인지, 어느 정도의 종양 조직학적 특성을 가지고 있는지 등을 파악할 수 있습니다.

gender, age_at_initial_pathologic, race, ethnicity 등은 환자의 **인구학**적 특성을 나타내는 변수입니다. 이들은 치매 발생과 인구학적 요인들 간의 연관성을 확인할 수 있습니다.

마지막으로, death01은 사망 여부를 나타내는 변수입니다. 이를 통해 치매와 사망률 간의 연관성을 확인할 수 있습니다.
