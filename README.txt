# Embedded-Recipes
recordings


19/10/14
1. Hardware collage-회로도읽기
  1) Hardware 꼴라쥬
  2) 신호와 주파수 영역 - Spectrum Analysis
    - 신호는 많은 주파수를 가진 주기 신호의 합
    
19/10/16
  3)Analog 신호와 Digital 신호, 그리고 Ground
    - Digital 신호 ∈ Analog 신호
    - Analog | AC : 주파수 성분O DC : 주파수 성분 X
    - Digital | Threshold : High, Low값의 임계값
    - Bounce : 0->1->0 변할 때 AC성분이 Transistion noise 발생
    - GND : 0V로 만드는 기준점, PCB기판 뒷면 저항을 적게 하여 만듬
    - CDMA 통신이 곽광받으며 Digital의 장점 부각
    - Capacitor : Power line의 전압, 전류 유지, GND에도 연결
    - filter : noise 제거
    
19/10/17
  4) 초간단 회로이론 R(저항), L(인덕터), C(캐패시터)
    - 저항은 회로의 특정 부분에 흐르는 전류의 양을 제한할 수 있다.
    - 전류가 저항을 지나고 나면 그 만큼의 전압이 원래 전압에서 빠진다.
    - 캐패시터는 AC성분만 통과시킨다.
    - 캐퍼시터는 DC성분과 AC성분을 분리해낸다.
    - 단위는 F, 패럿
    - 인덕터는 전류가 변화하지 못하도록 한다.
    - 단위는 H, 헨리
    - 저주파의 전류만이 통과할 수 잇다.
