# Tearch_Cam2

<p align="center">카페에 빈 좌석이 있는지 확인하고 방문하세요!</p>
<p align="center">카페에 사람이 몰리는 주말, 그리고 15시~19시!</p>
<p align="center">비어있는 근처 카페를 이용하고 싶다면 Tearch 이용해보세요</p>
<p align="center">Table + Search = Tearch ! 기억하세요!</p>
<p align="center">불필요하게 돌아다닐 필요가 없어져요</p>

___
### 부족한 점:
- createCaptureSession() deprecated : deprecated된 method를 고치는 법을 찾지 못했다. 다시 찾아볼 예정
- Auto Capture : 찾아보니 버튼을 누르면 시간에 따라 자동 촬영하는 기능이 없는 것 같았음. 그래서 강제적으로 함수들 간에 무한 루프를 돌게 하여 강제 자동 촬영을 하도록 만듦. 취소하는 것도 강제적으로 finish()를 하여 취소하는 방법.

___
#### 개발배경:
- 공휴일, 연남동과 같은 인구 밀집 지역은 여러 카페가 있음에도 몰리는 인원 탓에 카페가 가득차고 여러 카페들을 둘러봐야 하는 어려움이 생김
- 코로나 시대에 거리두기 정책으로 평소보다 적은 좌석으로 운영하고 사람이 적은 카페를 이용하길 원함
- 10세-59세 일반인을 상대로 조사한 결과 오후 3시~6시경에 이용시간이 가장 높고 평균 30분에서 2시간 정도 카페를 이용하는 것으로 집계되었음. 과거에 비해 많은 소비자들이 카페 공간을 이용하는지 나타났고 위의 이유들로 인해 실시간으로 가길 희망하는 카페의 자리가 얼마나 남았는지 알려주는 서비스가 필요하다고 생각이 들어 기획하게 되었음.

___
#### 개발목표 및 내용:
- Tearch_pc 어플리케이션에서 Tensorflow로 분석한 데이터를 Firebase를 통해 실시간 데이터 처리
- 카페의 빈 좌석을 한 눈에 볼 수 있도록 개발

___
#### 구성도:
![image](https://user-images.githubusercontent.com/66459882/130782728-6e9b2121-b444-481c-9b6a-745c8d7bae1a.png)

___
#### 기대효과 및 시장성:
- 사용자에게 카페의 빈 좌석 정보를 제공함으로써 카페를 이용하는 소비자에게 편의를 제공
- 카페가 잘 알려지지않거나 위치가 좋지 않은 경우에 소비자가 적은데, 이때에 빈 좌석 정보와 위치를 나타냄으로써 소비자들이 해당 카페도 이용할 수 있도록 도와줌

___
##### 배운점:
- Firebase Storage
- Hardware.Camera2
- Camera2.StateCallback
- TextureView
