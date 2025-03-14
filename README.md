# React를 활용한 Team Project - Korail

## 프로젝트 개요
**Korail** 프로젝트는 5명의 팀원으로 구성된 협업 프로젝트로 진행되었습니다. 

이 프로젝트에서는 **React**를 사용하여 웹 애플리케이션을 개발하였으며, **Firebase Firestore DB**, **Swiper**, **MUI (Material-UI)**를 활용하여 UI/UX를 향상시키고 데이터를 관리했습니다. 

또한, **Firebase Firestore**와 **JSON** 데이터를 활용하여 **역위치 정보**와 **열차 운임 조회 및 운임표 정보**를 처리했습니다.

## 사용 기술
- **React** (JSX, 컴포넌트 구조)
- **HTML5**, **CSS3**, **JavaScript**
- **Firebase Firestore DB** (실시간 데이터베이스 관리)
- **JSON** (정적인 데이터 사용)
- **Swiper Library** (슬라이드 기능)
- **MUI (Material-UI)** (UI 컴포넌트 라이브러리)
- **카카오지도 API** (위치 정보 표시)
- **AOS** (스크롤 시 동적 효과 적용)
- **Git** 및 **GitHub** (버전 관리 및 협업)

## 역할
- **Header**, **Visual Section(Section1)**, **Footer**, **Top Menu** 및 **역위치정보(sub5)** 서브페이지 전담
- **React**를 사용하여 컴포넌트 기반 UI 설계
- **Firebase Firestore DB**를 활용하여 **역위치정보** 데이터 처리

## 활용 기능
- **Firebase Firestore DB** : Firebase Firestore에서 station 컬렉션 데이터를 가져와 역 정보를 검색하고 표시되도록 구현했습니다. 사용자가 입력한 역명을 검색하여 해당 역의 정보를 필터링하고, 검색된 정보를 TaskDisplay 컴포넌트에 전달하여 기본 정보와 층별 시설 안내를 표시합니다. 또한, KakaoMap 컴포넌트를 사용해 각 역의 출입구 정보를 지도상에 표시되도록 설계했습니다.
- **Header** : 스크롤 이벤트를 통해 window.scrollY 값을 확인하고, 특정 위치(780px) 이상일 때 header의 스타일을 동적으로 변경하여 sticky 효과를 구현하였습니다. 사용자 편의를 위해 화면 크기가 768px 이하일 경우 햄버거 메뉴가 토글되며, 메뉴의 열림/닫힘 상태는 isSwitched 상태로 관리합니다. 접근성을 고려하여 본문 바로가기와 글로벌 네비게이션 바로가기 링크를 추가했습니다.
- **Visual Section (Section1)** : **Swiper Library**를 사용하여 슬라이드 기능을 구현했습니다. autoplay로 자동 전환 타이밍을 2.5초로 설정하고, speed로 전환 속도를 1.5초로 조정했습니다. effect="fade"와 fadeEffect를 사용해 부드러운 페이드 효과를 적용하며, loop 속성으로 슬라이드가 반복되도록 설정했습니다. 사용자 상호작용을 위한 내비게이션과 페이지네이션도 추가하여 직접 슬라이드를 넘길 수 있습니다.
- **Footer** : "계열사"와 "관련사이트" 항목을 토글할 수 있는 기능으로 family Site를 설계했습니다. useState를 사용하여 각각 isSwitched와 isSwitched2 상태를 관리했습니다. 각 버튼 클릭 시 isSwitched와 isSwitched2 상태 값에 따라 삼항 연산자를 사용해 ul의 클래스명을 동적으로 변경했으며, 이를 통해 목록이 보이거나 숨겨집니다. 각 링크는 새 창에서 열리도록 target="_blank"와 rel="noopener noreferrer" 속성을 설정했습니다.
- **Top menu** : 사용자의 스크롤 위치에 따라 Top menu의 표시 여부를 제어하고, '맨 위로 가기' 버튼을 부드럽게 작동하도록 구현했습니다. useState를 사용해 스크롤 위치에 따라 메뉴의 상태를 관리하고, handleScroll 함수에서 window.scrollY를 확인하여 스크롤이 300px 이상일 때 메뉴가 표시되도록 했습니다. topHandler 함수로 버튼 클릭 시 페이지를 부드럽게 상단으로 이동시키는 기능을 구현했습니다.
- **MUI 컴포넌트**: **Material-UI**를 사용하여 현대적이고 일관된 UI 스타일링을 적용하였으며, 버튼, 텍스트 필드 등 다양한 UI 요소를 통일감 있게 구성하여 사용자 경험을 개선했습니다.

## 협업 및 기여
프로젝트는 Git을 통해 협업하며 각자 역할을 분담하고, GitHub를 이용해 효율적으로 소스를 관리했습니다. 
팀원들과의 긴밀한 커뮤니케이션을 통해 UI/UX 디자인 및 기능 구현에 대한 피드백을 주고받으며 협업을 진행했습니다.

## 결론
**Korail** 프로젝트는 React를 사용한 웹 애플리케이션 개발을 통해 **Firebase Firestore DB**, **Swiper**, **MUI (Material-UI)**와 같은 라이브러리와 도구를 활용하여 기능적인 웹 애플리케이션을 만들었습니다. 

특히, **Firebase Firestore**의 데이터베이스를 활용하여 역 정보와 관련된 데이터를 관리하고, 사용자가 검색어를 입력하면 실시간으로 검색 결과를 필터링하여 보여주도록 하였습니다. 또한, KakaoMap API를 통합하여 각 역의 출입구 정보와 위치를 지도상에서 표시하며,직관적인 UI로 층별 시설 안내를 제공했습니다. 나아가, **JSON** 파일을 통해 열차 운임 조회 및 운임표 데이터를 처리하여 실시간 정보 제공이 가능하도록 하였습니다. 

이 프로젝트를 통해 데이터베이스 관리, UI/UX 개선, 그리고 팀 협업 경험을 쌓았으며, 이러한 경험을 바탕으로 더 나은 웹 개발자로 성장하고자 합니다.
