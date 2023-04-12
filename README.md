# 강서구, 광진구 주차 문제 해결 프로젝트
- 동 시간대 진행된 공모전 참가, 이하 코드 및 프로젝트 개요 서술.
- 강서구 : https://www.gangseo.seoul.kr/reserve/re040101/view?aplySn=44&curPage=1
- 광진구 : https://gwangjin.go.kr/portal/bbs/B0000003/view.do?nttId=6034623&menuNo=200192
## DSL 23-1 Modelling Project F조 - 광진구 정리 repository
**팀원** : 백민준, 손승진, 이승원

**역할 분담** 
- 백민준 : 데이터 전처리, 시계열 예측, 발표
- 손승진 : 데이터 전처리, 시계열 예측
- 이승원 : 데이터 전처리, ppt 제작, 폴리움 시각화


## Overview
---

**1. 개요**
- Background:
  - 서울특별시 민원 수는 매년 일정한 반면 서울특별시 불법주차 민원 수는 꾸준히 증가하고 있는 상황
  - 사망 사고, 소방 대응 취약으로 이어질 수 있는 불법 주정차 문제 해결
- 기획 내용(스토리보드)
![image01](image01)

**2. 데이터 확보**
- 주차장 데이터
  - 서울특별시 주차장 확보율 데이터
  https://data.seoul.go.kr/dataList/10357/S/2/datasetView.do
  - 서울특별시 주차정보안내시스템 데이터 (주차면 수, 위치 크롤링)

- 인구 데이터
  - 주민등록 인구 및 세대 현황 데이터
  https://jumin.mois.go.kr/
  - 행정동 단위 서울 생활인구(내국인) 데이터 
  https://data.seoul.go.kr/dataList/OA-14991/S/1/datasetView.do

- 불법주차 단속 데이터
  - 서울특별시 광진구 주차단속 현황 데이터
  https://www.data.go.kr/data/15034487/fileData.do
  - 서울특별시 광진구 불법주정차 위반 단속 CCTV 위치정보 데이터
  https://data.seoul.go.kr/dataList/OA-20476/S/1/datasetView.do

- 참고문헌 : 
  - 서울시 주차문제 해결을 위한 주차장 이용효율 향상 연구, 2020, 서울디지털재단
  
  **3. 데이터 전처리**
- 월별, 분기별 단속 수, 생활 인구, 주민등록 인구, 등록차량대수, 주차면수 데이터를 이용해 주차 수요 예측
- 데이터 전처리를 통해 폴리움 시각화 진행

**4. Pipeline**

- 불법 주정차 문제의 심각성 

- Folium 시각화와 클러스터링을 통한 광진구 현황 파악

- 팀 내에서 도출한 식을 이용해 행정동별 주차 수요 예측 진행 (월별, 분기별)

- 불법주차 해결 방안 제안(공급 정책, 공유 정책, 올파킹)

**5. 맺음말**


# 프로젝트의 가치
- 팀 내에서 자체적으로 도출한 식을 이용해 주차 수요 예측 진행
- 불법 주차 해결 가능 서비스 예시 제시
- 현실적인 주차장 확보율 고려


# End-to-End Inference
---
월별 주차 수요 예측을 통한 주차 솔루션 제시

### Dependencies
- google colab
