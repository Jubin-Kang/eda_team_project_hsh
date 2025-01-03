# eda-repo-3
EDA 프로젝트 3조 저장소. Home Sweet Home
<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/addinedu-ros-8th/eda-repo-3">
    <img src="https://github.com/addinedu-ros-8th/eda-repo-3/blob/main/flowermen.jpg" alt="outcome" width="350" height="250">
  </a>

  <h3 align="center">꽂보다남자 넷</h3>
  로봇 SW 개발자를 꿈꾸는 우리... 언제 집을 살 수 있을까??
  <p align="center">
    <br />
    <br />
  </p>
</p>

<hr>

## Result
|        | apt area | price | save_period | payback_period | total_period |
|--------|------|------|------|------|------|
| single   | 10평| 1억1천| 10.6개월| 10년|10년10.6개월 
| Married   | 25평| 8억| 35.6개월| 30년| 32년11.6개월       
- 원리금균등상환으로 10년 갚는데 매달 갚는 비용 (850,953원)
  - 10년간 이자비용 (14,114,446원)
- 원리금균등상환으로 30년 갚는데 매달 갚는 비용 (2,725,560원)
  - 30년간 이자비용 (337,201,895원)
## Intro 
경기도 성남시는 한국의 IT 및 로봇 산업의 중심지로, 많은 로봇 소프트웨어 프로그래머들에게 꿈의 직장으로 꼽히는 지역입니다. 하지만 그 지역의 집값은 여전히 높아, 이곳에서 집을 마련하는 것은 현실적으로 큰 도전 과제가 됩니다. 본 프로젝트는 로봇 소프트웨어 프로그래머가 성남시로 출퇴근이 가능한 주변 지역(성남, 용인, 과천 등)에서 집을 사는 데 얼마나 걸릴지를 데이터 기반으로 분석합니다. 다양한 요인을 종합적으로 분석하여 집을 사는 데 필요한 기간과 현실적인 재정 전략을 제시합니다.
 
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
- folium: Folium은 Python에서 지도를 생성하고 시각화하기 위한 라이브러리입니다.
```
  pip install pandas
  pip install selenium 
  pip install matplotlib 
  pip install seaborn 
  pip install beautifulsoup
  pip install folium
```
## Responsibility
|        | name | job |
|--------|------|-----|
| leader | 남상기 |  크롤링 및 분석, 발표자료준비|   
| worker | 강주빈 |  DB 구축 및 관리, 발표 준비 및 발표|   
| worker | 황한문 |  데이터분석, 프로젝트 서포트|    
| worker | 임동욱 |  통계자료 수집 및 시각화|   

## Data collection

### References 
|        | DATA | 
|--------|------|
| SITE   | 사람인, 잡코리아, 통계청, 은행연합회 소비자포털, 국토교통부 실거래가,NAVER API| 
| DATA   | 연봉, 부동산가격, 주거형태, 금리, 이동거리|        
         
### ER-Diagram 
![ER-Diagram](https://github.com/user-attachments/assets/0dc1663b-5592-4232-8309-e69d2646c212)

## Exploratory Data Analysis (EDA)
### 로봇 회사들은 주로 어디에 위치에 있는가? 🤖
![회사밀집지역](https://github.com/user-attachments/assets/feb36962-e257-474a-8d30-f2bb47ab8956)

- 현재 가장 많이 분포한 지역은 성남, 대전,  인천, 경남, 부산 순서
#### 여러 로봇회사의 밀집지역들 중 선호하는 지역은? 
![성남이좋은이유](https://github.com/user-attachments/assets/d0a45d66-2664-4d20-a1a6-13303679c3c5)

- 이러한 이유로 우리는 '성남'을 선정하였다

### 일하게 된다면 어떤 주거형태에 거주할까? 🤔 
![주거유형](https://github.com/user-attachments/assets/80bf3e54-c89c-4c03-afab-04850a7746d7)
![주거유형비율](https://github.com/user-attachments/assets/a8e7daad-0235-4d0e-97b0-9fdc609035fa)
- 본격적으로 구매를 시작하는 시기인 30대이후로 주거형태는 '아파트'의 비율이 가장 높았음.
### 아파트를 산다면, 몇평대를 사야할까?🏠 그 전에....
![미혼과기혼](https://github.com/user-attachments/assets/35e88cbf-7a0c-4be7-9fa6-f3a7435c95d8)
- 본격적으로 아파트를 구매하는 시기는 가구원의 수가 변하는 시기이도 합니다.❤️❤️ 

![평수](https://github.com/user-attachments/assets/2d842b7a-1a54-4d2e-8842-05b053e7610c)

- 1인가구의 경우 현실적으로 $40m^2$이하 즉, 10평대에 대다수 거주
- 2인가구 이상의 경우 $60-85m^2$ 즉, 25평대에 대다수 거주

### 회사근교는 너무 비싸, 출퇴근이 가능하고 싼 지역은 어디에 있을까? 🤔  
![레이더망](https://github.com/user-attachments/assets/5420946f-119a-4ebb-8b24-9bfe2f030034)
- 일단 서울은 규격외의 집값 수준을 보이기에 제외
- 회사지역을 중심으로 주변 지역들이 많이 있었음 

#### 거리상 가까운 지역들은 어디 있을까? 
NAVER 맵-길찾기 API를 사용한 결과, 자동차출퇴근 거리를 살펴보면
- 용인시: 15,951 meters
- 안양시: 20,301 meters
- 의왕시: 20,675 meters
- 과천시: 20,874 meters
- 광주시: 20,965 meters
- 군포시: 22,918 meters
- 수원시: 23,119 meters
- 하남시: 26,186 meters
- 광명시: 33,012 meters
- 이천시: 42,957 meters

#### 가까운지역 OK👌, 그러면 싼지역은 ...? 
![싼지역](https://github.com/user-attachments/assets/440176f0-0cf0-4b25-92f1-df98bee54751)
- 이천, 광주, 군포, 수원 등 순으로 아파트가격대 조사하였음.  

#### 가격과 거리가 합리적인 지역을 조사해 본다면
- 2번째로 싼지역이면서, 5번째로 가까운 지역은 **광주** 였음 ! 

#### 해당 지역의 우리가 원하는 가격은 얼마지?  
|   전용면적  | 20~25평대 | 10평대이하 |
|--------|------|-----|
| 평균금액(만원) | 40230 |  13577|
### 지역과 평수를 결정했다면, 구매하기 까지 고려해야할 것?
- 세금
  ![국세청_세금](https://github.com/user-attachments/assets/6b060e99-88f4-4da8-84bd-672e2a880f59)
- 예금이자
  ![예금이자](https://github.com/user-attachments/assets/83a264b2-067c-47c1-b13b-a06277d37bea)
- 주택담보대출이자
  ![주담보](https://github.com/user-attachments/assets/09bd6991-2265-4a8e-b0cd-c82870634b1d)
- 생활비
  ![image](https://github.com/user-attachments/assets/1b6926b5-d281-421c-aecf-91d89ed44d1d)


 
## Project Schedule
Project Period: 2024.12.26~2025.01.03
![Screenshot from 2025-01-03 12-14-27](https://github.com/user-attachments/assets/9e7cb741-095a-40fd-8d33-8c28dd6634e4)
