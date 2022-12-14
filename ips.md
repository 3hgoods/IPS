
### IPS


- https://www.mokosmart.com/ko/introduction-to-indoor-positioning-system/
```
IPS와 GPS는 어떻게 다른가요?
GPS와 IPS의 차이점에 관해서는 많은 사람들이 혼란스러워 할 수 있습니다., 유사한 작업을 수행하고 유사한 약어를 사용하기 때문에. 사실로, IPS는 GPS의 추가 개발 및 확장으로 간주될 수 있습니다.. 앞서 언급했듯이, IPS와 GPS의 가장 큰 차이점은 적용 분야에 있습니다.. 하나는 정확히 실내 환경용입니다., 다른 하나는 실제로 야외 공간을 위해 설계되었습니다..

실내와 실외의 공간차이가 크기 때문에, IPS와 GPS의 기술 채택은 완전히 다릅니다.. GPS 수신기는 위치를 결정하고 움직임을 추적하기 위해 3개 이상의 위성에서 오는 신호를 고정해야 합니다., IPS는 보다 정확한 측정을 위해 다양한 기술을 적용합니다.. 주목할 가치가 있는 것은 실내 GPS가 지속적인 연구 분야라는 것입니다., 미래에 새로운 옵션이 나타날 수 있습니다..

```


### 개발사례 1

- https://mobile.newsis.com/view.html?ar_id=NISX20220708_0001936498#_enliple

```
"GPS, 와이파이, 블루투스 신호 수신 칩과 관성센서, 기압센서, 지자기센서, 조도센서 등을 탑재시킨 실내외 통합 GPS 전용 보드를 제작했다"며 "이어 제작된 하드웨어(HW) 보드에 개발된 센서퓨전 위치인식 알고리즘을 탑재했다"고 설명했다.

지금까지는 GPS 신호가 도달하지 않는 공간에서는 무선랜 신호나 기지국 신호를 기반으로 위치를 인식하는 것이 일반적이었다.

이번에 개발한 실내외 통합 GPS 시스템은 신호가 존재하지 않고 실내지도가 제공되지 않는 건물에서도 위치인식을 가능한 첫 기술로 전 세계 어디서나 사용할 수 있는 범용적인 실내외 통합 GPS 시스템을 구축할 수 있는 기반을 마련했다는 평가다.

이 알고리즘은 구글, 애플의 위치인식 서비스에서는 제공하지 않는 건물 안의 정확한 층 정보를 제공할 수 있고 지구 자기장, 무선랜 측위 방식과 달리 사전 준비 작업도 필요치 않다

연구팀은 위치인식 보드가 내장된 태그를 제작하고 박물관, 과학관, 미술관 방문객들을 위한 위치기반 전시 안내 서비스에 적용할 예정이다.
 
개발된 실내외 통합 GPS 태그는 어린이나 노약자를 보호하는 목적으로도 활용할 수 있으며 소방관 혹은 작업장 작업자의 위치 파악에도 활용할 수 있다.

연구팀은 지하 주차장과 같은 실내로 진입하는 차량의 위치를 추정하는 차량용 센서 퓨전 위치인식 알고리즘과 위치인식 보드 개발에도 나섰고 차량용 실내외 통합 GPS 위치인식 보드가 제작되면 자동차 제조사 등과 협력해 고도화 및 상용화를 모색하고 스마트폰에 탑재될 센서 퓨전 위치인식 알고리즘도 개발할 예정이다.

개발된 알고리즘이 내장된 실내외 통합 GPS 앱이 개발되면 위치인식 분야에서 다양한 사업화를 모색하는 통신사와의 협력도 가능할 것으로 기대된다.

```



### 개발방향1

```
1) mobius iot 플랫폼을 빅데이터 수집수단으로 사용
 data1 --> 핸드폰에서 수집한 정보를 서버에 전달하는 방식
 data2 --> 정답 데이타 (실제 위치 데이터)

2) 꼭 있어야 하는 보정 기술
 묻고 답하기 기술  (태그) 
 건물에 태그는 묻는 위치 정보에 대한 답은 주는 수단.
 
 보정1: 정보 수신후 변경된 나의 위치 정보에 대한 수정업데이트 how?
        혹시 태그에 출발한 시간 정보를 주어 태그 위치점에서 변경된 위치를 계산할 수 있지 않나?
        --> wifi 중계기에 넣을 수 있나?
        
 보정2: 엘리베이터가 터널과 같이 기존 센서의 오차공간인데.. 오히려 정보 보정공간으로 사용?
 
 보정3: 벽을 통해 전달된 정보에 딜레이가 있다면 어떻게 보정해야 하는가?
       - 여러개의 중계기에서 가장 빨리 도착한 AP중심 혹은 강도가 센/ 전송속도?? 장비를 중심으로 변경되도록..
       - wifi도 자동 변경이 되나?
       
 보정4: 내가 wifi 잡지 않았는데도 정보 수신이 되나??
        - 반대로 내가 한개의 wifi를 잡았는데... 나머지에게서도 계속 접속??정보를 수신해야 하나?
  
 보정5: 5G,LTE, 2G 각각 속도가 다른데 수신 계산을 구분할 수 있나?
 -   
 
```

### 개발방향2 wifi tag

```
wifi tag 정보를 전송하여 보낸 기기의 위치 정보를 확인하여 나의 위치정보를 계산할 수 있을까?

```

- 관련정보 https://www.yna.co.kr/view/AKR20190406057600017

```
- 지하철역사 와이파이 위치정보, 민간에 개방된다

7일 정보기술(IT)업계에 따르면 한국인터넷진흥원(KISA)은 올해 수도권과 부산, 광주, 대전, 대구 등의 실내 지하철 역사 890곳의 와이파이 접속장치(AP) 데이터베이스(DB)를 스타트업 등 민간이 활용할 수 있도록 지원할 계획이다.

KISA는 DB를 갱신해 개선한 후 개방할 예정이다.

DB는 원데이터와 함께 원데이터가 아닌 데이터를 활용해 위치 측정이 가능한 개발툴(SDK) 형태로 개방된다.

사용자의 단말기를 스캔해 주변의 AP 정보를 수집한 후 이미구축된 DB와 가장 유사한 패턴을 분석해 최종 위치를 측정, 전송한다.

스타트업이 DB를 활용하면 초기 개발비용 부담을 줄여 다양한 위치 정보 관련 콘텐츠와 서비스를 개발하는 데 도움이 될 것으로 기대되고 있다


```

관련 특허
- https://patents.google.com/patent/KR101453317B1/ko
-




### 개발방향3 건물 단위로 맵핑정보 제공받음.

```
건물주가 참여(제공)하는 방식의 맵핑 정보를 활용한 구성

```

```

우리 공유기는 위치 정보를 나름 제공하고 있다.
https://slic.tistory.com/1464

와이파이 기반 위치 획득 체계 (Wi-Fi positioning system, WPS)


```

- 프로그램 제공

```
https://developers.loplat.com/wps/
ttps://loplat-ai.appspot.com/wps



```






