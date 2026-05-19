# 📘 Today I Learned

### 1. 오늘 배운 내용
- React의 생명주기(Mount → Update → Unmount)와 Hook(useState, useEffect)에 대해 배웠다
- React Router를 이용한 SPA 구현 방법을 배웠다
- 실습으로 뽀모도로 타이머를 만들었다 (집중/휴식 카운트다운 + 자동 페이지 전환 + 세션 기록)

### 2. 핵심 정리 (내 언어로)
- -useState를 쓰는 이유: useState를 쓰면 값이 바뀔 때 React가 알아서 화면을 다시 그려준다. 
- useEffect의 의존성 배열: 배열을 안 넣으면 매번 실행, 빈 배열이면 처음 1번만, 값을 넣으면 그 값이 바뀔 때만 실행된다. 타이머처럼 반복 실행하는 건 cleanup(return)으로 꼭 정리해줘야 무한루프나 메모리 누수가 안 생긴다.
- React Router: SPA는 HTML이 하나라서 React 혼자서는 URL을 구분 못 한다. React Router가 URL을 보고 맞는 컴포넌트를 골라서 보여주는 역할을 한다. Link는 사용자가 클릭해서 이동, useNavigate는 코드로 조건 충족 시 자동 이동하는 차이가 있다.
- Context: props를 부모→자식→손자로 계속 내려보내는 게 번거로울 때, Context를 쓰면 어디서든 바로 꺼내 쓸 수 있다. 뽀모도로에서 세션 횟수를 페이지가 바뀌어도 유지하려고 Context를 썼다.
- 뽀모도로 실습: AI에게 프롬프트를 작성해서 구현했다. 직접 코드를 짜진 못했지만, 프롬프트를 쓰려면 "어떤 Hook을 왜 써야 하는지"를 이해해야 해서 교안 내용을 다시 정리하는 계기가 됐다.

### 3. 실습 / 과제 / 결과물
- 코드: React + React Router + Context + Tailwind CSS로 뽀모도로 타이머 구현
- 스크린샷: 디스코드에 업로드

### 4. 느낀 점 & 다음 계획
- 1회차 때보다 React의 구조가 조금씩 보이기 시작했다. useState로 값을 바꾸고 화면이 바뀌는 흐름이 이제 어느 정도 이해된다.
- 아직 useEffect의 의존성 배열이나 cleanup은 직접 쓰려면 헷갈릴 것 같다. 타이머 같은 간단한 예제를 직접 처음부터 짜보면서 연습해야겠다.
- AI 프롬프트를 잘 쓰려면 결국 개념을 알아야 한다는 걸 느꼈다. "useEffect에 setInterval 넣고 cleanup으로 clearInterval 해줘"라고 구체적으로 지시할 수 있었던 건 교안을 읽었기 때문이다.
- 다음 목표는 간단한 컴포넌트라도 AI 없이 직접 작성해보는 것!