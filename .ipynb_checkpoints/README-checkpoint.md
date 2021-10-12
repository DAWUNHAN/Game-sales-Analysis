# Game-sales-Analysis

- 다음 분기 설계할 게임을 위해 게임 출고량 데이터를 분석합니다. 
- [PPT 파일 정리](https://da-journal.com/entry/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EA%B2%8C%EC%9E%84-%EC%84%A4%EA%B3%84%EB%A5%BC-%EC%9C%84%ED%95%9C-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EB%B6%84%EC%84%9D)

## 데이터 전처리
- 데이터셋 크기 : 16598 * 9 
- 데이터 전처리 
    - 데이터 크기가 유독 작은 2017, 2020년은 유의미한 분석이 어려우므로 삭제
    - 총 판매량을 계산하기 위해 Total 컬럼 추가
    - 출고량 컬럼의 단위를 K로 통일 한다.
    - 연도 변경
        - 20 이하는 +2000
        - 20 초과 100 미만은 +1900
        
![df](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/df.png?raw=true)


## 연도별 게임의 트렌드 존재 여부
### 연도에 따른 장르별 판매량 (라인 그래프)
![연도에 따른 장르별 판매량](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%97%B0%EB%8F%84%EB%B3%84%20%EA%B2%8C%EC%9E%84%20%EC%9E%A5%EB%A5%B4%20%ED%8A%B8%EB%A0%8C%EB%93%9C.png?raw=true)

### 연도에 따른 각 지역별 출고량 (라인 그래프)
![연도에 따른 각 지역별 출고량](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%97%B0%EB%8F%84%EC%97%90%20%EB%94%B0%EB%A5%B8%20%EC%A7%80%EC%97%AD%EB%B3%84%20%EC%B6%9C%EA%B3%A0%EB%9F%89.png?raw=true)

### 연도에 따른 게임 판매량 vs. 넷플릭스 수익
- 대표적인 Indoor Activity인 게임과 넷플릭스는 서로 관계가 있을까?
![연도에 따른 게임 판매량과 넷플릭스 수익](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EA%B2%8C%EC%9E%84%20%EC%B6%9C%EA%B3%A0%EB%9F%89%EA%B3%BC%20%EB%84%B7%ED%94%8C%EB%A6%AD%EC%8A%A4%20%EC%88%98%EC%9D%B5%20%EB%B9%84%EA%B5%90.png?raw=true)

### 연도에 따른 탑10 플랫폼별 판매량 그래프
![](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%97%B0%EB%8F%84%EC%97%90%20%EB%94%B0%EB%A5%B8%20TOP10%20%ED%94%8C%EB%9E%AB%ED%8F%BC%EB%B3%84%20%ED%8C%90%EB%A7%A4%EB%9F%89.png?raw=true)

### 시대별 (10년 단위) 게임 장르 트렌드
![](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EA%B0%81%20%EC%8B%9C%EB%8C%80%EC%9D%98%20%EA%B2%8C%EC%9E%84%20%EC%9E%A5%EB%A5%B4%EB%B3%84%20%ED%8C%90%EB%A7%A4%EB%9F%89%20scatter.png?raw=true)

![](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EA%B0%81%20%EC%8B%9C%EB%8C%80%EC%9D%98%20%EA%B2%8C%EC%9E%84%20%EC%9E%A5%EB%A5%B4%EB%B3%84%20%ED%8C%90%EB%A7%A4%EB%9F%89.png?raw=true)


## 출고량이 높은 게임에 대한 분석

### TOP 30 게임의 장르별 판매량
![TOP 30 게임의 장르별 판매량](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/TOP%2030%20%EA%B2%8C%EC%9E%84%EC%9D%98%20%EC%9E%A5%EB%A5%B4%EB%B3%84%20%ED%8C%90%EB%A7%A4%EB%9F%89.png?raw=true)

### TOP 30 플랫폼에 따른 판매율
![TOP 30 플랫폼에 따른 판매율](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/TOP%2030%20%ED%94%8C%EB%9E%AB%ED%8F%BC%EC%97%90%20%EB%94%B0%EB%A5%B8%20%ED%8C%90%EB%A7%A4%EC%9C%A8.png?raw=true)


## 지역에 따른 게임 출고 분석

### 지역별 게임 장르 판매량
![지역별 게임 장르 판매량](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%A7%80%EC%97%AD%EB%B3%84%20%EA%B2%8C%EC%9E%84%20%EC%9E%A5%EB%A5%B4%20%ED%8C%90%EB%A7%A4%EB%9F%89.png?raw=true)

### 각 지역별 총 판매량을 지도 위에 표시하기
![각 지역별 총 판매량](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%A7%80%EC%97%AD%EB%B3%84%20%EA%B2%8C%EC%9E%84%20%EC%B6%9C%EA%B3%A0%EB%9F%89%20%EB%B9%84%EA%B5%90.png?raw=true)


## 게임 장르와 플랫폼의 연관 관계

- Two-sample Chi-square Test를 통해 서로 독립인지 수치적으로 확인

## 게임 이름을 Wordcloud로 표현

![Wordcloud로](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/wordcloud.png?raw=true)

## 스포츠 게임과 스포츠 대회 상관 관계
![](https://github.com/DAWUNHAN/Game-sales-Analysis/blob/master/image/%EC%8A%A4%ED%8F%AC%EC%B8%A0%20%EA%B2%8C%EC%9E%84%20%EC%B6%9C%EA%B3%A0%EB%9F%89%EA%B3%BC%20%EB%8C%80%ED%9A%8C%20%EA%B0%9C%EC%B5%9C%20%EC%97%AC%EB%B6%80%20%EB%B9%84%EA%B5%90.png?raw=true)
