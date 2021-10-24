# 에어컨과 에어커튼 기술을 조합한 실내 화재 사고 지연 장치

## 목표
고층 화재 발생 시 구조 및 생존 가능성을 증가

## 핵심내용
1. 화재 발생 시 장치 중앙에 위치한 버튼을 사용자가 눌러 장치를 동작 시킴과 동시에 소방서에 장치의 고유 코드를 전송하여 구조 요청 전달(유해가스 센서 작동을 통해 오작동 방지)
2. 사용자에게 가장 인접한 유해가스를 장치 중앙의 흡기 팬을 이용하여 외부로 배출 (유동적 작동)
3. 사용자에게 외부 공기를 공급하고, 화염 보호용 에어 커튼을 구성하기 위해 장치 상단의 4개의 흡기 팬을 이용하여 사용자가 주변에 에어 커튼 대류 층 형성 (실외기 통합 기능 사용)
4. 비교적으로 고기압인 대류층에서의 기체들이 저기압인 사용자가 있는 위치 방향으로 모이는 원리를 이용하여 화재가 다른 곳으로 확산되는 것을 막아 실내의 다른 위치에 2차 피해 발생 방지
5. 에어컨에 추가적으로 장착하여 에어컨의 한 기능으로 설정하거나 독립적으로 설치하여 사용 가능
6. 평상시의 실내 미세먼지나 냄새를 제거하기 위해 By-Pass식 환기 기능을 도입하여 다른 환기 수단에 비해 효율성이 높음
7. 실외기 통합기능을 통해 효율적인 전력 사용, 오작동 하락

## 중요성
1. 고층 화재 시, 구조 및 생존 가능성을 증가시키는 효과
2. 기압차를 이용한 2차 피해 방지 기능을 통해 인명 피해 최소화
3. 에어 커튼을 이용한 더 효율적인 온/냉방 가능

## 서론
### 배경 설명, 사례 분석
지난 2017년부터 2019년까지 국내에서 큰 규모의 화재 사고가 많았습니다. **2017년 화성 동탄 메타폴리스 상가 화재 사고, 제천 스포츠센터 화재 사고, 2019년 진주 아파트 방화 살인 사건** 등 건물 화재 사고가 많았습니다.
국가화재정보센터에서 발표한 “화재 시 사망 원인 통계”에 따르면 화재 시 사망 원인의 약 60%가 연기로 인한 질식사라고 합니다. 특히 2016년부터 2018년까지 화재 사고 시 대피 실패로 인한 사망자는 350명인데 이것은 전체 화재 사고 사망자의 34%를 차지합니다. 이는 단순한 화재 예방 교육만으로는 원활한 대피가 이루어지지 않음을 나타냅니다.

### 문제 정의
화염이나 유해가스 등에 둘러싸여 대피를 못하는 경우가 있을 것이다.

### 극복 방안
원형 시스템 에어컨과 에어커튼을 보고, 화재 시에 시스템 에어컨의 에어커튼을 최대출력으로 출력시켜 주변 공기가 위아래로 대류 하는 구조를 만들고, 그 중앙에 사용자를 위치시킨다면, 유해가스가 사용자에게 다가가지 못해 피해를 최소화할 수 있을 것입니다.

## 본론
### 시스템 개요
![image](https://user-images.githubusercontent.com/51695816/138585088-083f2f33-d50c-4ebf-812a-86a3754b45b9.png)

### 필요한 기술 요소
본 장치를 구현하기 위해선 화재 및 유해가스를 인식할 수 있는 각종 센서와 에어커튼을 생성해줄 팬, 하드웨어를 제어할 MCU, 화재에서도 작동하기 위해 열에 강한 소재가 필요합니다. 또한, 시연장치 구현을 위해 3D 모델링 및 3D 프린팅 기술을 활용할 계획입니다.

### 구현 방안 및 개발 방향
본 장치의 작동을 보여주기 위한 시연장치를 제작할 것입니다. 아래와 같은 과정을 통해 구현할 것입니다.
* 3D 모델링으로 설계한 장치를 3D 프린터로 출력 및 조립
* 아크릴 상자로 실내 제작
* MCU를 이용해 센서 검출부, 전원 구동부, 외부 연결부를 제어 장치 구현
* 소방서를 가정한 외부 출력부에 연동하여 실시간 신고 구현
