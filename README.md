## 2017 빅데이터 아카데미 제조 빅데이터 분석 파일럿 프로젝트 1조

### 데이터/ 소스코드/ RMarkdown/ 시각화 자료 등을 여기서 관리해 보세요  


> 폴더는 다음과 같이 분류하면 좋습니다


|<center>폴더명</center>|<center>폴더 내용</center>|
|:------------:|:--------------------------------------:|
|data|데이터 소스를 담는 폴더|
|script|R 소스 코드를 담는 폴더|
|img|시각화 파일을 담는 폴더|
|RMD|RMarkdown을 담는 폴더|

***

> 1조 데이터 분석 개요

* 개요 : 한국수자원 공사에서 제공하는 경기도 지역 정수장 Data (공공)
* Data 주기 : 1시간 단위 (2016년 1년간 Data 분석 예정, 8460 rows)
* 변수 종류
  + 발생일시 : 년 / 월 / 일 / 시
  + 시설명 : 8개소 (고양/덕소/반월/성남/수원/수지/시흥/와부/일산)
  + 수위 : 정수장 내 수위 (m, 정수장 별 2~3개 tag)
  + 압력 : 정수장 유입 원수에 대한 유입 압력 (kg/cm2)
  + 유량 : 공업/생활 유출수에 대한 유량 (m3/h, 정수장 별 2~3개 tag)
  + 유량 적산차 : 시간별 유출되는 유출수의 volume (m3, 정수장 별 2~3개 tag)
  + pH : 용수의 pH 측정값 (Control Range : 5.8 ~ 8.5)
  + 탁도 (NTU) : 용수의 탁도 측정값 (Control Range : 0.5 이하)
  + 잔류염소 (mg/L) : 용수의 잔류염소 측정값 (Control Range : 0.1 ~ 4.0)
* 활용 Data
  + 수질 Data : 탁도, 잔류염소 (낮을수록 우수한 품질)
* pH는 잔류염소와 강한 상관관계가 있어 제외하여도 무관한 것으로 판단되며,Control Range 이내로 관리하면 되고 측정값 중 우수한 값을 정의할 수 없음  
  + Variables : 압력 / 수위 / 유량 / 유량적산차
  + 외부 Data 활용 : 수원 지역 일별 강수량 Data

***

> 프로젝트 발표자료 작성 내용

* 프로젝트 개요
  + 배경 및 목적
  + 기대효과
  + 수행일정
* 데이터의 이해
  + 데이터 선정 및 수집방법
  + 데이터 정제: 이상치, 결측치 제거, 변수 분류 등
  + 탐색적 데이터 분석: 기초 통계 (분포, 상관분석, 의사결정 나무 등)
* 데이터 모델링
  + 분석 방법: 나무모형, 회귀분석, 시계열 분석,랜덤 포레스트, k-NN, 뉴럴넷
  + 분석 결과
* 데이터 시각화
  + 시각화 방법
  + 시각화 결과
* 결론
  + 프로젝트를 통한 시사점
  + 향후 발전 방향

***

> `데이터 분석`을 위한 참고 자료
- [R에서 자유자재로 데이터 가공하기](http://rpubs.com/jmhome/R_data_wrangling)
- [R에서 데이터 정제하기 (결측치,이상치)](http://rpubs.com/jmhome/R_data_processing)
- [R에서 통계기법을 이용한 가설 검정](http://rpubs.com/jmhome/StatisticalAnalysis)
- [R에서 한글문서 열때 인코딩 문제 해결](http://philogrammer.com/2017-03-15/encoding)

> `데이터 시각화`를 위한 참고 자료
- [샤이니 보드를 활용한 Interactive Chart 구현](https://www.slideshare.net/r-kor/ruck-2017-interactive-chart)
- [샤이니 보드 심플 예제](https://yihui.shinyapps.io/DT-rows/)
- [R Shiny를 이용한 데이터 시각화](https://rstudio.github.io/shinydashboard/index.html)
- [R을 위한 대화형 대시보드 제작](http://rmarkdown.rstudio.com/flexdashboard/)
- [R을 위한 다이나믹 차트 구현](http://rstudio.github.io/crosstalk/)
- [JavaScript 데이터 시각화를 R과 연동](http://www.htmlwidgets.org/)

> 기타 유용한 참고 자료
- [R 코딩 스타일 가이드](http://rpubs.com/jmhome/R_CodingStyle)

