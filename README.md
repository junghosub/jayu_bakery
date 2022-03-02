# 자유빵집🥖
## 캐셔에서 데이터 분석까지
<p align = "center">
<img src="https://miro.medium.com/max/1400/1*KdQIMfK-2l15-Iop3333zw.jpeg" width="750">
</p>
  
## 분석 배경 및 내용
>개인 빵집에서 1년 6개월가량 아르바이트를 했습니다. 자그마한 빵집이었지만 빵지순례 코스로 자리 잡고 있을만큼 매일 손님으로 북적이던 곳이었습니다. 2019년 7월 . 지역 주민을 위해 배달의 민족 서비스를 시작했고, 코로나의 확산으로 전 직원이 배달 서비스의 중요성을 느끼게 되었습니다. <b> 배달 서비스를 이용하는 고객의 니즈와 개선점을 파악하고 이를 공유하기 위해 진행하였습니다.</b>

<b> 배달의 민족 사이트에서 데이터를 직접 수집</b>한 후, 아래와 같은 분석을 실시하였고, 해당 분석 결과는 월말 전 직원들과 공유했습니다.

1. 월별 판매액과 품목별 판매액을 파악하였습니다. 판매량이 저조했던 달이 있다면 제품 또는 서비스의 문제였는지에 대해 회의를 통해 문제점들을 파악하였습니다.
2. 시간대에 따른 주문량을 파악했습니다. 이를 통해 제품의 생산량을 조절하였고, 필요 직원의 수와 요일별 임금을 조정할 수 있었습니다.
3. 장바구니 분석을 진행하여 제품별 support, confidence, lift를 확인하였습니다.

매출 관련 데이터이므로 2020년 4월까지의 데이터만 공개하였습니다.

--- 
## 분석 결과
### 1. 코로나-19🤧와 배달의 민족🏍️

<img src = "https://miro.medium.com/max/1400/1*qys8gjWGRwfuxkqn2-tyCg.png" width = "550" height = "300">
흔히 말하는 오픈빨이 있었는지 8월 매출이 상당히 높았습니다. 그 이후로는 안정세를 보이다 코로나-19가 확산된 시기인 2020년 1월 이후 매출이 다시 늘었습니다.
<p>
  </p>
<img src = "https://miro.medium.com/max/1400/1*FS0s-20bxGWzF9IV7qHj3w.png" width = "550" height = "300">
1차 대유행이 있던 2,3월에는 많은 매출을 기록했고, 소강 상태에 접어들던 4월에는 배달의 민족 매출이 이전보다 감소한 것을 확인할 수 있었습니다.

--- 

### 2. 제품별 판매량💳

<table>
   <tr>
     <td> 앙버터 </td>
     <td> 크로아상 </td>
   </tr>
   <tr>
      <td><img align="left" src="https://miro.medium.com/max/1756/1*AlfGCprWO_Z0PaPfooAWHw.png" alt="Made with Angular" title="앙버터" hspace="0" width = "450"/>
      <td><img align="left" src="https://miro.medium.com/max/1690/1*EbVZAFQep_ndx_WIfRTJ-A.png" alt="Made with Bootstrap" title="크로아상" hspace="0" width = "450"/>
  </tr>
</table>
 
 <table>
  <tr>
    <td> 식빵 </td>
    <td> 뺑오쇼콜라 </td>
  </tr>
  <tr>
      <td><img align="left" src="https://miro.medium.com/max/1712/1*ABGheNcabr4iCEXFGfv8Xg.png" alt="Made with Angular" title="식빵" hspace="0" width = "450"/>
      <td><img align="left" src="https://miro.medium.com/max/1702/1*05FQscRAAfYGCkWMNRahhw.png" alt="Made with Bootstrap" title="뺑오쇼콜라" hspace="0" width = "450"/>
  </tr>
 </table>
 
  <table>
  <tr>
    <td> 티라미수 크로아상 </td>
    <td> 카카오딥 </td>
  </tr>
  <tr>
      <td><img align="left" src="https://miro.medium.com/max/1756/1*c_32klApYPhKnKr53O8_9g.png" alt="Made with Angular" title="티라미수 크로아상" hspace="0" width = "450"/>
      <td><img align="left" src="https://miro.medium.com/max/1702/1*n2lF8joO7H5knFGvd5RXTQ.png" alt="Made with Bootstrap" title="카카오딥" hspace="0" width = "450"/>
  </tr>
 </table>
 
   <table>
  <tr>
    <td> 팡도르 </td>
    <td> 오렌지파운드 </td>
  </tr>
  <tr>
      <td><img align="left" src="https://miro.medium.com/max/1730/1*e1eq7nsq0nGPP765tqP5eA.png" alt="Made with Angular" title="팡도르" hspace="0" width = "450"/>
      <td><img align="left" src="https://miro.medium.com/max/1690/1*1EnQeKd4wwV_8tjCP44y4w.png" alt="Made with Bootstrap" title="오렌지 파운드" hspace="0" width = "450"/>
  </tr>
 </table>
 
 
### 3. 요일과 시간대에 따른 판매량🌞
 
#### 월별, 요일별 평균 주문량
<img src = "https://miro.medium.com/max/1400/1*Y-BJhSst0himWeyy1clDUg.png" width = "700">

#### 요일별 총 주문량
<img src = "https://miro.medium.com/max/1400/1*eMkrH09yLD-cGBlwW5VJ1w.png" width = "700" height = "370">

