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
    - R이 클수록 전류를 더 조금 흐르게
    - C가 클수록 저항이 작아져서 전류가 많이 흐르고
    - L이 클수록 저항이 커져서 전류가 조금 흐르게 한다.
    - R은 주파수를 타지 않고
    - C는 높은 주파수일수록 저항이 작고
    - L은 높은 주파수일수록 저항이 크다.
    - L과 C는 filter로 사용
  5) 초간단 회로이론 응용 - 필터(Filter)
    - LPF는 Low Pass Filter라고 하며, 저주파 성분만 통과
  6) Transistor 1%
    - TR은 npn형과 pnp형 두가지가 있다.
    - 스위치에 넣어주는 전압량(전류량)에 따라 포화 영역, 활성 영역, 차단 영역이 생긴다.
    - 증폭 기능과 Switching 기능
  
19/10/23
  7) Pull up, Pull down 그리고 Open Collector
    - Low-Active, High-Active => Pull up <-> Pull down
    - reliable한 Default 값을 보장하기 위해 Pull up이나 Pull down
    - Switch가 Master chip 내부에 아예 들어가 있는 경우를 Open collector라고 부른다.
    - High Impedance 상태 ≒  Floating
  8) RLC와 Transistor 感   
  9) 논리회로로의 확장
    - 카르노맵을 구사하면 간단하게 input에 대한 output을 만들어 내는 논리 조합을 만들어 낼 수 있다.
  10) IC기본
    - 자리표시가 되어 있는 부분을 왼쪽에 놓고, 반시계방향으로 읽는다.
    - NC : 기능 없음 / CLK : edge trigger / GND : Ground / VCC: 전원
    
19/10/28
  11) Register 넌 누구냐
    - Register는 Flip Flop의 집합
    - Flip Flop 회로는 다음 input이 들어올 때까지 Data Out을 유지
    - RS Flip Flop
    - Level Trigger Latch : Write 신호가 High로 올라가 있는 동안 DI 기억
    - Edge trigger Latch : clk가 올라가는 순간이나 내려가는 순간에만 write가 가능하고 그것이 아닌 순간에만 그 전에 write 된 값을 기억
    - General Purpose Register / Special Purpose Register
    - I/O Register

19/10/30
  12) clock이란?
    - 동기화(Synchronization)
    - system적으로 Clock이 모든 행위의 단위
    - 처리 속도가 다른 논리회로 출력 판단
    - 디바이스들의 시간적인 동작 범위가 있으므로 무조건 빠르다고 될 일은 아니다.

19/11/26
  13) Bus Transfer Mechanism
    - Bus system은 Clock에 맞추어 한 가지 종류의 신호만 존재
    - Arbiter : Algorithm Policy에 의거하여 사용권을 부여
  14) Timing 그리고 Spec 읽기
    - 전달 지연 시간, 스위칭 특성
    - 상승시간, 하강시간->물리적인 차이까지 System 구성 시 고려
    - Timing Diagram->Timing Spec 해석으로 시간 제햔/최소시간 조절하여 Data를 잘 처리할 시간을 번다.

19/11/27
  15) Memory의 선정과 XIP
    - Memory의 선정은 System 구성과 Performance에 영향력 행사
    - RAM 휘발성/ROM 비휘발성
    - XIP : 메모리상에서 직접 program/code 실행 (Execute In Place) Random Access가 가능해야한다.
