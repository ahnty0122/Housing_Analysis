세종시 주택 시장 특성 분석  
==========    
  
## 세종시 주택 시장 특성을 쉽고 명확히 보이도록 시각화

### __사용 Tool__
- Tableau
- Python (jupyter notebook)

### __1. join_code.ipynb__
- __사용한 데이터__
1. 세종시 상업업무용 실거래가
2. 세종시 토지 실거래가
3. 세종시 분양권 실거래가
4. 세종시 지역코드 데이터
- __Goal__  
상업업무용 실거래가 데이터, 세종시 토지 실거래가 데이터,  세종시 분양권 실거래가 데이터에
공간 데이터와 매칭시키기 위해 주소체계(지역코드) 생성 (외부 데이터 이용)

### __2. join_data.ipynb__
- __사용한 데이터__
1. 세종시 아파트 매매 실거래가
2. 세종시 연립다세대 매매 실거래가
3. 세종시 단독다가구 매매 실거래가
4. 세종시 오피스텔 매매 실거래가
5. 세종시 아파트 전월세 실거래가
6. 세종시 연립다세대 전월세 실거래가
7. 세종시 단독다가구 전월세 실거래가
8. 세종시 오피스텔 전월세 실거래가
9. 세종시 지역코드 데이터
- __Goal__  
아파트, 연립다세대, 단독다가구, 오피스텔 실거래가 데이터
한 파일로 합친 후 공간 데이터와 매칭시키기 위해 주소체계(지역코드) 생성 (외부 데이터 이용)

- __시각화__  
1. 아파트 매매 데이터  

<img width="800" alt="아파트매매시장" src="https://user-images.githubusercontent.com/61795757/112185869-f7061300-8c43-11eb-8d04-a73b2d43d045.png">

2. 아파트 전세 데이터

<img width="800" alt="아파트전세시장" src="https://user-images.githubusercontent.com/61795757/112186224-464c4380-8c44-11eb-99cc-07bcb85a4ffe.png">

3. 주택 매매 전체 현황

<img width="800" alt="주택매매전체" src="https://user-images.githubusercontent.com/61795757/112186594-a5aa5380-8c44-11eb-9777-0fc2f5680aef.png">

4. 주택 전/월세 현황

<img width="800" alt="주택월세,전세" src="https://user-images.githubusercontent.com/61795757/112186931-f28e2a00-8c44-11eb-94e8-203551caff9a.png">

### __3. code_name_merge.ipynb__
- __사용한 데이터__
1. 세종시 도로명주소 건물
2. 코드정의서

- __Goal__  
세종시 도로명 주소 건물 파일에서 건물 코드와 건물 구분 코드를 코드명으로 명시

- __시각화__  
<img width="800" alt="도로명주소건물" src="https://user-images.githubusercontent.com/61795757/112185178-53b4fe00-8c43-11eb-8da6-cbcd8cf5616f.png">

### __4. population_preprocess.ipynb__
- __사용한 데이터__  
세종시 연령별 인구현황


- __Goal__  
지역별+연령대별로 동별인구수/세종시인구수의 추이를 새로운 데이터프레임으로 만들어 시각화 하기 좋게 만들고자 함

- __시각화__
<img width="800" alt="인구현황" src="https://user-images.githubusercontent.com/61795757/112186321-59f7aa00-8c44-11eb-8a12-d1517c6244e0.png">

### __5. 세대구성_preprocess.ipynb__
- __사용한 데이터__  
세종시 지역별 세대원수별 세대수


- __Goal__  
읍면동 + 세대구성 별로 새로운 기준의 데이터프레임을 만들어 시각화 하기 좋게 만들고자 함


- __시각화__  
<img width="800" alt="세대현황" src="https://user-images.githubusercontent.com/61795757/112185734-db027180-8c43-11eb-9aaa-4e93cf03154b.png">

### __6. 매매_분양권비교.ipynb__
- __사용한 데이터__  
1. 세종시 주택 거래 매매 데이터 (join_data.ipynb 사용 후)
2. 세종시 분양권 거래 데이터 (join_code.ipynb 파일 사용 후)

- __Goal__  
같은 유형의 주택에 대해 매매와 분양권 거래 추이를 비교해보고자 매매 데이터와 분양권 거래 데이터 MERGE


### __7. 매매_전월세비교.ipynb__
- __사용한 데이터__  
1. 세종시 주택 거래 매매 데이터 (join_data.ipynb 사용 후)
2. 세종시 주택 거래 전월세 데이터 (join_data.ipynb 사용 후)


- __Goal__  
같은 유형의 주택에 대해 매매와 전월세 추이를 비교해보고자 매매 데이터와 분양권 거래 데이터 MERGE

- __시각화__
<img width="800" alt="전세가격추이" src="https://user-images.githubusercontent.com/61795757/112186417-7562b500-8c44-11eb-9b68-dac596d457e0.png">

- - -
- - -
### Contributor
- __Data Preprocessing__: 안태영 [![Instagram Badge](http://img.shields.io/badge/-Instagram-white?style=flat&logo=Instagram&link=https://instagram.com/_tae.0_/=https://instagram.com/_tae.0_/)](https://instagram.com/_tae.0_) 
- __Data Visualization__: 안진영 [![Instagram Badge](http://img.shields.io/badge/-Instagram-white?style=flat&logo=Instagram&link=https://instagram.com/_tae.0_/=https://instagram.com/1004jin0/)](https://instagram.com/1004jin0)