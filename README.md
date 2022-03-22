# Wegabox

- [메가박스](https://www.megabox.co.kr/) 영화 예매 사이트를 학습 목적으로 클론하는 프로젝트
- 필수 구현 사항과 추가 구현 사항을 나누어 2주간 진행
- `Front-End`와 `Back-End`로 나누어서 실무에 가깝게 협업하는 방식으로 진행하였으며 개발환경 초기세팅부터 AWS 배포까지 직접 완료

## 개발 인원 및 기간

- 2022.01.10 ~ 2022.01.21
- Front-End: [김용선](https://github.com/seankim1111), [윤종호](https://github.com/myway8907), [정민아](https://github.com/minami-cs)
- Back-End: [강민성](https://github.com/nonasking), [장민욱](https://github.com/black2code)
- [Wegabox Back-End Repository](https://github.com/wecode-bootcamp-korea/28-2nd-Wegabox-backend)

## 사용 기술

- Front-End: <img alt="react" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" /> <img alt="react-router" src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" /> <img alt="styled-components" src="https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white" /> <img alt="chartjs" src="https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white" /> <img alt="aws" src="https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
- Back-End: <img alt="python" src="https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen" /> <img alt="django" src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=green" /> <img alt="mysql" src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" /> <img alt="aws" src="https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />

## 협업 도구

- [Trello](https://trello.com/b/UVZf8Oim/wegabox-wecode-4-team)
- Slack

## 구현 사항

[Wegabox 웹사이트 보러 가기](http://54.144.54.249:8000/)

1. 메인 페이지 by. [정민아](https://github.com/minami-cs)
   ![mainpage](https://user-images.githubusercontent.com/66506477/150678855-7ed2702d-0e8e-488e-b173-54b2ee9e8d33.gif)

2. 소셜 로그인(카카오톡) by. [김용선](https://github.com/seankim1111)
   ![kakaologin](https://user-images.githubusercontent.com/66506477/150678726-a595bd25-8e8d-4a93-a1a9-45445124f9b1.gif)

3. 목록 페이지 by. [정민아](https://github.com/minami-cs)
   ![listpage](https://user-images.githubusercontent.com/66506477/150679005-9edb5a0c-9308-4a27-ad9d-2a3b4fa5713c.gif)

4. 상세 페이지 by. [정민아](https://github.com/minami-cs)
   ![detailpage](https://user-images.githubusercontent.com/66506477/150678923-0c325bbd-5f7c-4184-b8ae-c74aa0b6575d.gif)

5. 예매 페이지 by. [윤종호](https://github.com/myway8907)
   ![bookingpage](https://user-images.githubusercontent.com/66506477/150679205-b99c68ed-0907-4e31-9f14-a6bd4eccc5d1.gif)
   
✔️ **UI 기획 및 구현**
- 참조 사이트를 기반으로 하여 UI 기획
- `React-scroll` 등의 라이브러리 활용하여 페이지 스타일링

✔️ **공통 컴포넌트를 재사용하여 예매 옵션 목록 구현**
- props로 전달되는 내용에 따라 상황에 맞는 내용이 화면에 렌더링 되도록 구현

✔️ `**Styled-components`를 이용하여 반복 사용되는 공통 스타일링 컴포넌트 제작 및 활용**

✔️ `**transition & transform` 속성을 사용하여 커서 이동 시 목록 요소들의 사용자 반응 스타일링**

✔️ **예매 프로세스 기획 및 구현**
- 반복 사용되는 함수들을 컴포넌트에서 분리하여 모듈화 및 재사용
- `React state` 하나를 변화의 구심점으로 삼아, 사용자가 선택한 영화 상영 옵션들이 저장되도록 구성
- 옵션 선택이 저장된 state의 변화에 따라 선택한 옵션 이외의 옵션들이 그에 반응하도록 구현
- 다양한 상황마다 필요한 state를 생성하지 않고, 단일 state를 중심으로 변화가 돌아가도록 구현하여 불필요한 state 생성을 예방하고 state 관리 최소화
- **빠른 코드 작성 보다 명확한 로직을 확립을 지향**
- ![image](https://user-images.githubusercontent.com/93215875/159452030-279071ce-f3a1-4eac-81e8-e47dd390a6b3.png)


# Reference

- 이 프로젝트는 메가박스 사이트를 참조하여 학습목적으로 만들었습니다.
  실무수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
- 이 프로젝트에서 사용하고 있는 사진 대부분은 위코드에서 구매한 것이므로 해당 프로젝트 외부인이 사용할 수 없습니다.
