# 1. 워드클라우드 표현


1. 마크 텍스트 클릭
2. 텍스트는 메뉴명으로
3. 색상과 크기는 칼로리로 (여기서 칼로리가 합계인 이유는 메뉴명이 가장 작은 구분 카테고리이기 때문!)


<img width="681" alt="스크린샷 2023-08-01 오후 6 11 10" src="https://github.com/hozyhozy/Tableau/assets/123252821/5e443b02-8b5a-49b0-ae16-4e504bbaae63">



# 2. 박스플롯 표현
> 박스플롯은 데이터의 분포 상태와 이상치를 동시에 보여주면서 서로 다른 데이터 군을 쉽게 비교할 수 있는 좋은 시각화
> 여러 개의 데이터를 한 눈에 표현할 수 있어 값을 비교하기에 유용


1. 열 카테고리 , 행 칼로리
2. 마크 세부사항에 메뉴명 --> 수준을 메뉴명으로 바꾸어주기!
3. 마크는 원, 색상은 카페인
4. 분석탭에서 박스플롯 드래그 화면에 놓기


<img width="818" alt="스크린샷 2023-08-01 오후 6 14 10" src="https://github.com/hozyhozy/Tableau/assets/123252821/58e7de8d-645d-4b89-8825-37dbe0984457">



<img width="232" alt="스크린샷 2023-08-01 오후 6 16 12" src="https://github.com/hozyhozy/Tableau/assets/123252821/4616e1ea-4390-4dd0-a88d-c5b045906439">


> 질문:  칼로리가 낮고 카페인이 높지 않은 메뉴를 마시고 싶다면?  답은 티바나!


# 3. 계산된 필드 만들기
> 분석에 필요한 필드가 데이터 원본에 이미 포함되어 있지 않을 경우
> 이 때, 계산된 필드를 사용하면 데이터 원본에 이미 존재하는 데이터에서 새 데이터를 만들 수 있을 뿐만 아니라 데이터에 대한 계산을 수행할 수 있음
> 이를 통해 복잡한 분석을 수행하고 데이터 원본에 고유한 필드를 즉석에서 추가 가능

### 수익률이라는 필드를 만들어봅시다


1. 계산된 필드 만들기 클릭 (만드는 법은 다양함)


<img width="212" alt="스크린샷 2023-08-01 오후 6 21 35" src="https://github.com/hozyhozy/Tableau/assets/123252821/1f4db526-6d77-4c1b-b802-282dea517898">


2. 식 넣기

   
<img width="485" alt="스크린샷 2023-08-01 오후 6 22 29" src="https://github.com/hozyhozy/Tableau/assets/123252821/0ba4cff2-bd5f-4f44-aff0-3d6f307346c3">



<img width="225" alt="image" src="https://github.com/hozyhozy/Tableau/assets/123252821/2b65dd93-c7e3-45c3-acc4-b45ee7c0dde4">


> 계산될 필드의 결과가 숫자일 경우 아이콘이 =# 라고 나타남




<img width="758" alt="스크린샷 2023-08-01 오후 6 24 11" src="https://github.com/hozyhozy/Tableau/assets/123252821/4200afa7-49b4-4044-b87b-3bc9d1877eb6">


> 계산된 필드가 수익성이 있는 것과 없는 것으로 결과를 나타낼때 아이콘은 =Abc라고 나타남



### Q. 계산식을 만들어서 평균 카페인 함유량이 80mg 보다 높은 카테고리와 아닌 카테고리를 분류해보자


<img width="1138" alt="스크린샷 2023-08-01 오후 6 28 53" src="https://github.com/hozyhozy/Tableau/assets/123252821/98204570-f955-474a-89ac-32d6f14423cd">


1. 색상을 변하게 하려면 새로 만든 계산식을 색깔에다가 드래그하기
2. 그리고 색상을 클릭하면 색상 편집이 가능!


### Q. “매장명” 별로 “매장운영시간”을 표현하고, 시도를 필터로 걸어 각 시도의 매장 별 운영 시간을 확인해보자

hint: “매장운영시간”은 “영업시작시간”과 “영업종료시간”의 차이를 계산해서 표현


ref1: https://help.tableau.com/current/pro/desktop/ko-kr/functions_functions_date.htm


ref2: https://help.tableau.com/current/pro/desktop/ko-kr/functions_functions_date.htm#datepart-%EA%B0%92


<img width="710" alt="스크린샷 2023-08-01 오후 6 33 46" src="https://github.com/hozyhozy/Tableau/assets/123252821/a809f177-d1f7-4a36-9164-25c8dd95d8c5">


<img width="697" alt="스크린샷 2023-08-01 오후 6 33 23" src="https://github.com/hozyhozy/Tableau/assets/123252821/33b614ef-e6e9-46d7-9c1e-7e08f4528d61">





