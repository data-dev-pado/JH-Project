Netflix 콘텐츠 분석: 데이터 기반 인사이트와 트렌드

# **1. 프로젝트 개요**

목적: Netflix 콘텐츠 데이터 분석을 통한 인사이트 도출

데이터셋: Netflix 영화 및 TV 쇼 정보

사용한 기술 : Python, Pandas, Matplotlib, Seaborn, WordCloud

# **2. 데이터 전처리**

결측치 처리: 'country', 'cast', 'director' 열의 NaN 값을 'No Data'로 대체

날짜 데이터 변환: 'date_added' 열을 datetime 형식으로 변환

연령 그룹 매핑: 'rating'을 기반으로 'age_group' 열 생성

# 3.탐색적 데이터 분석 EDA

## **3.1 콘텐츠 유형 분석**

영화와 TV 쇼의 비율 시각화 (파이 차트, 막대 그래프)

인사이트: 영화가 69%, TV 쇼가 31%를 차지

## **3.2 연령 그룹별 콘텐츠 분포**

연령 그룹별 콘텐츠 수 분석

주요 발견: 성인 대상 콘텐츠가 가장 많음 (4,089개)

## **3.3 시간에 따른 콘텐츠 추가 트렌드**

연도별 콘텐츠 추가 추이 분석 (스택 막대 그래프)

월별 콘텐츠 추가 패턴 분석

인사이트: 2019년에 가장 많은 영화 추가, 연중 일정하지 않은 추가 패턴

## **3.4 국가별 및 연령대별 콘텐츠 선호도**

히트맵을 통한 국가별, 연령대별 콘텐츠 선호도 시각화

주요 발견: 국가와 연령대에 따른 뚜렷한 선호도 차이

## **3.5 장르 분석**

연령 그룹별 상위 10개 장르 분석

인사이트: 연령 그룹에 따른 장르 선호도 차이 확인

## **4. 텍스트 분석**

WordCloud를 활용한 Netflix 콘텐츠 키워드 시각화

주요 키워드 및 트렌드 파악

***
Movie (영화 산업 데이터 분석)
## **프로젝트 개요**

TMDB 영화 데이터셋을 활용하여 영화 산업의 트렌드와 성공 요인을 분석했습니다. 주요 분석 내용으로는 연도별 흥행 수익, 최고 흥행 영화, 성공한 감독과 배우, 그리고 장르별 수익 분포 등이 포함됩니다.

## 프로젝트에 사용된 기술

Python
데이터 분석: Pandas, NumPy
데이터 시각화: Matplotlib, Seaborn, Plotly Express
데이터 처리: ast (Abstract Syntax Trees)

## 데이터 전처리

필요한 컬럼 선택 및 데이터 병합
ROI(Return on Investment) 컬럼 생성
감독 정보 추출 및 컬럼 생성
출연 배우 정보 추출 및 컬럼 생성
주요 장르 추출 및 컬럼 생성
날짜 데이터 타입 변환 및 연도, 월 컬럼 생성
결측치 처리

## **분석 결과**

## **1. 연도별 흥행 수익 분석**

Insight : 

2000년대 이후 영화 흥행 수익이 급격히 증가하는 추세입니다

2016년까지의 데이터 분석 (최신 데이터 날짜: 2016-09-16)

## **2. 최고 흥행 영화 Top 10**

Insight : 

'Avatar', 'Star Wars: The Force Awakens' 등이 상위권에 랭크

블록버스터 영화들의 압도적인 흥행 성과 확인

## **3. 성공한 감독과 배우 분석**

Insight :

감독: Steven Spielberg, Peter Jackson 등이 높은 흥행 수익 기록

배우: Robert Downey Jr., Scarlett Johansson 등이 높은 흥행 수익과 연관

## **4. 장르별 수익 분포 분석**

Insight :

액션, 어드벤처 장르가 전반적으로 높은 수익을 보입니다.

애니메이션, 가족 영화 장르도 평균적으로 높은 수익을 기록했습니다. 

장르별 평균 수익 순위: 애니메이션 > 어드벤처 > 가족 > SF > 판타지 > 액션

## **추가 분석**

- 예산과 흥행 수익의 관계
- 투표수와 흥행 수익의 관계
- 연도별, 월별 장르 트렌드 변화

## **결론**

대규모 예산의 블록버스터 영화들이 흥행을 주도하고 있습니다. 특정 유명 감독과 배우들의 영향력이 큰 것으로 나타났으며, 장르별로는 액션, 어드벤처, 애니메이션 등이 높은 수익을 올리고 있습니다. 2000년대 이후 전반적인 영화 산업의 규모가 크게 확대되었습니다.

***
Traffic (서울 지하철 승하차 데이터 분석)
## **프로젝트 개요**

**언어**: Python

**라이브러리**: pandas, numpy, matplotlib, seaborn, plotly, scikit-learn

본 프로젝트는 서울 지하철 노선의 승하차 데이터를 분석하여 유의미한 인사이트를 도출하는 것을 목표로 합니다. 시간대별, 역별 승하차 패턴을 파악하고 클러스터링을 통해 역들의 특성을 분류했습니다.

## **데이터 소개**

**데이터 출처**: 서울시 지하철 호선별 역별 시간대별 승하차 인원 정보 (https://data.seoul.go.kr/dataList/OA-12252/S/1/datasetView.do)

**주요 변수**: 사용월, 연도, 월, 지하철역, 시간대별 승차인원

## **데이터 전처리**

결측치 및 이상치 처리

시간대별 데이터 통합

연도 및 월 변수 생성

## **탐색적 데이터 분석 (EDA)**

역별 평균 승차인원 분석

연도별, 월별 승차인원 추이 분석

시간대별 승차패턴 분석

## **고급 분석**

K-means 클러스터링을 통한 역 유형 분류

엘보우 방법을 통한 최적 클러스터 수 결정

# Insight

## **1. 승차인원 상위 역**

상위 5개 역의 월평균 승차인원

1. 강남: 2,627,498명
2. 잠실: 2,334,455명
3. 홍대입구: 2,057,443명
4. 신림: 1,906,915명
5. 구로디지털단지: 1,731,064명

## **2. 연도별 승차인원 추이**
2015년부터 2019년까지 꾸준히 증가하는 추세를 보였습니다.
2020년에 급격한 감소가 있었으며, 이는 COVID-19 팬데믹의 영향으로 추정됩니다.
2021년부터 점진적인 회복세를 보이고 있습니다.

## **3. 시간대별 패턴**
대부분의 역에서 오전 8-9시, 오후 6-7시에 피크가 관찰됩니다.
강남, 삼성 등 업무지구 역들은 오후 피크가 더 높게 나타납니다.

## **4. 역 클러스터링 결과**
K-means 클러스터링 결과, 3개의 뚜렷한 클러스터가 발견되었습니다:
**클러스터 0 (업무지구 중심)**: 강남, 삼성, 역삼, 을지로입구 등
**클러스터 1 (주거지역 중심)**: 구로디지털단지, 신림, 서울대입구 등
**클러스터 2 (복합지역)**: 잠실, 홍대입구, 건대입구 등

## **결론**

2호선은 서울의 주요 업무 및 상업지구를 연결하는 노선이라는 사실이 명확합니다. 
COVID-19 팬데믹의 영향이 뚜렷하게 관찰되며, 지속적인 회복 추세 모니터링이 필요합니다.
역별 특성에 맞는 맞춤형 서비스 제공을 고려해볼 수 있습니다. 
향후에는 날씨, 주요 이벤트 등 외부 요인과 관련지어서 연관성 분석을 할 수 있습니다.