점심시간에 주문량이 많이 몰리는 것을 확인 할 수 있습니다. 이는 전 직원이 체감했던 점입니다. 하지만 금요일에 배달 주문량이 적다는 사실은 의외였습니다. 금요일 아르바이트생에겐 높은 시급을 주었는데 이번 분석을 통해 조정하게 되었습니다.

#### 주말엔 브런치🥪
<img src = "https://miro.medium.com/max/1400/1*cgRZIKxhiuboUcZuRBhF3g.png" width = "700" height = "370">

매장에서보다 배달의 민족을 통해 식빵을 찾는 고객이 더욱 많았습니다. 특히, 주말 점심 시간대에 많은 주문량이 몰리는 것을 보아 토스트, 샌드위치 등 브런치를 위해 먹는 사람이 많을 것 같다는 생각을 하였습니다. 차후 회의를 통해 브런치에 걸맞는 메뉴인 크로크무슈를 새로 만들게 되었습니다.

### 4. 지역에 따라🏡
<img src = "https://miro.medium.com/max/1400/1*MBqGb30v6T_YTIdLpBmPDw.png" height = "370">

매장의 위치가 동면에 위치하고 있기 때문인지 동면과 근접 지역인 후평동에서 주문량이 많았습니다. 배달의 민족에서는 거리에 따라 배달 요금이 상이합니다. 고객의 거리가 먼 경우엔 매장에서 부담하는 배달 요금이 많아지기 때문에 해당 지역까지 배달 서비스를 제공하지 않았습니다. 이러한 이유로 거리가 먼 지역에서는 주문량이 상대적으로 적었습니다.

<img src = "https://miro.medium.com/max/1400/1*aHPtGImFOnMvDUqIsYhpaw.png" height = "450" width = "700">
공공데이터를 활용하여 경쟁 상대가 될 수 있는 프랜차이즈 빵집의 위치를 확인해보았습니다.(파랑 : 파리바게트, 녹색 : 뚜레쥬르, 빨강 : 본 매장) 석사동과 퇴계동에 프랜차이즈 빵집들이 많이 위치한 것을 볼 수 있습니다. 경쟁 상대도 많지않고, 최근 아파트 단지가 조성되고 있는 온의동 또한 좋은 후보가 될 것 같습니다. 다음 2호점은 현재 매장에서 거리가 멀어도 수요가 있는 석사동과 퇴계동 또는 온의동 지역에 오픈하는 것이 좋을 것 같다고 의견을 나누었습니다.

시간이 지나고 실제로 온의동에 [2호점](https://map.naver.com/v5/entry/place/1894407066?c=14217435.9557047,4559570.4774992,13,0,0,0,dh&placePath=%2Fhome%3Fentry=plt)을 오픈하였습니다!

### 5. 장바구니 분석🧺
통계학과에서 데이터 마이닝 강좌를 수강하며 '[장바구니 분석](https://en.wikipedia.org/wiki/Association_rule_learning)'에 대해 공부한 적이 있습니다. 해당 분석을 통해 고객들의 구매 리스트에서 유의미한 관계를 도출한다면 이벤트나 세트 상품을 만들 수 있을 것이라 판단해 Python에서 구현해보았습니다.

- support순으로 정렬한 결과
<img src = "https://miro.medium.com/max/620/1*KtRHGLlapqAFYwlDwCP1IA.png">
앙버터로 유명한 가게이니만큼 대부분의 사람들이 앙버터를 주문하고 있었습니다. 매장과는 다르게 식빵의 판매 비중 또한 높았습니다.
<p>
  </p>

- lift순으로 정렬한 결과
<img src = "https://miro.medium.com/max/1400/1*-tDaKKXCx30qmSzufEpeIQ.png">

식빵과 잼 또는 구매 수가 높은 앙버터, 크로아상 등의 제품들이 lift가 높았습니다. 대형 마트와 같이 제품 수가 많지 않아 아쉽게도 눈에 띄는 관계들은 찾기 어려웠습니다. 하지만 강의에서 배운 이론을 직접 구현해본 것은 좋은 경험이 되었습니다.

---
## 마치며🙂
호기심으로 시작해본 분석이라 그런지 많이 부족한 것 같습니다. 처음 분석을 진행할 땐 Python을 아예 할 줄 몰라서 유튜브, 책 등을 통해 마구잡이로 공부하기 시작했습니다. 해결되지 않는 오류에 짜증 내보기도 하고, 더 나은 분석을 위해 Kaggle 커뮤니티에 질문도 해보고 피드백도 받아보았습니다.
여러 시행착오를 겪었지만 데이터를 직접 수집 및 전처리 해보고 직원분들께 발표도 해보는 등 좋은 경험을 쌓은 것 같습니다. 또한 타인의 문제를 코드를 통해 해결할 수 있다는 점도 깨달았습니다.

나아가 팬데믹으로 많은 산업들이 오프라인에서 온라인으로 전환되고 있는 상황 속에서 로컬 비즈니스 또한 변화하고 있다는 점을 깨달았습니다. 재빨리 딜리버리 또는 온라인 판매를 도입하시는 사장님분들도 계신 반면 온라인에 익숙하지 않으셔서 더욱 힘든 시기를 겪고 계신 분들도 있을 것입니다. 향후 이런 분들을 위한 간편화된 매장 매출 분석 서비스나 단골 고객 유치를 위한 서비스를 제공해보고 싶습니다.
