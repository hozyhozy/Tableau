# 필드 구분
1. 차원: 정성적인 값 (제품명, 날짜, 지리명 등...) 불연속형 데이터로 측정값을 쪼개어 보는 하나의 관점
2. 측정값: 정량적인 값 / 연속형 데이터로 집계가 되는 데이터


# 측정값은 차원을 기준으로 집계되어 표현된다
> 집계란? 합계, 평균, 중앙값, 카운트, 카운트 (고유), 최소값, 최대값, 백분위수, 표준편차, 분산등을 의미
> 측정값을 화면에 가져다 놓으면 기본적으로 합계 값을 보여줌


### 집계형태를 변경해주는 방법
1) 행 또는 열, 마크 선반에 놓여진 알약에서 마우스 오른쪽 버튼 클릭 후 측정값의 집계 형태를 변경


2) 측정값을 가져올 때부터 집계 형태를 변경


- Windows : 측정값에서 마우스 오른쪽 버튼을 누른 상태로 드래그


- Mac :  Option키 누른 상태로 드래그


1. 필드를 **행 선반에 놓으면 Y축**에 표현, **열 선반에 놓으면 X축**에 표현
2. 마크 선반에 있는 마크의 형태, 색상, 크기, 레이블, 세부 정보, 도구 설명, (경로, 각도, 모양) 속성을 통해 원하는 형태로 다양한 시각화 표현
3. 필요한 값은 필터 선반을 통해 필터링 ( **[데스크탑 UI 구성 요소: 용어 해설](https://www.notion.so/8a4b21a9737e4bfbb4d5d97219adeb4d?pvs=21)** 문서를 참고하세요.)
4. 대시보드는 기존에 만들어 놓은 워크시트를 조합하여 만듦


# 과제 1
### Q1. 음료 카테고리별 칼로리와 카페인 시각화
1. 칼로리와 카페인을 가져올때 평균값으로 집계한다. 
2. 색을 지정하고 싶다면 마크의 색상에 원하는 값을 드래그하면 된다. 

![스크린샷 2023-07-24 오후 9 05 19](https://github.com/hozyhozy/Tableau/assets/123252821/0f79d2a8-f1a5-4f9f-af7d-59e53ea353c7)


### Q2. 카테고리의 더 아래수준인 메뉴명 별 칼로리와 카페인 --> 트리맵사용 (마크 사각형)
1. 칼로리와 카페인을 가져올 때 합계를 가져와도 상관없다. why? 메뉴명이 가장 작은 단위임
2. 트립맵은 마크 사각형에서 실행한다. 행열에 알약을 드래그하면 안된다. 마크에 바로 드래그하기!

   
![스크린샷 2023-07-24 오후 9 12 24](https://github.com/hozyhozy/Tableau/assets/123252821/dc8eef43-74cc-4514-9731-e615510c9243)


### Q3. 두개의 시트를 연결해보자!
1. 도구설명을 클릭해서 시트 연결
2. maxwidth, maxheight 조정하기


![image](https://github.com/hozyhozy/Tableau/assets/123252821/7a7c40ef-4ecd-4800-b4be-057368716356)


### Q4. 당분 함유량과 칼로리 상관관계_ scatter 시각화
1. 가로축, 세로축에 무엇을 놓을 지 고민하기
2. 색상과 크기를 어떻게 놓을 지 고민하기
3. 마크 형태는 원으로!
4. 마크 세부정보에 메뉴명 드래그 --> 전체 데이터 수준에서 메뉴명 수준으로 변경됨
5. 추세선은 분석 --> 추세선 클릭 + 드래그


   
![image](https://github.com/hozyhozy/Tableau/assets/123252821/aefd22b0-6f6c-4462-85c7-4ff390ca1dea)



### Q5. 시군구 별 매장 분포 현황_ map을 활용하여 시각화
1. 경도(열), 위도(행) 데이터 셋을 활용
2. 마크 크기와 색상을 어떤 지표로 시각화할지 고민하기 (매장 코드를 카운트 하여 매장 수를 표현할 수 있음)
3. 세부사항은 시도 또는 시군구로 조절 가능
   

![스크린샷 2023-07-24 오후 9 38 34](https://github.com/hozyhozy/Tableau/assets/123252821/f16688ac-ec1d-40d1-978d-91546cfdf99a)


### Q6. 대시보드 만들기


![image](https://github.com/hozyhozy/Tableau/assets/123252821/45385e30-c533-4916-a061-7e94988bd991)


![스크린샷 2023-07-24 오후 9 42 53](https://github.com/hozyhozy/Tableau/assets/123252821/5fa52b9a-af48-4226-8961-fbdd1850b2a4)



# Key Takeaway 
1. 막대 차트 사용시 비슷한 값 비교를 명확하게 하기 위해 데이터 정렬을 권장
2. 변수의 의미를 잘 파악해야함 ex. 카페인, 칼로리일 경우 카테고리로 집계하게 된다면 합계X 평균O
3. **트리맵의 장점**: 계층 구조의 데이터를 표시하는데 적합한 시각화로 전체 대비 부분의 비율이 얼마나 되는지 비교하는데 많이 사용 / 더 많은 양을 한번에 볼 수 있다는 장점!
4. **스캐터 플롯**: 2개의 연속형 데이터에 대한 상관관계를 분석하는데 가장 많이 사용되는 시각화로 두 개의 축으로 데이터가 얼마나 퍼져 있는지 분포를 살펴 볼 수 있고, 상수 라인 / 평균 라인 / 사분위수 및 중앙값 / 추세선 등과 같은 참조 라인을 추가하여 값의 분포를 비교하기에도 유용함!
5. **map**: 위도는 행, 경도는 열
