# 📘 Today I Learned

### 1. 오늘 배운 내용

- React의 생명주기란?
- Hooking 이란?
- React Router란?

### 2. 핵심 정리 (내 언어로)

- React의 생명주기란: 컴포넌트가 생성되고 사용되고 소멸될 때 까지의 일련의 과정
  - Mount: 컴포넌트가 처음으로 DOM에 추가될때 (처음 화면에 나타나는 순간)
  - Update: 컴포넌트의 state 또는 props가 바뀔 때 (변경이 생길떄마다)
    - 발생시키는조건 3가지(부모 컴포넌트의 리렌더링 / state 변화 / context 변화)
  - Unmount: 컴포넌트가 제거되기 직전 (사라지기 직전)

- Hooking
  - 컴퓨터 프로그램에서 소프트웨어 구성 요소간에 발생하는 함수 호출, 메시지, 이벤트 등을 중간ㅇ에서 바꾸거나 가로채는 행위

- Hook
  - 함수 컴포넌트에서 React State와 생명주기 기능을 연동할 수 있게 해주는 함수
  - React에서 제공하는 Hook 종류들
    - useStates - state(현재값) 관리
      - 값이 바뀌면 화면이 바뀌어야 할 때 유용하게 사용가능
      - 로컬 데이터 관리 - 컴포넌트 내부에서 선언, 관리
      - 불변성 - 직접 수정하지 않고, setState(값을 바꾸는 함수) 혹은 useState로만 변경
      - UI 와 동기화 - 상태가 변경되면 리렌더링됨
      - setState 호출 -> React에서 리렌더링 예약 -> 컴포넌트 함수 재실행 -> 화면 갱신

      - state 업데이트
        - 일반형 업데이트
        - 함수형 업데이트

    - useEffect - 생명주기 처리
      - Mount, Update, Unmount의 3단계를 useEffect를 사용해서 나타낼 수 있다.
      - setInterval
        - 일정 시간마다 코드를 반복 실행하는 브라우저 내장 함수 (JavaScript 자체 기능)
    - useRef - DOM 직접 접근
    - useContexct - 전역 상태 접슨
    - useMemo - 값 캐싱
    - useCallback - 함수캐싱

  - Hook 규칙?
    - 컴포넌트 최상위에서만 호출 가능
    - React 함수형 컴포넌트 안에서만 호출 가능

- React Router
  - SPA(Single Page Application)
    - 일반웹사이트: 페이지마다 HTML 파일이 따로 존재.
    - SPA: HTML 파일은 하나고, JavaScript로 화면을 바꿈.
  - 왜 사용하는가? -> React는 기본적으로 URL을 인식못하기 때문.
    - URL에 따라 다른 컴포넌트를 보여주려면 React Router가 필요
  - React Router의 역할: URL 변경감지 -> 매칭되는 컴포넌트 렌더링 -> 새로고침 없이 화면 교체
  - NavLink: 활성화 스타일 포함된 Link
    - 현재 URL과 일치하면 자동으로 active 상태가된다. 이를 이용해서 현재 위치한 페이지를 시작적으로 표현.
    - 모든 페이지에서 보이는 메뉴, 사이드바에서 현재 어디에 들어가 있는지 확인할 때 유용
  - 중럽라우트&Qutlet: 페이지 안에 공통 레이아웃이 있고, 그 안에서 또 라우트가 나뉠 때 사용.

### 3. 실습 / 과제 / 결과물

- 실습 코드 : https://github.com/xlouisjungx/2026_FE_Session.git

### 4. 느낀 점 & 다음 계획

- React를 더 활용하기 위해서는 아직 알아야할 부분이 많다고 느꼈다.
- 세션 시간에 배운 부분 외에도 알아야할 부분에 대해 조사해볼 것이다.
