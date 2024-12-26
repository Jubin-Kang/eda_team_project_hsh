# eda-repo-3
EDA 프로젝트 3조 저장소. home sweet home

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/addinedu-ros-8th/eda-repo-3">
    <img src="https://github.com/addinedu-ros-8th/eda-repo-3/blob/main/flowermen.jpg" alt="outcome" width="350" height="250">
  </a>

  <h3 align="center">꽂보다남자 넷</h3>

  <p align="center">
    로봇 SW 프로그래머는 몇년안에 집을 장만 할 수 있을까 ?
    <br />
    <br />
  </p>
</p>

<hr>

## Preview  


## Intro 
판교는 한국의 IT 및 로봇 산업의 중심지로, 많은 로봇 소프트웨어 프로그래머들에게 꿈의 직장으로 꼽히는 지역입니다. 하지만 판교와 그 주변 지역의 집값은 여전히 높아, 이곳에서 집을 마련하는 것은 현실적으로 큰 도전 과제가 됩니다.
본 프로젝트는 로봇 소프트웨어 프로그래머를 가상의 주인공으로 설정하고, 그가 판교 및 출퇴근 가능한 주변 지역(성남, 용인, 과천 등)에서 집을 사는 데 얼마나 걸릴지를 데이터 기반으로 분석합니다.
다양한 요인을 종합적으로 분석하여 집을 사는 데 필요한 시간과 현실적인 재정 전략을 제시합니다
### Scenario
로봇 소프트웨어 프로그래머로 최근 취직의 성공한 20~30대 사회초년생 
이름: 김철수 
나이: 30세 
직업: 로봇 SW 개발자 
연봉: 개발자 사회 초년생 평균 연봉 
소망: 회사와 출퇴근 가능한 지역에서 거주할 집을 매매 
조건: 
1. 부동산 
- 전용면적 85제곱미터 이하()
- 지역별 평균 매매가 기준

2. 제정 
- 생활비 제외 (식비나 교통비등은 개인마다 편차가 큼)
- 연봉 상승률 제외 

3.
- 대출 및 저축을 병행하여 집을 사는 데 걸리는 시간을 계산   
- 지역별 걸리는 시간
- ㅈ
## Insructions
### Environment   
- Dev: Jupyter Notebook - Python  
- DB: AWS RDS - MySQL
- Collab: Jira, Confluence and Slack   

### Installation 
#### Linux
Dependencies include `seaborn 0.13.2`, `selenium 4.27.1`, `beautifulsoup4 4.12.3`, `pandas 2.2.3`
```
  git clone https://github.com/addinedu-ros-8th/eda-repo-3.git
  code eda-repo-3  
```
#### Libraries Used
- Selenium: 웹 애플리케이션 자동화 및 테스트를 위한 포터블 프레임워크 
- BeautifulSoup: HTML과 XML 문서들의 구문을 분석하기 위한 파이썬 패키지
- Pandas: 데이터 조작 및 분석을 위한 파이썬 프로그래밍 언어 용으로 작성된 SW 라이브러리
- Seaborn: Matplotlib을 기반으로 다양한 색상 테마와 통계용 차트 등의 시각화 패키지
- Matplotlib: Python 프로그래밍 언어 및 수학적 확장 NumPy lib를 활용한 플로팅 라이브러리.


## Responsibility
|        | name | job |
|--------|------|-----|
| leader | 남상기 |  크롤링 및 분석, 발표준비|   
| worker | 강주빈 |  DB 구축 및 관리 |   
| worker | 황한문 |  데이터분석, 프로젝트 서포트|    
| worker | 임동욱 |  통계자료 수집 및 시각화 |   

## Data collection

### References 
|        | DATA | 
|--------|------|
| SITE   | 사람인 |        
| DATA   | 연봉, 부동산가격, 주거형태  |        
         
### ER-Diagram 
<img src="https://github.com/addinedu-ros-8th/eda-repo-3/blob/main/Home Sweet Home.jpg" alt="outcome" width="250" height="350">
<p align="center">
- 기업-사람 연관성을 조회할 수 있도록 join database 설계 
  <br />
</p>

## Exploratory Data Analysis (EDA)
### 로봇 회사들은 주로 어디에 위치에 있는가?
### 사회 초년생의 주거형태는 주로 무엇인가? 
### 매매지역과 월세지역별로 주거의 형태가 다른가 ?
### 빠르게 부채를 상환하는 법, 저축 vs 투자 
### 위치별 매매가격 차이 

## Project Schedule

## Review