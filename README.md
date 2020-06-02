# React Interview Questions & Answers

### Contributor

<a href="https://github.com/SeonHyungJo" target="_blank" rel="nofollow">
	<img src="https://avatars2.githubusercontent.com/u/24274424?s=60&v=4">
</a>
<a href="https://github.com/BKJang" target="_blank" rel="nofollow">
	<img src="https://avatars2.githubusercontent.com/u/24209005?s=60&v=4">
</a>

> * :clipboard: 본 문서는 [sudheerj](https://github.com/sudheerj)의 [reactjs-interview-questions](https://github.com/sudheerj/reactjs-interview-questions)의 번역본입니다.
> * :star: 이 프로젝트가 마음에 드셨다면 **STAR**를 눌러주세요.
> * :heavy_check_mark: 풀 리퀘스트는 언제든 환영입니다.
> * :clap: [vuejs-interview-questions-korean](https://github.com/sudheerj/vuejs-interview-questions-korean)를 참고를 해서 작성하였습니다.

### Table of Contents

| No. | Questions |
| --- | --------- |
|   | **Core React** |
|1  | [React란 무엇인가?](#React란-무엇인가) |
|2  | [React의 주요 특징은?](#React의-주요-특징은) |
|3  | [JSX란 무엇인가?](#JSX란-무엇인가) |
|4  | [Element와 Component의 차이점은?](#element와-component의-차이점은) |
|5  | [React에서 components는 어떻게 만드나?](#React에서-components는-어떻게-만드나) |
|6  | [언제 Function Component 대신에 Class Component를 사용하나?](#언제-Function-Component-대신에-Class-Component를-사용하나) |
|7  | [Pure Components란 무엇인가?](#Pure-Components란-무엇인가) |
|8  | [React에서 state는 무엇인가?](#React에서-state는-무엇인가) |
|9  | [React에서 props는 무엇인가?](#React에서-props는-무엇인가) |
|10 | [state와 prop의 차이점은?](#state와-prop의-차이점은) |
|11 | [왜 state를 직접 update하면 안되나?](#왜-state를-직접-update하면-안되나) |
|12 | [setState()의 argument로 callback 함수를 사용하는 이유는?](#setState()의-argument로-callback-함수를-사용하는-이유는) |
|13 | [HTML과 React의 event handling의 차이점은?](#HTML과-React의-event-handling의-차이점은) |
|14 | [어떻게 JSX 콜백에서 메서드와 이벤트 핸들러를 바인드하나?](#어떻게-JSX-콜백에서-메서드와-이벤트-핸들러를-바인드하나) |
|15 | [어떻게 이벤트 핸들러나 콜백에 매개 변수를 전달하나?](#어떻게-이벤트-핸들러나-콜백에-매개-변수를-전달하나) |
|16 | [React에 SyntheticEvent란 무엇인가?](#React에-SyntheticEvent란-무엇인가) |
|17 | [인라인 조건 표현식이란?](#인라인-조건-표현식이란) |
|18 | ["key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?](#key-props는-무엇이며-elements의-배열에서-사용하면-이점이-무엇인가) |
|19 | [refs는 어떻게 사용되는가?](#refs는-어떻게-사용되는가) |
|20 | [refs는 어떻게 생성하는가?](#refs는-어떻게-생성하는가)
|21 | [forward refs는 무엇인가?](#forward-refs는-무엇인가) |
|22 | [callback refs 및 findDOMNode()에서 선호되는 옵션은?](#callback-refs-및-findDOMNode()에서-선호되는-옵션은) |
|23 | [String Refs가 왜 legacy인가?](#String-Refs가-왜-legacy인가) |
|24 | [Virtual DOM이란?](#Virtual-DOM이란) 
|25 | [Virtual DOM은 어떻게 작동하나?](#Virtual-DOM은-어떻게-작동하나) |
|26 | [Shadow DOM과 Virtual DOM의 차이점](#Shadow-DOM과-Virtual-DOM의-차이점) |
|27 | [React Fiber란?](#React-Fiber란) |
|28 | [React Fiber의 주요 목표는?](#React-Fiber의-주요-목표는) |
|29 | [controlled components란?](#controlled-components란) |
|30 | [uncontrolled components란?](#uncontrolled-components란) |
|31 | [createElement와 cloneElement의 차이점은?](#createElement와-cloneElement의-차이점은?) |
|32 | [React에서 Lifting State Up란?](#React에서-Lifting-State-Up란) |
|33 | [컴포넌트 라이프 사이클의 다른 단계들은?](#컴포넌트-라이프-사이클의-다른-단계들은?) |
|34 | [React의 라이프 사이클 메서드에는 무엇이 있나?](#React의-라이프-사이클-메서드에는-무엇이-있나?) |
|35 | [고차(Higher-Order) 컴포넌트란?](#고차(Higher-Order)-컴포넌트란?) |
|36 | [HOC 컴포넌트를 사용해서 props 프록시를 만드는 방법은?](#HOC-컴포넌트를-사용해서-props-프록시를-만드는-방법은) |
|37 | [context란?](#context란) |
|38 | [children prop이란?](#children-prop이란) |
|39 | [React에서 주석을 어떻게 다는가?](#React에서-주석을-어떻게-다는가) |
|40 | [props argument가 있는 생성자에서 super를 사용하는 목적은 무엇입니까?](#props-argument가-있는-생성자에서-super를-사용하는-목적은-무엇입니까) |
|41 | [조정(reconciliation)이란?](#조정(reconciliation)이란) |
|42 | [state의 키 이름을 동적으로 설정하는 방법은?](#state의-키-이름을-동적으로-설정하는-방법은?) |
|43 | [컴포넌트가 렌더링 될 때마다 호출되는 함수에 대한 실수는 무엇일까?](#컴포넌트가-렌더링-될-때마다-호출되는-함수에-대한-실수는-무엇일까) |
|44 | [왜 컴포넌트 이름은 대문자로 해야 하나?](#왜-컴포넌트-이름은-대문자로-해야-하나) |
|45 | [React는 왜 class가 아닌 className 속성을 사용하나?](#React는-왜-class가-아닌-className-속성을-사용하나?) |
|46 | [fragments란?](#fragments란) |
|47 | [div보다 fragments가 더 우수한 이유는?](#div보다-fragments가-더-우수한-이유는) |
|48 | [React의 portals이란?](#React의-portals이란) |
|49 | [stateless 컴포넌트란?](#stateless-컴포넌트란) |
|50 | [stateful 컴포넌트란?](#stateful-컴포넌트란) |
|51 | [React에서 props 유효성 검사를 적용하는 방법은?](#React에서-props-유효성-검사를-적용하는-방법은) |
|52 | [React의 장점은?](#React의-장점은) |
|53 | [React의 한계는?](#React의-한계는) |
|54 | [React v16에서 error boundaries란 무엇인가?](#React-v16에서-error-boundaries란-무엇인가) 
|55 | [React v15에서는 어떻게 error boundaries 조작하나?](#React-v15에서는-어떻게-error-boundaries-조작하나) |
|56 | [정적 타입 검사에 권장되는 방법은?](#정적-타입-검사에-권장되는-방법은) |
|57 | [react-dom 패키지 사용법은?](#react-dom-패키지-사용법은) |
|58 | [react-dom의 render 메서드란?](#react-dom의-render-메서드란) |
|59 | [ReactDOMServer란?](#ReactDOMServer란) |
|60 | [React에서 innerHTML를 사용하는 방법?](#React에서-innerHTML를-사용하는-방법) |
|61 | [React에서 스타일을 사용하는 방법?](#React에서-스타일을-사용하는-방법) |
|62 | [React에서 이벤트가 어떻게 다른가?](#React에서-이벤트가-어떻게-다른가) |
|63 | [생성자에서 setState()를 사용하면 어떻게 되나?](#생성자에서-setState()를-사용하면-어떻게-되나) |
|64 | [키로 인덱스를 사용하면?](#키로-인덱스를-사용하면) |
|65 | [componentWillMount() 메서드에서 setState()를 사용하는 것은 좋은가?](#componentWillMount()-메서드에서-setState()를-사용하는-것은-좋은가) |
|66 | [초기 state에 props를 사용하면 어떻게 되나?](#초기-state에-props를-사용하면-어떻게-되나) |
|67 | [컴포넌트를 조건부로 렌더링하는 방법?](#컴포넌트를-조건부로-렌더링하는-방법)
|68 | [DOM 엘리먼트에서 spread props를 조심해야하는 이유는?](#DOM-엘리먼트에서-spread-props를-조심해야하는-이유는) 
|69 | [React에서 데코레이터를 사용하는 방법?](#React에서-데코레이터를-사용하는-방법) |
|70 | [컴포넌트를 어떻게 메모하나?](#컴포넌트를-어떻게-메모하나) |
|71 | [Server Side Rendering 또는 SSR 구현방법?](#Server-Side-Rendering-또는-SSR-구현방법) |
|72 | [React에서 production 모드를 사용하는 방법?](#React에서-production-모드를-사용하는-방법) |
|73 | [CRA란 무엇이며 장점은?](#CRA란-무엇이며-장점은) |
|74 | [마운팅의 라이프 사이클 메서드 순서는?](#마운팅의-라이프-사이클-메서드-순서는) |
|75 | [What are the lifecycle methods going to be deprecated in React v16?](#what-are-the-lifecycle-methods-going-to-be-deprecated-in-react-v16) |
|76 | [getDerivedStateFromProps() 라이프 사이클 메서드의 사용 목적은?](#getDerivedStateFromProps()-라이프-사이클-메서드의-사용-목적은) |
|77 | [getSnapshotBeforeUpdate() 라이프 사이클 메서드의 사용 목적은?](#getSnapshotBeforeUpdate()-라이프-사이클-메서드의-사용-목적은) |
|78 | [Hooks는 렌더링 props와 고차원 컴포넌트를 대체한다?](#Hooks는-렌더링-props와-고차원-컴포넌트를-대체한다) |
|79 | [컴포넌트를 명명하는데 권장되는 방법은?](#컴포넌트를-명명하는데-권장되는-방법은) |
|80 | [컴포넌트 클래스에서 권장되는 메서드 순서는?](#컴포넌트-클래스에서-권장되는-메서드-순서는) |
|81 | [스위칭 컴포넌트란?](#스위칭-컴포넌트란) |
|82 | [왜 setState()에 함수를 전달해야 하나?](#왜-setState()에-함수를-전달해야-하나) |
|83 | [React의 strict mode란?](#React의-strict-mode란) |
|84 | [React Mixins이란?](#React-Mixins이란) |
|85 | [왜 isMounted()가 안티 패턴이며 적절한 해결책은?](#왜-isMounted()가-안티-패턴이며-적절한-해결책은) |
|86 | [React에서 지원되는 Pointer Events는?](#React에서-지원되는-Pointer-Events는) |
|87 | [왜 컴포넌트의 이름은 대문자로 시작하나?](#왜-컴포넌트의-이름은-대문자로-시작하나) |
|88 | [React v16에서 사용자 정의 DOM 속성을 지원하나?](#React-v16에서-사용자-정의-DOM-속성을-지원하나) |
|89 | [constructor과 getInitialState의 차이점은?](#constructor과-getInitialState의-차이점은) |
|90 | [setState를 호출하지 않고도 컴포넌트 리렌더링이 가능한가?](#setState를-호출하지-않고도-컴포넌트-리렌더링이-가능한가) |
|91 | [ES6 클래스를 사용하는 React에서 super()와 super(props)의 차이점은?](#ES6-클래스를-사용하는-React에서-super()와-super(props)의-차이점은) |
|92 | [JSX 내부에서 반복하는 방법?](#JSX-내부에서-반복하는-방법) |
|93 | [속성 인용문에 props를 어떻게 넣나?](#속성-인용문에-props를-어떻게-넣나) |
|94 | [모양이 있는 React proptype array란?](#모양이-있는-React-proptype-array란) |
|95 | [클래스 속성을 조건부로 적용하는 방법은?](#클래스-속성을-조건부로-적용하는-방법은) |
|96 | [React와 ReactDOM의 차이점?](#React와-ReactDOM의-차이점) |
|97 | [왜 ReactDOM은 React와 분리되었나?](#왜-ReactDOM은-React와-분리되었나) |
|98 | [React 라벨 엘리먼트를 사용하는 방법은?](#React-라벨-엘리먼트를-사용하는-방법은) |
|99 | [여러 개의 인라인 스타일 객체를 결합하는 방법은?](#여러-개의-인라인-스타일-객체를-결합하는-방법은) |
|100| [브라우저 크기를 조정할 때 뷰를 리렌더링하는 방법은?](#브라우저-크기를-조정할-때-뷰를-리렌더링하는-방법은)
|101| [setState()와 replaceState() 메서드의 차이점은?](#setState()와-replaceState()-메서드의-차이점은) |
|102| [state 변경을 인지하는 방법?](#state-변경을-인지하는-방법) |
|103| [React state에서 배열 엘리먼트를 제거하는 권장 방법은?](#React-state에서-배열-엘리먼트를-제거하는-권장-방법은) |
|104| [HTML 렌더링없이 React를 사용할 수 있나?](#HTML-렌더링없이-React를-사용할-수-있나) |
|105| [React에서 JSON을 이쁘게 출력하는 방법?](#React에서-JSON을-이쁘게-출력하는-방법) |
|106| [React에서 props를 업데이트할 수 없는 이유는?](#React에서-props를-업데이트할-수-없는-이유는) |
|107| [페이지 로드 시 input 엘리먼트에 포커스를 주는 방법은?](#페이지-로드-시-input-엘리먼트에-포커스를-주는-방법은) |
|108| [What are the possible ways of updating objects in state?](#what-are-the-possible-ways-of-updating-objects-in-state) |
|109| [왜 함수가 setState() 객체보다 선호되는가?](#왜-함수가-setState()-객체보다-선호되는가) |
|110| [브라우저 런타임에 React 버전을 어떻게 알 수 있나?](#브라우저-런타임에-React-버전을-어떻게-알-수-있나) |
|111| [create-react-app에 polyfill을 포함시키는 방법은?](#create-react-app에-polyfill을-포함시키는-방법은) |
|112| [create-react-app에서 http 대신 https를 사용하는 방법?](#create-react-app에서-http-대신-https를-사용하는-방법) |
|113| [How to avoid using relative path imports in create-react-app?](#how-to-avoid-using-relative-path-imports-in-create-react-app) |
|114| [React Router용 Google 웹 로그 분석을 추가하는 방법은?](#React-Router용-Google-웹-로그-분석을-추가하는-방법은) |
|115| [매 초마다 컴포넌트를 업데이트 하는 방법은?](#매-초마다-컴포넌트를-업데이트-하는-방법은) |
|116| [React에서 인라인 스타일에 벤더 접두사는 어떻게 적용하나?](#React에서-인라인-스타일에-벤더-접두사는-어떻게-적용하나) |
|117| [React와 ES6를 사용해서 컴포넌트를 가져오고 내보내는 방법은?](#React와-ES6를-사용해서-컴포넌트를-가져오고-내보내는-방법은) |
|118| [React 컴포넌트 이름이 대문자로 시작해야 하는 이유는?](#React-컴포넌트-이름이-대문자로-시작해야-하는-이유는) |
|119| [컴포넌트 생성자는 왜 한 번만 불리나?](#컴포넌트-생성자는-왜-한-번만-불리나) |
|120| [React에서 상수를 정의하는 방법은?](#React에서-상수를-정의하는-방법은) |
|121| [React에서 프로그래밍 방식으로 클릭 이벤트를 발생시키는 방법은?](#React에서-프로그래밍-방식으로-클릭-이벤트를-발생시키는-방법은) |
|122| [async/await를 평범한 React에서 사용할 수 있나?](#async/await를-평범한-React에서-사용할-수-있나) |
|123| [React의 일반적인 폴더 구조는?](#React의-일반적인-폴더-구조는) |
|124| [인기 애니메이션 패키지는?](#인기-애니메이션-패키지는) |
|125| [스타일 모듈의 이점은?](#스타일-모듈의-이점은) |
|126| [인기있는 React-관련 linters는?](#인기있는-React-관련-linters는) |
|127| [AJAX 호출하는 방법과 어느 컴포넌트 라이프 사이클 메서드에서 AJAX 호출을 해야하나?](#AJAX-호출하는-방법과-어느-컴포넌트-라이프-사이클-메서드에서-AJAX-호출을-해야하나?) |
|128| [render props란?](#render-props란) |
|   | **React Router** |
|129| [React Router란?](#React-Router란) |
|130| [React Router가 history 라이브러리와 다른점은?](#React-Router가-history-라이브러리와-다른점은) |
|131| [Router v4의 `<Router>` 컴포넌트는 무엇인가?](#what-are-the-router-components-of-react-router-v4) |
|132| [history의 push, place 메서드의 목적은?](#history의-push-place-메서드의-목적은) |
|133| [React Router v4를 사용하여 프로그래밍 방식으로 어떻게 탐색하나?](#React-Router-v4를-사용하여-프로그래밍-방식으로-어떻게-탐색하나) |
|134| [React Router v4에서 쿼리 매개 변수를 얻는 방법은?](#React-Router-v4에서-쿼리-매개-변수를-얻는-방법은) |
|135| [왜 Router may have only one child element라는 경고 메시지가 나오나?](#왜-Router-may-have-only-one-child-element라는-경고-메시지가-나오나) |
|136| [React Router v4의 history.push 메서드에 매개 변수를 전달하는 방법은?](#React-Router-v4의-`history.push`-메서드에-매개-변수를-전달하는-방법은) |
|137| [default 또는 NotFound 페이지 구현 방법?](#default-또는-NotFound-페이지-구현-방법) |
|138| [React Router v4에서 history를 얻는 방법은?](#React-Router-v4에서-history를-얻는-방법은) |
|139| [로그인 후 자동 리디렉션을 수행하는 방법은?](#로그인-후-자동-리디렉션을-수행하는-방법은) |
|   | **React Internationalization** |
|140| [What is React-Intl?](#what-is-react-intl) |
|141| [What are the main features of React Intl?](#what-are-the-main-features-of-react-intl) |
|142| [What are the two ways of formatting in React Intl?](#what-are-the-two-ways-of-formatting-in-react-intl) |
|143| [How to use FormattedMessage as placeholder using React Intl?](#how-to-use-formattedmessage-as-placeholder-using-react-intl) |
|144| [How to access current locale with React Intl](#how-to-access-current-locale-with-react-intl) |
|145| [How to format date using React Intl?](#how-to-format-date-using-react-intl) |
|   | **React Testing** |
|146| [What is Shallow Renderer in React testing?](#what-is-shallow-renderer-in-react-testing) |
|147| [What is TestRenderer package in React?](#what-is-testrenderer-package-in-react) |
|148| [What is the purpose of ReactTestUtils package?](#what-is-the-purpose-of-reacttestutils-package) |
|149| [What is Jest?](#what-is-jest) |
|150| [What are the advantages of Jest over Jasmine?](#what-are-the-advantages-of-jest-over-jasmine) |
|151| [Give a simple example of Jest test case](#give-a-simple-example-of-jest-test-case) |
|   | **React Redux** |
|152| [flux란?](#flux란) |
|153| [Redux란?](#redux란) |
|154| [Redux의 핵심 원칙은?](#redux의-핵심-원칙은) |
|155| [Flux와 비교한 Redux의 단점은?](#flux와-비교한-redux의-단점은) |
|156| [mapStateToProps()과 mapDispatchToProps()의 차이점은?](#mapstatetoprops과-mapdispatchtoprops의-차이점은?) |
|157| [reducer에서 action을 전달할 수 있나?](#reducer에서-action을-전달할-수-있나) |
|158| [컴포넌트 외부의 Redux store에 접근하는 방법은?](#컴포넌트-외부의-Redux-store에-접근하는-방법은) |
|159| [MVW 패턴의 단점은 무엇인가](#MVW-패턴의-단점은-무엇인가) |
|160| [Redux와 RxJS의 비슷한 점은?](#Redux와-RxJS의-비슷한-점은) |
|161| [로드 시점에 action을 전달하는 방법은?](#로드-시점에-action을-전달하는-방법은) |
|162| [React Redux에서 connect()를 사용하는 방법은?](#React-Redux에서-connect()를-사용하는-방법은) |
|163| [Redux에서 state를 재설정하는 방법은?](#Redux에서-state를-재설정하는-방법은) |
|164| [Whats the purpose of at symbol in the redux connect decorator?](#whats-the-purpose-of-at-symbol-in-the-redux-connect-decorator) |
|165| [React context와 React Redux의 차이점은?](#React-context와-React-Redux의-차이점은) |
|166| [Redux state 함수가 reducer라고 불리는 이유는?](#Redux-state-함수가-reducer라고-불리는-이유는) |
|167| [Redux에서 AJAX를 요청하는 방법은?](#Redux에서-AJAX를-요청하는-방법은) |
|168| [Should I keep all component's state in Redux store?](#should-i-keep-all-components-state-in-redux-store) |
|169| [Redux store에 접근하는 올바른 방법은?](#Redux-store에-접근하는-올바른-방법은) |
|170| [React Redux에서 컴포넌트와 컨테이너의 차이점은?](#React-Redux에서-컴포넌트와-컨테이너의-차이점은) |
|171| [Redux에서 상수의 목적은 무엇인가?](#Redux에서-상수의-목적은-무엇인가) |
|172| [mapDispatchToProps()를 작성하는 다른 방법은?](#mapdispatchtoprops를-작성하는-다른-방법은) |
|173| [mapStateToProps() 과 mapDispatchToProps()에서 ownProps 매개 변수의 사용방법은?](#mapstatetoprops-과-mapdispatchtoprops에서-ownProps-매개-변수의-사용방법은) |
|174| [Redux 최상위 디렉토리를 구성하는 방법은?](#Redux-최상위-디렉토리를-구성하는-방법은) |
|175| [redux-saga란?](#redux-saga란) |
|176| [redux-saga의 정신 모델은?](#redux-saga의-정신-모델은) |
|177| [redux-saga에서 call과 put의 차이점은?](#redux-saga에서-call과-put의-차이점은) |
|178| [Redux Thunk란?](#Redux-Thunk란) |
|179| [redux-saga와 redux-thunk의 차이점은?](#redux-saga와-redux-thunk의-차이점은) |
|180| [Redux DevTools이란?](#Redux-DevTools이란) |
|181| [Redux DevTools의 기능에는 무엇이 있나?](#Redux-DevTools의-기능에는-무엇이-있나) |
|182| [Redux selectors가 무엇이며 사용해야하는 이유는?](#Redux-selectors가-무엇이며-사용해야하는-이유는) |
|183| [Redux Form이란?](#Redux-Form이란) |
|184| [Redux Form의 주요 기능은?](#Redux-Form의-주요-기능은) |
|185| [Redux에 여러 미들웨어를 추가하는 방법은?](#Redux에-여러-미들웨어를-추가하는-방법은) |
|186| [Redux에서 초기 state를 설정하는 방법은?](#Redux에서-초기-state를-설정하는-방법은) |
|187| [Relay와 Redux의 차이점은?](#Relay와-Redux의-차이점은) |
|   | **React Native** |
|188| [What is the difference between React Native and React?](#what-is-the-difference-between-react-native-and-react) |
|189| [How to test React Native apps?](#how-to-test-react-native-apps) |
|190| [How to do logging in React Native?](#how-to-do-logging-in-react-native) |
|191| [How to debug your React Native?](#how-to-debug-your-react-native) |
|   | **React supported libraries and Integration** |
|192| [reselect이란 무엇이며 어떻게 작동하나?](#reselect이란-무엇이며-어떻게-작동하나) |
|193| [Flow란?](#what-is-flow) |
|194| [Flow와 PropTypes의 차이점은?](#Flow와-PropTypes의-차이점은) |
|195| [React에서 Font Awesome icons를 어떻게 사용하나?](#React에서-Font-Awesome-icons를-어떻게-사용하나) |
|196| [React Dev Tools이란?](#React-Dev-Tools이란) |
|197| [로컬 파일을 연 Chrome에서 DevTools이 로딩되지 않는 이유는?](#로컬-파일을-연-Chrome에서-DevTools이-로딩되지-않는-이유는) |
|198| [React에서 Polymer를 사용하는 방법은?](#React에서-Polymer를-사용하는-방법은) |
|199| [Vue.js보다 React의 장점은 무엇인가?](#Vue.js보다-React의-장점은-무엇인가) |
|200| [React와 Angular의 차이점은?](#React와-Angular의-차이점은) |
|201| [DevTools에 React 탭이 표시되지 않는 이유는?](#DevTools에-React-탭이-표시되지-않는-이유는) |
|202| [Styled Components란?](#Styled-Components란) |
|203| [Styled Components의 예시는?](#Styled-Components의-예시는) |
|204| [Relay란?](#Relay란) |
|205| [create-react-app 애플리케이션에서 TypeScript를 사용하는 방법?](#create-react-app-애플리케이션에서-TypeScript를-사용하는-방법) |
|   | **Miscellaneous** |
|206| [Reselect 라이브러리의 주요 기능은?](#Reselect-라이브러리의-주요-기능은) |
|207| [Reselect 사용법에 대한 예시는?](#Reselect-사용법에-대한-예시는) |
|208| [Redux에서 action이란?](#Redux에서-action이란) |
|209| [React의 ES6 클래스는 static object와 함께 사용 가능한가?](#React의-ES6-클래스는-static-object와-함께-사용-가능한가?) |
|210| [Redux는 React에서만 사용 가능한가?](#Redux는-React에서만-사용-가능한가) |
|211| [Redux를 사용하기 위한 특별한 빌드 도구가 필요한가?](#Redux를-사용하기-위한-특별한-빌드-도구가-필요한가) |
|212| [Redux Form `initialValues`는 state에서 어떻게 업데이트하나?](#Redux-Form-initialValues는-state에서-어떻게-업데이트하나) |
|213| [React PropTypes이 하나의 prop에서 다른 타입들을 허용하는 방법은?](#React-PropTypes이-하나의-prop에서-다른-타입들은-허용하는-방법은) |
|214| [SVG file을 react 컴포넌트로 가져올 수 있나?](#SVG-file을-react-컴포넌트로-가져올-수-있나) |
|215| [인라인 ref 콜백 또는 함수를 권장하지 않는 이유는?](#인라인-ref-콜백-또는-함수를-권장하지-않는-이유는)|
|216| [react에서 render hijacking이란?](#react에서-render-hijacking이란)|
|217| [HOC 팩토리 구현이란?](#HOC-팩토리-구현이란)|
|218| [React 컴포넌트에 숫자를 전달하는 방법은?](#React-컴포넌트에-숫자를-전달하는-방법은)|
|219| [모든 state를 Redux에서 관리를 해야하나? react 내부 state를 사용해야하나?](#모든-state를-Redux에서-관리를-해야하나-react-내부-state를-사용해야하나)|
|220| [React에서 registerServiceWorker의 목적은?](#React에서-registerServiceWorker의-목적은)|
|221| [React의 memo 함수란?](#React의-memo-함수란)|
|222| [React의 lazy function란?](#React의-lazy-function란)|
|223| [setState를 사용하는데 있어 불필요한 업데이트를 방지하는 방법은?](#setState를-사용하는데-있어-불필요한-업데이트를-방지하는-방법은?)|
|224| [React 16버전에서 Array, Strings와 Numbers를 렌더링하는 방법은?](#React-16버전에서-Array,-Strings와-Numbers를-렌더링하는-방법은)|
|225| [React 클래스에서 클래스 필드 선언 구문을 사용하는 방법은?](#React-클래스에서-클래스-필드-선언-구문을-사용하는-방법은)|
|226| [hooks이란?](#hooks이란)|
|227| [hooks를 위해서 지켜야 하는 규칙은 무엇인가?](#hooks를-위해서-지켜야-하는-규칙은-무엇인가)|
|228| [hooks가 프로젝트의 규칙을 준수하도록 하는 방법은?](#hooks가-프로젝트의-규칙을-준수하도록-하는-방법은)|
|229| [Flux와 Redux의 차이점은?](#Flux와-Redux의-차이점은)|
|230| [React Router V4의 장점은?](#React-Router-V4의-장점은)|
|231| [componentDidCatch 생명주기 메서드에 대해서 설명할 수 있나?](#componentDidCatch-생명주기-메서드에-대해서-설명할-수-있나)|
|232| [어떤 에러 바운더리(error boundary)에서 잡지 못할까?](#어떤-에러-바운더리(error-boundary)에서-잡지-못할까?)|
|233| [이벤트 핸들러에 에러 바운더리가 필요하지 않은 이유는?](#이벤트-핸들러에-에러-바운더리가-필요하지-않은-이유는)|
|234| [try catch 블록과 에러 바운더리의 차이점은?](#try-catch-블록과-에러-바운더리의-차이점은)|
|235| [react 16에서 잡히지 않는 오류의 동작은?](#react-16에서-잡히지-않는-오류의-동작은)|
|236| [에러 바운더리의 적절한 위치는?](#에러-바운더리의-적절한-위치는)|
|237| [에러 바운더리에서 컴포넌트 스택 추적의 장점은?](#에러-바운더리에서-컴포넌트-스택-추적의-장점은)|
|238| [클래스 컴포넌트에 정의해야 하는 메서드는 무엇인가?](#클래스-컴포넌트에-정의해야-하는-메서드는-무엇인가)|
|239| [render 메서드의 return 가능한 타입은?](#render-메서드의-return-가능한-타입은)|
|240| [constructor의 주요 목적은?](#constructor의-주요-목적은)|
|241| [React 컴포넌트의 생성자를 정의해야 하나?](#React-컴포넌트의-생성자를-정의해야-하나)|
|242| [default props란?](#default-props란)|
|243| [componentWillUnmount에서 setState를 호출하면 안되는 이유는?](#componentWillUnmount에서-setState를-호출하면-안되는-이유는)|
|244| [getDerivedStateFromError의 목적은?](#getDerivedStateFromError의-목적은)|
|245| [리렌더링할 때 메서드의 순서는?](#리렌더링할-때-메서드의-순서는)|
|246| [에러 핸들링 중 호출되는 메서드는?](#에러-핸들링-중-호출되는-메서드는)|
|247| [displayName 클래스 속성의 목적은?](#displayName-클래스-속성의-목적은)|
|248| [react 응용프로그램의 브라우저 지원은 어디까지인가?](#react-응용프로그램의-브라우저-지원은-어디까지인가)|
|249| [unmountComponentAtNode 메서드의 목적은?](#unmountComponentAtNode-메서드의-목적은)|
|250| [code-splitting이란?](#code-splitting이란)|
|251| [strict mode의 장점은?](#strict-mode의-장점은)|
|252| [Keyed Fragments란?](#Keyed-Fragments란)|
|253| [React는 모든 HTML 속성을 지원하나?](#React는-모든-HTML-속성을-지원하나)|
|254| [HOC의 한계는?](#HOC의-한계는)|
|255| [개발자 도구에서 forwardRefs를 디버깅하는 방법은?](#개발자-도구에서-forwardRefs를-디버깅하는-방법은)|
|256| [컴포넌트 props의 기본값은 true인가?](#컴포넌트-props의-기본값은-true인가)|
|257| [NextJS는 무엇이며, 주요한 기능은?](#NextJS는-무엇이며,-주요한-기능은)|
|258| [이벤트 핸들러를 컴포넌트에 어떻게 전달하나?](#이벤트-핸들러를-컴포넌트에-어떻게-전달하나)|
|259| [render 메서드에서 화살표 함수를 사용하는 것이 좋은가?](#render-메서드에서-화살표-함수를-사용하는-것이-좋은가)|
|260| [함수가 여러 번 호출되는 것을 방지하는 방법은?](#함수가-여러-번-호출되는-것을-방지하는-방법은)|
|261| [JSX가 Injection 공격은 막는 방법은?](#JSX가-Injection-공격은-막는-방법은)|
|262| [렌더링 된 요소는 어떻게 업데이트하나?](#렌더링-된-요소는-어떻게-업데이트하나)|
|263| [props가 읽기 전용이어야 하는 이유는?](#props가-읽기-전용이어야-하는-이유는)|
|264| [state updates가 어떻게 병합되나?](#state-updates가-어떻게-병합되나?)|
|265| [이벤트 핸들러에 인수를 어떻게 넘기나?](#이벤트-핸들러에-인수를-어떻게-넘기나)|
|266| [컴포넌트 렌더링을 막는 방법은?](#컴포넌트-렌더링을-막는-방법은)|
|267| [index를 키로 안전하게 사용하기 위한 조건은?](#index를-키로-안전하게-사용하기-위한-조건은)|
|268| [키가 전체에서 고유해야 하나?](#키가-전체에서-고유해야-하나)|
|269| [Form 처리에 가장 많이 사용되는 선택지는?](#Form-처리에-가장-많이-사용되는-선택지는)|
|270| [redux form 라이브러리보다 formik의 장점은?](#redux-form-라이브러리보다-formik의-장점은)|
|271| [상속할 필요가 없는 이유는?](#상속할-필요가-없는-이유는)|
|272| [react 애플리케이션에서 웹 컴포넌트를 사용할 수 있나?](#react-애플리케이션에서-웹-컴포넌트를-사용할-수-있나)|
|273| [dynamic import란?](#dynamic-import란)|
|274| [loadable 컴포넌트란?](#loadable-컴포넌트란)|
|275| [suspense 컴포넌트란?](#suspense-컴포넌트란)|
|276| [라우트 기반의 코드 스플리팅이란?](#라우트-기반의-코드-스플리팅이란)|
|277| [context를 어떻게 사용하는지에 대한 예제](#context를-어떻게-사용하는지에-대한-예제)|
|278| [context에서 기본값의 목적은?](#context에서-기본값의-목적은)|
|279| [contextType은 어떻게 사용하나?](#contextType은-어떻게-사용하나)|
|280| [consumer란?](#consumer란)|
|281| [How do you solve performance corner cases while using context?](#how-do-you-solve-performance-corner-cases-while-using-context)|
|282| [What is the purpose of forward ref in HOCs?](#what-is-the-purpose-of-forward-ref-in-hocs)|
|283| [Is it ref argument available for all functions or class components?](#is-it-ref-argument-available-for-all-functions-or-class-components)|
|284| [Why do you need additional care for component libraries while using forward refs?](#why-do-you-need-additional-care-for-component-libraries-while-using-forward-refs)|
|285| [How to create react class components without ES6?](#how-to-create-react-class-components-without-es6)|
|286| [Is it possible to use react without JSX?](#is-it-possible-to-use-react-without-jsx)|
|287| [What is diffing algorithm?](#what-is-diffing-algorithm)|
|288| [diffing 알고리즘에 적용되는 규칙은?](#diffing-알고리즘에-적용되는-규칙은)|
|289| [When do you need to use refs?](#when-do-you-need-to-use-refs)|
|290| [Is it prop must be named as render for render props?](#is-it-prop-must-be-named-as-render-for-render-props)|
|291| [What are the problems of using render props with pure components?](#what-are-the-problems-of-using-render-props-with-pure-components)|
|292| [How do you create HOC using render props?](#how-do-you-create-hoc-using-render-props)|
|293| [What is windowing technique?](#what-is-windowing-technique)|
|294| [How do you print falsy values in JSX?](#how-do-you-print-falsy-values-in-jsx)|
|295| [What is the typical use case of portals?](#what-is-the-typical-use-case-of-portals?)|
|296| [How do you set default value for uncontrolled component?](#how-do-you-set-default-value-for-uncontrolled-component)|
|297| [What is your favorite React stack?](#what-is-your-favorite-react-stack)|
|298| [What is the difference between Real DOM and Virtual DOM?](#what-is-the-difference-between-real-dom-and-virtual-dom)|
|299| [How to add Bootstrap to a react application?](#how-to-add-bootstrap-to-react-application)|
|300| [Can you list down top websites or applications using react as front end framework?](#can-you-list-down-top-websites-or-applications-using-react-as-front-end-framework)|
|301| [Is it recommended to use CSS In JS technique in React?](#is-it-recommended-to-use-css-in-js-technique-in-react)|
|302| [Do I need to rewrite all my class components with hooks?](#do-i-need-to-rewrite-all-my-class-components-with-hooks)|
|303| [How to fetch data with React Hooks?](#how-to-fetch-data-with-react-hooks)|
|304| [Is Hooks cover all use cases for classes?](#is-hooks-cover-all-use-cases-for-classes)|
|305| [What is the stable release for hooks support?](#what-is-the-stable-release-for-hooks-support)|
|306| [Why do we use square brackets in useState?](#why-do-we-use-square-brackets-in-usestate)|
|307| [What are the sources used for introducing hooks?](#what-are-the-sources-used-for-introducing-hooks)|
|308| [How do you access imperative API of web components?](#how-do-you-access-imperative-api-of-web-components)|
|309| [What is formik?](#what-is-formik)|
|310| [What are typical middleware choices for handling asynchronous calls in Redux?](#what-are-typical-middleware-choices-for-handling-asynchronous-calls-in-redux)|
|311| [Is browsers understand JSX code?](#is-browsers-understand-jsx-code)|
|312| [Describe about data flow in react?](#describe-about-data-flow-in-react)|
|313| [What is react scripts?](#what-is-react-scripts)|
|314| [What are the features of create react app?](#what-are-the-features-of-create-react-app)|
|315| [What is the purpose of renderToNodeStream method?](#what-is-the-purpose-of-rendertonodestream-method)|
|316| [What is MobX?](#what-is-mobx)|
|317| [What are the differences between Redux and MobX?](#what-are-the-differences-between-redux-and-mobx)|
|318| [Should I learn ES6 before learning ReactJS?](#should-i-learn-es6-before-learning-reactjs)|
|319| [What is Concurrent Rendering?](#what-is-concurrent-rendering)|
|320| [What is the difference between async mode and concurrent mode?](#what-is-the-difference-between-async-mode-and-concurrent-mode)|
|321| [Can I use javascript urls in react16.9?](#can-i-use-javascript-urls-in-react16.9)|
|322| [What is the purpose of eslint plugin for hooks?](#what-is-the-purpose-of-eslint-plugin-for-hooks)|
|323| [What is the difference between Imperative and Declarative in React?](#what-is-the-difference-between-imperative-and-declarative-in-react)|
|324| [What are the benefits of using typescript with reactjs?](#what-are-the-benefits-of-using-typescript-with-reactjs)|

## Core React

1. ### React란 무엇인가?

    React는 단일 페이지 어플리케이션으로 UI(user interface)를 만드는데 사용되는 **오픈-소스 프론트엔드 JavaScript 라이브러리** 로 웹과 모바일 앱에서 view layer를 다루는데 사용된다. React는 Facebook에서 소프트웨어 엔지니어로 있는 Jordan Walke가 만들었다. React는 2011년 Facebook's News Feed, 2012년 Instagram에서 처음 선보였다.

2. ### React의 주요 특징은?

    React의 주요 특징은 :

    * 실제돔(RealDOM)을 조작하는 것은 비용이 크다는 것을 고려하여 실제돔 대신에 **가상돔(VirtualDOM)** 을 사용한다.
    * **서버-사이드 렌더링(server-side rendering)** 를 지원한다.
    * **단방향** 데이터 흐름 또는 데이터 바인딩을 따른다.
    * 화면 개발을 위해 **재사용 가능한(reusable)/구성 가능한(composable)** UI 컴포넌트를 사용한다.

3. ### JSX란 무엇인가?

    *JSX* 는 ECMAScript를 위한 XML-처럼 생긴 구문 확장자(*JavaScript XML* 의 약어)이다. 기본적으로 `React.createElement()` 함수를 위한 syntactic sugar, JavaScript의 표현력과 HTML같은 템플릿 문법을 제공한다.

    아래 예제에서 `<h1>` 태그 안의 텍스트는 render 함수에 JavaScript 함수로 반환된다.

    ```jsx harmony
    class App extends React.Component {
      render() {
        return(
          <div>
            <h1>{'Welcome to React world!'}</h1>
          </div>
        )
      }
    }
    ```

4. ### Element와 Component의 차이점은?

    *Element* 는 DOM 노드나 다른 컴포넌트들 관점에서 화면에 보이기 원하는 걸 묘사한 일반 객체이다. *Elements* 는 props에 있는 다른 *Elements* 를 포함할 수 있다. React element를 만드는 것은 저렴하다. 일단 element가 만들어지면 절대 변경되지 않는다.

    React Element 객체 표현은 다음과 같다. :

    ```javascript
    const element = React.createElement(
      'div',
      {id: 'login-btn'},
      'Login'
    )
    ```

    위의 `React.createElement()` 함수는 객체를 반환한다. :

    ```
    {
      type: 'div',
      props: {
        children: 'Login',
        id: 'login-btn'
      }
    }
    ```

    마지막으로 `ReactDOM.render()` 를 사용해서 DOM으로 렌더링한다. :

    ```html
    <div id='login-btn'>Login</div>
    ```

    반면에 **component** 는 여러 다른 방법으로 선언될 수 있다. `render()` 메소드를 포함한 클래스가 될 수 있다. 또는 단순하게 함수로 정의될 수 있다. 두 경우 모두, 입력으로 props를 가져오고, 출력으로 JSX tree를 return한다.

    ```javascript
    const Button = ({ onLogin }) =>
      <div id={'login-btn'} onClick={onLogin}>Login</div>
    ```

    JSX는 `React.createElement()` 함수 트리로 변환된다. :

    ```javascript
    const Button = ({ onLogin }) => React.createElement(
      'div',
      { id: 'login-btn', onClick: onLogin },
      'Login'
    )
    ```

5. ### React에서 components는 어떻게 만드나?

    컴포넌트를 만드는 방법은 2가지가 있다.

    1. **Function Components:** 컴포넌트를 만드는 가장 간단한 방법이다. 순수 JavaScript functions 로 첫번째 인자로는 props 객체를 받고 React elements를 반환한다. : 

        ```jsx harmony
        function Greeting({ message }) {
          return <h1>{`Hello, ${message}`}</h1> 
        }
        ```

    2. **Class Components:** ES6의 class를 사용해서 컴포넌트를 만들 수 있다. 위의 함수는 다음과 같이 작성될 수 있다. :

        ```jsx harmony
        class Greeting extends React.Component {
          render() {
            return <h1>{`Hello, ${this.props.message}`}</h1>
          }
        }
        ```

6. ### 언제 Function Component 대신에 Class Component를 사용하나?

    만약, 컴포넌트가 `state나 lifecycle methods`가 필요하다면 class 컴포넌트를 사용하고 아니라면 function 컴포넌트를 사용한다.
    
7. ### Pure Components란 무엇인가?

    *`React.PureComponent`* 는 `shouldComponentUpdate()` 메서드를 제어하는 것을 제외하면 *`React.Component`*와 다르지 않다. props나 state가 변경되면 *PureComponent* 는 props와 state 에 대해서 얕은 비교를 수행한다. 반면에 *Component* 는 현재의 props와 state에 대해 비교를 하지 않는다. 따라서 `shouldComponentUpdate`가 호출될 때마다 리렌더링된다.
    
8. ### React에서 state는 무엇인가?

    컴포넌트의 *State*는 컴포넌트의 변경 될 수 있는 정보를 보유하는 객체이다. 가능한 한 간단하게 상태를 만들고 stateful 컴포넌트의 수를 최소화해야 한다. message state를 가진 User 컴포넌트를 만들어보자.

    ```jsx harmony
    class User extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          message: 'Welcome to React world'
        }
      }

      render() {
        return (
          <div>
            <h1>{this.state.message}</h1>
          </div>
        )
      }
    }
    ```

    ![state](images/state.jpg)

    state는 props와 비슷하지만 private 하며 컴포넌트에 의해 제어된다. 즉, 상태는 이를 가지고 있거나 설정할 수 있는 컴포넌트 이외에는 접근할 수 없다.

9. ### React에서 props는 무엇인가?

      *Props*는 컴포넌트에 대한 입력이다. Props는 HTML 태그 속성과 같은 작명 규칙을 사용하여 컴포넌트에 전달되는 단일 값 혹은 객체다. props는 부모 컴포넌트에서 자식 컴포넌트로 전달된다.

      React에서 props의 주목적은 다음과 같은 컴포넌트의 기능들을 제공하는 것이다.

      1. 커스텀 데이터를 컴포넌트로 전달한다.
      2. state의 변경을 일으킨다.
      3. 컴포넌트의 `render()` 메서드 내에서 `this.props.reactProp` 를 통해 사용한다.

      예를 들어 `reactProp` 요소를 가진 엘리먼트를 만들어보자.

    ```jsx harmony
    <Element reactProp={'1'} />
    ```
    
    이 `reactProp` (또는 여러분이 만든 것은 무엇이든) React를 사용하여 생성된 모든 컴포넌트에 원래 존재하는 props 객체의 속성이 된다.

    ```
    props.reactProp
    ```

10. ### state와 prop의 차이점은?

    *props*와 *state*는 모두 순수 자바스크립트 객체다. 둘 다 렌더링 결과에 영향을 주는 정보를 가지고 있지만, 컴포넌트와 관련된 기능 면에서 다르다. props는 함수의 매개변수와 비슷하게 컴포넌트로 전달되는 반면, state는 함수 내에서 선언된 변수와 유사하게 컴포넌트 내에서 관리된다.

11. ### 왜 state를 직접 update하면 안되나?

    혹시라도 state를 직접적으로 업데이트를 하게 되면 컴포넌트는 re-render를 하지 않는다.

    ```javascript
    //Wrong
    this.state.message = 'Hello world'
    ```

    대신에 `setState()` 메소드를 사용한다. 이 메소드는 컴포넌트의 state 객체에 대한 업데이트를 예약한다. state가 바뀌게 되면, 컴포넌트는 re-rendering으로 응답을 한다.

    ```javascript
    //Correct
    this.setState({ message: 'Hello World' })
    ```

    **Note:** *constructor*에서나 최신 Javascript의 class 선언 구문을 사용해서 state 객체에 직접 할당할 수 있다.

12. ### `setState()`의 argument로 callback 함수를 사용하는 이유는?

    callback 함수는 setState가 끝나고 컴포넌트가 render 되었을 때 작동한다. `setState()`는 **비동기식**이여서 callback 함수는 모든 작업 후 사용된다.

    **Note:** 이 callback 함수보다는 lifecycle 메소드를 사용하는 것이 좋다.

    ```javascript
    setState({ name: 'John' }, () => console.log('The name has updated and component re-rendered'))
    ```

13. ### HTML과 React의 event handling의 차이점은?

    1. HTML에서, 이벤트 이름은 *소문자*여야 한다:

    ```html
    <button onclick='activateLasers()'>
    ```

    반면에 React에서는 *camelCase* 규칙을 따른다:

    ```jsx harmony
    <button onClick={activateLasers}>
    ```

    1.  HTML에서, 기본 동작 방지를 위해 `false`를 반환할 수 있다:

    ```html
    <a href='#' onclick='console.log("The link was clicked."); return false;' />
    ```

    반면에 React에서는 `preventDefault()`를 명시적으로 호출해야 한다:

    ```javascript
    function handleClick(event) {
      event.preventDefault()
      console.log('The link was clicked.')
    }
    ```

14. ### 어떻게 JSX 콜백에서 메서드와 이벤트 핸들러를 바인드하나?

    이를 이루기 위한 3가지 방법이 있다.

    1.	**생성자에서 바인딩:** JavaScript 클래스에서, 메서드는 기본적으로 바인딩 되지 않는다. 클래스 메서드로 정의된 React  이벤트 핸들러에게서도 똑같은 문제가 적용된다. 일반적으로 우리는 생성자 안에서 바인드를 한다.

    ```javascript
    class Component extends React.Componenet {
      constructor(props) {
        super(props)
        this.handleClick = this.handleClick.bind(this)
      }

      handleClick() {
        // ...
      }
    }
    ```

    1. **Public 클래스 필드 구문:** 바인드 접근법이 싫다면 콜백을 올바르게 바인드하기 위해 *public 클래스 필드 구문* 을 사용할 수 있다.

    ```jsx harmony
    handleClick = () => {
      console.log('this is:', this)
    }
    ```

    ```jsx harmony
    <button onClick={this.handleClick}>
      {'Click me'}
    </button>
    ```

    1. **콜백 안에서 화살표 함수:** 콜백 안에서 직접 *화살표 함수*를 사용할 수 있다.

    ```jsx harmony
    <button onClick={(event) => this.handleClick(event)}>
      {'Click me'}
    </button>
    ```

    **Note:** 콜백이 자식 컴포넌트에 prop으로 전달이 되면, 해당 컴포넌트는 추가 리렌더링을 수행할 수 있다. 이 경우에, 성능을 고려하여 `.bind()` 또는 *public 클래스 필드 구문* 접근법을 사용하는 것이 좋다.

15. ### 어떻게 이벤트 핸들러나 콜백에 매개 변수를 전달하나?

    *화살표 함수*를 사용해서 *이벤트 핸들러*를 감싸고 매개변수를 전달할 수 있다.

    ```jsx harmony
    <button onClick={() => this.handleClick(id)} />
    ```

    `.bind`를 호출하는 것과 동일하다:

    ```jsx harmony
    <button onClick={this.handleClick.bind(this, id)} />
    ```
    Apart from these two approaches, you can also pass arguments to a function which is defined as array function
    ```jsx harmony
    <button onClick={this.handleClick(id)} />
    handleClick = (id) => () => {
        console.log("Hello, your ticket number is", id)
    };
    ```

16. ### React에 SyntheticEvent란 무엇인가?

    `SyntheticEvent`는 브라우저의 기본 이벤트를 감싼 cross-browser wrapper이다. `stopPropagation()`과 `preventDefault()`를 포함한 API로, 브라우저의 기본 이벤트와 동일하지만, 모든 브라우저에서 동일하게 작동한다는 점이 다르다.

17. ### 인라인 조건 표현식이란?

    JS에서 조건부로 식을 표현하기 위해서 *if 문* 이나 *삼항 표현식* 을 사용할 수 있다. 이러한 접근법 외에도, JS 논리연산자인 `&&`가 있는 중괄호로 감싼 표현식을 JSX에 포함할 수도 있다.

    ```jsx harmony
    <h1>Hello!</h1>
    {
        messages.length > 0 && !isLogin?
          <h2>
              You have {messages.length} unread messages.
          </h2>
          :
          <h2>
              You don't have unread messages.
          </h2>
    }
    ```

18. ### "key" props는 무엇이며 elements의 배열에서 사용하면 이점이 무엇인가?

    `key`는 elements 배열을 만들 때 포함**시켜야 하는** 특수 문자열 속성이다. *Keys*는 React가 변경, 추가, 제거된 항목을 식별하는 데 도움을 준다.

    우리는 대개 데이터에서 ID를 *keys*로 사용한다.

    ```jsx harmony
    const todoItems = todos.map((todo) =>
      <li key={todo.id}>
        {todo.text}
      </li>
    )
    ```

    렌더링된 항목 중 안정적인 ID가 없을 때, 마지막 수단으로 항목의 *index*를 *key*로 사용할 수 있다.

    ```jsx harmony
    const todoItems = todos.map((todo, index) =>
      <li key={index}>
        {todo.text}
      </li>
    )
    ```

    **Note:**

    1. 항목의 순서가 변경될 수 있는 경우 *index*를 *keys*로 사용하는 것은 **추천하지 않는다.** 이는 성능 저하와 컴포넌트 state에 문제를 발생시킬 수 있다.
    2. 리스트 항목을 별도의 컴포넌트로 추출하는 경우 `li` 태그 대신에 리스트 컴포넌트에 *keys*를 적용해라.
    3. 리스트 항목에 `key` prop가 없으면 console에 경고 메시지가 표시될 것이다.

19. ### refs는 어떻게 사용되는가?

    *ref*는 엘리먼트에 대한 참조를 반환하는 데 사용된다. 대부분의 경우에서 *피하는 것이 좋지만*, DOM 엘리먼트나 컴포넌트의 인스턴스에 직접 접근하는 경우 유용할 수 있다.

20. ### refs는 어떻게 생성하는가?

    refs를 생성하는 방법에는 2가지 방법이 있다.
    1. 다음은 최근에 추가된 방법이다. *Refs*는 `React.createRef()`메서드를 통해 생성되며 `ref` 속성을 통해 React 엘리먼트에 적용된다. 엘리먼트 전체에서 *refs*를 사용하려면 생성자 내의 인스턴스 속성에 *ref*를 할당하면 된다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        this.myRef = React.createRef()
      }
      render() {
        return <div ref={this.myRef} />
      }
    }
    ```
    1. React 버전에 관계없이 ref 콜백 접근법을 사용할 수도 있다. 예를 들어, 검색창 컴포넌트의 입력 엘리먼트에서는 다음과 같이 접근한다.
    ```jsx harmony
    class SearchBar extends Component {
       constructor(props) {
          super(props);
          this.txtSearch = null;
          this.state = { term: '' };
          this.setInputSearchRef = e => {
             this.txtSearch = e;
          }
       }
       onInputChange(event) {
          this.setState({ term: this.txtSearch.value });
       }
       render() {
          return (
             <input
                value={this.state.term}
                onChange={this.onInputChange.bind(this)}
                ref={this.setInputSearchRef} />
          );
       }
    }
    ```

    **클로저(closures)** 를 사용하여 함수형 컴포넌트에서 *refs*를 사용할 수도 있다.
    **참고**: 권장하진 않지만, 인라인 ref 콜백을 이용할 수도 있다.

21. ### forward refs는 무엇인가?

    *Ref 전달(Ref forwarding)* 특정 컴포넌트에서 *ref*를 받아 자식에게 전달하는 기능이다.

    ```jsx harmony
    const ButtonElement = React.forwardRef((props, ref) => (
      <button ref={ref} className="CustomButton">
        {props.children}
      </button>
    ));

    // Create ref to the DOM button:
    const ref = React.createRef();
    <ButtonElement ref={ref}>{'Forward Ref'}</ButtonElement>
    ```

22. ### callback refs 및 findDOMNode()에서 선호되는 옵션은?

    `findDOMNode()` API 위에 *callback refs*를 사용하는 것이 좋다. `findDOMNode()`이 추후 React에서의 개선 사항을 방해하기 때문이다.

    `findDOMNode`를 사용하는 **legacy** 접근법은 다음과 같다.

    ```javascript
    class MyComponent extends Component {
      componentDidMount() {
        findDOMNode(this).scrollIntoView()
      }

      render() {
        return <div />
      }
    }
    ```

    권장되는 접근법은 다음과 같다.

    ```javascript
    class MyComponent extends Component {
      constructor(props){
        super(props);
        this.node = createRef();
      }
      componentDidMount() {
        this.node.current.scrollIntoView();
      }

      render() {
        return <div ref={this.node} />
      }
    }
    ```

23. ### String Refs가 왜 legacy인가?

    React를 사용해보기 전이라면, 예전 API에서 `ref={'textInput'}`과 같은 `ref` 속성이 문자열인 것과 DOM node가 `this.refs.textInput`과 같이 액세스 되는 것에 익숙할 것이다. *String Refs에 문제가 있어*, legacy로 간주하기 때문에 사용하지 않기를 바란다. String Refs는 **React v16에 제거되었다**.

    1. *React가 현재 실행 중인 컴포넌트를 추적하도록 강제된다*. 이는 react 모듈을 stateful 하게 만들고, react 모듈이 번들에 복제될 때 이상한 오류를 유발하기 때문에 문제가 된다.
    2. *composable* 하지 않다. — 라이브러리가 전달된 자식에 ref를 넣으면, 사용자는 다른 ref를 추가할 수 없다. Callback ref는 완벽하게 구성이 가능하다.
    3. Flow와 같은 *정적 분석에서는 작동하지 않는다*. Flow는 프레임워크가 String Refs를 `this.refs`에 표시하도록 하는 마법과 그것의 타입(다를 수 있음)을 추측할 수 없다. Callback ref는 정적 분석에 친숙합니다..
    4. 대부분의 사람이 생각하는 "render callback" 패턴으로 작동하지 않는다. (예). `<DataGrid renderRow={this.renderRow} />`)
       ```jsx harmony
       class MyComponent extends Component {
         renderRow = (index) => {
           // This won't work. Ref will get attached to DataTable rather than MyComponent:
           return <input ref={'input-' + index} />;

           // This would work though! Callback refs are awesome.
           return <input ref={input => this['input-' + index] = input} />;
         }

         render() {
           return <DataTable data={this.props.data} renderRow={this.renderRow} />
         }
       }
       ```
24. ### Virtual DOM이란?

    *Virtual DOM* (VDOM)는 *실제 DOM*의 인-메모리 표현이다. UI 표현은 메모리에 유지되고 "실제" DOM과 동기화된다. 이는 렌더 함수의 호출과 화면상 elements를 표현하는 사이에 발생하는 단계이다. 이 전체 프로세스는 *조정* 이라고 한다.

25. ### Virtual DOM은 어떻게 작동하나?

    *Virtual DOM*는 세 가지 간단한 단계로 작동한다.

    1. 기본 데이터가 변경될 때마다, 전체 UI는 Virtual DOM 표현으로 리렌더링 된다.
        ![vdom](images/vdom1.png)

    2. 이전 DOM 표현과 새로운 표현 사이의 차이를 계산한다.
        ![vdom2](images/vdom2.png)

    3. 계산이 완료되면, 실제 DOM은 실제로 변경된 것만 업데이트할 것이다.
        ![vdom3](images/vdom3.png)

26. ### Shadow DOM과 Virtual DOM의 차이점

    *Shadow DOM* 주로 *웹 컴포넌트*에서 변수와 CSS의 범위 지정을 위해 디자인된 브라우저 기술이다. *Virtual DOM*는 브라우저 API를 기반으로 Javascript 라이브러리로 구현된 개념이다.

27. ### React Fiber란?

    Fiber는 React v16에서 새로운 *조정된* 엔진 또는 핵심 알고리즘의 재구현이다. React Fiber의 목표는 애니메이션, 레이아웃, 제스처, 작업 일시중지, 중단, 재사용 같은 영역에 대한 적합성을 높이고 다양한 유형의 업데이트에 우선순위를 정하는 것이다. 

28. ### React Fiber의 주요 목표는??

    *React Fiber*의 목표는 애니메이션, 레이아웃, 제스처, 작업 일시중지, 중단, 재사용 같은 영역에 대한 적합성을 높이는 것이다. 주요 기능은 **incremental rendering**으로 렌더링 작업을 청크(chunk)로 분할하고 여러 프레임에 걸쳐 펼치는 기능이다.

29. ### controlled components란?

    사용자가 입력한 뒤 폼의 입력창을 제어하는 component를 **Controlled Component**라고 한다. 즉 모든 상태 변이에는 관련된 핸들러 함수가 있다.

    예를 들어, 모든 이름을 대문자로 작성하기 위해서, 아래와 같은 handleChange를 사용한다.

    ```javascript
    handleChange(event) {
      this.setState({value: event.target.value.toUpperCase()})
    }
    ```

30. ### uncontrolled components란?

    The **Uncontrolled Components**는 내부적으로 자신의 상태를 저장하는 것으로, 현재의 값을 찾기 위해 필요하다면 ref를 사용하여 DOM에서 찾아온다. 이것은 전통적인 HTML과 더 비슷하다.

    아래의 UserProfile component에서, `이름` 입력은 ref를 사용해서 액세스한다.

    ```jsx harmony
    class UserProfile extends React.Component {
      constructor(props) {
        super(props)
        this.handleSubmit = this.handleSubmit.bind(this)
        this.input = React.createRef()
      }

      handleSubmit(event) {
        alert('A name was submitted: ' + this.input.current.value)
        event.preventDefault()
      }

      render() {
        return (
          <form onSubmit={this.handleSubmit}>
            <label>
              {'Name:'}
              <input type="text" ref={this.input} />
            </label>
            <input type="submit" value="Submit" />
          </form>
        );
      }
    }
    ```

    대부분의 경우 양식을 구현하는 데 controlled components를 사용하는 것을 추천한다.

31. ### createElement와 cloneElement의 차이점은?

    JSX elements는 `React.createElement()` 함수로 옮겨져서 UI의 객체 표현에 사용되는 React elements를 만든다. 반면에 `cloneElement`은 element를 복사하고 새로운 props로 전달하는 데 사용된다.

32. ### React에서 Lifting State Up란?

    여러 컴포넌트가 동일한 변경 데이터를 공유해야 하는 경우 가장 가까운 공통 조상으로 *lift the shared state up*을 하는 것을 추천한다. 즉 2개의 자식 컴포넌트가 부모로부터 동일한 데이터를 공유하는 경우, 모든 자식 컴포넌트에서 로컬 상태를 유지하는 대신에 상태를 부모에서 관리하는 것이다.

33. ### 컴포넌트 라이프 사이클의 다른 단계들은?

    컴포넌트 라이프 사이클는 세 가지의 고유한 단계가 있다.

    1. **Mounting:** 컴포넌트가 브라우저 DOM에 mount 할 준비가 되었다. 이 단계는 `constructor()`, `getDerivedStateFromProps()`, `render()`, `componentDidMount()` 라이프 사이클 메서드의 초기화에 대해 다룬다.

    2. **Updating:** 이 단계에서는, 컴포넌트는 두 가지 방법으로 업데이트가 되는데, 새로운 props를 보내거나, `setState()` 또는 `forceUpdate()`으로 state를 업데이트하는 것이다. 이 단계에서는 `getDerivedStateFromProps()`, `shouldComponentUpdate()`, `render()`, `getSnapshotBeforeUpdate()`, `componentDidUpdate()` 라이프 사이클 메서드를 다룬다.

    3. **Unmounting:** 이 마지막 단계에서는, 컴포넌트는 필요하지 않으며 브라우저 DOM에서 unmount된다. 이 단계에서는 `componentWillUnmount()` 라이프 사이클 메서드가 포함된다.

    React는 DOM에 변경 사항을 적용할 때 내부적으로 단계의 개념을 가지고 있다는 것을 언급할 필요가 있다. 다음과 같이 분리된다.

    1. **Render** 컴포넌트는 부수 효과 없이 렌더링 된다. Pure 컴포넌트에 적용되며 이 단계에서 React는 렌더링을 일시 정지, 중단 또는 재시작할 수 있다.

    2. **Pre-commit** 컴포넌트가 실제로 DOM에 변경사항을 적용하기 전에, React가 `getSnapshotBeforeUpdate()`를 통해서 DOM을 읽을 수 있는 순간이다.

    3. **Commit** React는 DOM과 함께 작동하고 Mount를 위한 `componentDidMount()`, 업데이트를 위한 `componentDidMount()`, Unmount를 위한 `componentWillUnmount()`의 최종 라이프 사이클을 각각 실행한다.

    React 16.3+ 단계 (또는) [일반적인 버전](http://projects.wojtekmaj.pl/react-lifecycle-methods-diagram/))

    ![phases 16.3+](images/phases16.3.jpg)

    React 16.3 전에는

    ![phases 16.2](images/phases.png)


34. ### React의 라이프 사이클 메서드에는 무엇이 있나?

    React 16.3+

    - **getDerivedStateFromProps:** `render()`가 호출되기 바로 전에 호출되며 *모든* 렌더링에서 호출된다. 이전 state가 필요한 드문 경우에 사용이 된다. [이전 state가 필요하면](https://reactjs.org/blog/2018/06/07/you-probably-dont-need-derived-state.html) 읽을만한 가치가 있다.
    - **componentDidMount:** 첫 번째 렌더링 이후에 실행되고, 여기서 모든 AJAX 요청, DOM 또는 state 업데이트 및 이벤트 리스너가 설정된다.
    - **shouldComponentUpdate:** 컴포넌트를 업데이트 해야 할지 여부를 결정한다. 기본적으로 `true`를 반환한다. state나 props가 업데이트된 후에 컴포넌트를 렌더링할 필요 없다고 확신하는 경우 false를 반환할 수 있다. 컴포넌트가 새로운 props를 받으면 리렌더링하는 것을 방지할 수 있어 성능을 향상하는데 매우 좋다.
    - **getSnapshotBeforeUpdate:** 렌더링 된 출력이 DOM에 커밋되기 바로 직전에 실행된다. 이로 인해 모든 값은 `componentDidUpdate()`에 전달이 된다. DOM에서 스크롤 위치 같은 정보를 가져오는 데 유용하다.
    - **componentDidUpdate:** 주로 props나 state의 변경에 대한 응답으로 DOM을 업데이트하는데 사용된다. `shouldComponentUpdate()`가 `false`를 반환하면 실행되지 않는다.
    - **componentWillUnmount** 나가는 네트워크 요청을 취소하거나 컴포넌트와 관련된 모든 이벤트 리스너를 제거하는 데 사용된다.

    Before 16.3

    - **componentWillMount:** 렌더링 전에 실행되며 root 컴포넌트의 App 수준 구성을 하는 데 사용된다.
    - **componentDidMount:** 첫 번째 렌더링 이후에 실행되고, 여기서 모든 AJAX 요청, DOM 또는 state 업데이트 및 이벤트 리스너가 설정된다.
    - **componentWillReceiveProps:** 특정 props 업데이트가 state 전환을 일으킬 때 실행된다.
    - **shouldComponentUpdate:** 컴포넌트를 업데이트 해야 할지 여부를 결정한다. 기본적으로 `true`를 반환한다. state나 props가 업데이트된 후에 컴포넌트를 렌더링할 필요 없다고 확신하는 경우 false를 반환할 수 있다. 컴포넌트가 새로운 props를 받으면 리렌더링하는 것을 방지할 수 있어 성능을 향상하는데 매우 좋다.
    - **componentWillUpdate:** true를 반환하는 `shouldComponentUpdate()`에 의해 확인된 props 및 state 변경이 있을 때 컴포넌트를 리렌더링하기 전에 실행된다.
    - **componentDidUpdate:** 주로 props나 state 변경에 대한 응답으로 DOM을 업데이트하는 데 사용된다.
    - **componentWillUnmount:** 나가는 네트워크 요청을 취소하거나 컴포넌트와 관련된 모든 이벤트 리스너를 제거하는 데 사용된다.

35. ### 고차(Higher-Order) 컴포넌트란?

    *고차(Higher-Order) 컴포넌트* (*HOC*)는 컴포넌트를 가져와서 새로운 컴포넌트를 반환하는 함수이다. 기본적으로, 컴포넌트 구성상의 본질에서 파생된 패턴이다.

    동적으로 제공된 자식 컴포넌트는 허용할 수 있지만, 입력 컴포넌트의 어떠한 동작을 수정하거나 복사하지 않으므로 **순수 컴포넌트(pure components)** 라고 부른다. 

    ```javascript
    const EnhancedComponent = higherOrderComponent(WrappedComponent)
    ```

    HOC는 아래와 같은 많은 사례에서 사용할 수 있다.

    1. 코드 재사용, 논리 및 부트스트랩 추상화
    2. 도용 렌더링
    3. State 추상화 및 조작
    4. Props 조작.

36. ### HOC 컴포넌트를 사용해서 props 프록시를 만드는 방법은?

    다음과 같이 *props proxy* 패턴을 사용하여 컴포넌트에 전달된 props를 추가/편집할 수 있다.

    ```jsx harmony
    function HOC(WrappedComponent) {
      return class Test extends Component {
        render() {
          const newProps = {
            title: 'New Header',
            footer: false,
            showFeatureX: false,
            showFeatureY: true
          }

          return <WrappedComponent {...this.props} {...newProps} />
        }
      }
    }
    ```

37. ### context란?

    *Context*는 수동으로 모든 단계에 props를 전달하지 않고 컴포넌트 트리를 통해 데이터를 전달하는 방법을 제공한다. 예를 들어, 인증된 사용자, locale 기본 설정, UI 테마는 많은 컴포넌트를 통해 응용 프로그램에서 액세스해야 한다.

    ```javascript
    const {Provider, Consumer} = React.createContext(defaultValue)
    ```

38. ### children prop이란?

    *Children*(`this.prop.children`)는 다른 prop와 마찬가지로 다른 컴포넌트에 데이터를 전달할 수 있는 요소(`this.prop.children`)다. 컴포넌트의 여는 태그와 닫는 태그 사이에 놓인 컴포넌트 트리가 해당 컴포넌트의 `children` prop로 전달된다.

    이 prop을 사용하기 위해 React API에서 사용할 수 있는 여러 가지 방법이 있다. 여기에는`React.Children.map`,`React.Children.forEach`,`React.Children.count`,`React.Children.only`,`React.Children.toArray`가 포함된다.
    children prop의 간단한 사용법은 다음과 같다.

    ```jsx harmony
    const MyDiv = React.createClass({
      render: function() {
        return <div>{this.props.children}</div>
      }
    })

    ReactDOM.render(
      <MyDiv>
        <span>{'Hello'}</span>
        <span>{'World'}</span>
      </MyDiv>,
      node
    )
    ```

39. ### React에서 주석을 어떻게 다는가?

    React / JSX의 주석은 JavaScript Multiline 주석과 유사하지만 중괄호로 묶인다.

    **Single-line comments:**

    ```jsx harmony
    <div>
      {/* 한 줄 주석 (바닐라 자바 스크립트에서는 한 줄 주석은 이중 슬래시 (//)로 표시된다) */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```

    **Multi-line comments:**

    ```jsx harmony
    <div>
      {/* 한 줄이상의
        여러 줄 주석 */}
      {`Welcome ${user}, let's play React`}
    </div>
    ```

40. ### props argument가 있는 생성자에서 super를 사용하는 목적은 무엇입니까?

    자식 클래스 생성자는`super()`메서드가 호출 될 때까지 `this`를 참조할 수 없습니다. ES6 하위 클래스에도 동일하게 적용된다. super() 호출에 props 매개 변수를 전달하는 주요한 이유는 자식 생성자에서 `this.props`에 접근하기 위해서다.

    **props 전달**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    **props 미전달**

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()

        console.log(this.props) // prints undefined

        // but props parameter is still available
        console.log(props) // prints { name: 'John', age: 42 }
      }

      render() {
        // no difference outside constructor
        console.log(this.props) // prints { name: 'John', age: 42 }
      }
    }
    ```

    위 코드를 보면 `this.props`가 생성자 내에서만 다른 것을 볼 수 있다. 생성자 밖에서는 동일하다.

41. ### 조정(reconciliation)이란?

    컴포넌트의 props나 state가 변경되었을 때, React는 새로 반환된 엘리먼트와 이전에 렌더링된 것을 비교해서 실제 DOM이 업데이트가 필요한지를 결정한다. 동등하지 않을 때, React가 DOM을 업데이트할 것이다. 이 프로세스를 *조정(reconciliation)*이라고 한다.

42. ### state의 키 이름을 동적으로 설정하는 방법은?

    ES6나 Babel transpiler를 사용하여 JSX코드를 변환하는 경우 *원하는 속성(property)명*으로 설정할 수 있다.

    ```javascript
    handleInputChange(event) {
      this.setState({ [event.target.id]: event.target.value })
    }
    ```

43. ### 컴포넌트가 렌더링 될 때마다 호출되는 함수에 대한 실수는 무엇일까?

    함수를 매개변수로 전달하는 동안 함수가 호출되지 않도록 확인해야 한다.

    ```jsx harmony
    render() {
      // Wrong: handleClick is called instead of passed as a reference!
      return <button onClick={this.handleClick()}>{'Click Me'}</button>
    }
    ```

    대신에, 괄호 없이 함수 자체를 전달해야 한다.

    ```jsx harmony
    render() {
      // Correct: handleClick is passed as a reference!
      return <button onClick={this.handleClick}>{'Click Me'}</button>
    }
    ```

44. ### 왜 컴포넌트 이름은 대문자로 해야 하나?

    컴포넌트는 DOM 엘리먼트가 아니기 때문에 대문자로 표기해야 한다. 또한, JSX 소문자 태그 이름은 HTML 엘리먼트를 나타내며 컴포넌트는 참조하지 않는다.

45. ### React는 왜 `class`가 아닌 `className` 속성을 사용하나?

    `class`는 JavasScript의 키워드이며, JSX는 JavaScript의 확장이다. 이것이 React가 `class` 대신 `className`을 사용하는 주된 이유이다. `className` prop으로 문자열을 넘겨야 한다.

    ```jsx harmony
    render() {
      return <span className={'menu navigation-menu'}>{'Menu'}</span>
    }
    ```

46. ### fragments란?

    컴포넌트가 여러 엘리먼트를 반환하는 데 사용하는 React의 일반적인 패턴이다. *Fragments*를 사용하면 DOM에 노드를 추가하지 않고 자식 목록을 그룹화할 수 있다.

    ```jsx harmony
    render() {
      return (
        <React.Fragment>
          <ChildA />
          <ChildB />
          <ChildC />
        </React.Fragment>
      )
    }
    ```

    *더욱더 짧은 구문*도 있지만, 많은 도구에서 지원하지 않는다.

    ```jsx harmony
    render() {
      return (
        <>
          <ChildA />
          <ChildB />
          <ChildC />
        </>
      )
    }
    ```

47. ### div보다 fragments가 더 우수한 이유는?

    1. Fragments는 조금 더 빠르며 여분의 DOM 노드를 만들지 않아서 메모리를 덜 사용한다. 이것은 매우 크고 깊은 트리(tree)에서 실질적인 이득을 가져다준다.
    2. *Flexbox*와 *CSS Grid* 같은 일부 CSS 메커니즘에는 특수한 부모-자식 관계를 가지고 있어서, 중간에 div를 추가하면 원하는 레이아웃을 유지하기가 어렵다.
    3. DOM Inspector가 덜 복잡해진다.

48. ### React의 portals이란?

    *Portal*은 상위 컴포넌트의 DOM 계층 구조 외부에 있는 DOM 노드에 자식을 렌더링하는데 권장되는 방법이다.

    ```javascript
    ReactDOM.createPortal(child, container)
    ```

    첫 번째 인수는 렌더링 가능한 React 엘리먼트, 문자열, fragment 같은 하위요소이다. 두 번째 인수는 DOM 엘리먼트이다.

49. ### stateless 컴포넌트란?

    동작이 state와 관련이 없는 경우 stateless 컴포넌트가 될 수 있다. function이나 class를 사용해서 stateless 컴포넌트를 만들 수 있다. 컴포넌트에서 라이프 사이클 훅을 사용해야 하는 경우가 아니라면 function 컴포넌트를 사용하는게 좋다. function 컴포넌트를 사용하면 여러 이점이 있는데, 쓰기, 이해 및 테스트하기가 쉽고 더 빠르며, `this` 키워드를 피할 수 있다.

50. ### stateful 컴포넌트란?

    컴포넌트의 동작이 컴포넌트의 *state*에 따라 달라진다면 stateful 컴포넌트라고 할 수 있다. *stateful 컴포넌트*는 항상 *class 컴포넌트* 이며 `constructor`에서 초기화가 되어 state를 가지게 된다.

    ```javascript
    class App extends Component {
      constructor(props) {
        super(props)
        this.state = { count: 0 }
      }

      render() {
        // ...
      }
    }
    ```

51. ### React에서 props 유효성 검사를 적용하는 방법은?

    응용 프로그램이 *development 모드*에서 실행될 때, React는 자동으로 컴포넌트에 설정한 모든 props를 확인하여 *올바른 타입*인지 확인한다. 타입이 맞지 않는다면, React는 콘솔에 경고 메시지를 띄운다. *production 모드*에서는 성능에 영향을 미치므로 사용할 수 없다. 주요한 props는 `isRequired`로 정의된다.

    사전 정의된 props 타입이다.

    1. `PropTypes.number`
    2. `PropTypes.string`
    3. `PropTypes.array`
    4. `PropTypes.object`
    5. `PropTypes.func`
    6. `PropTypes.node`
    7. `PropTypes.element`
    8. `PropTypes.bool`
    9. `PropTypes.symbol`
    10. `PropTypes.any`

    다음과 같이 `User` 컴포넌트에 대한 `propTypes`을 정의할 수 있다.

    ```jsx harmony
    import React from 'react'
    import PropTypes from 'prop-types'

    class User extends React.Component {
      static propTypes = {
        name: PropTypes.string.isRequired,
        age: PropTypes.number.isRequired
      }

      render() {
        return (
          <>
            <h1>{`Welcome, ${this.props.name}`}</h1>
            <h2>{`Age, ${this.props.age}`}</h2>
          </>
        )
      }
    }
    ```

    **Note:** React v15.5버전에서 *PropTypes*는 `React.PropTypes`에서 `prop-types` 라이브러리로 이동되었다.

52. ### React의 장점은?

    1. *Virtual DOM*으로 애플리케이션의 성능이 향상된다.
    2. JSX는 코드를 읽고 쓰기 쉽게 해준다.
    3. 클라이언트와 서버사이드(*SSR*) 렌더링이 둘 다 가능하다.
    4. 오직 view 라이브러리이기 때문에, 프레임워크(Angular, Backbone)에 쉽게 통합이 가능하다.
    5. Jest와 같은 툴을 사용하여 단위 및 통합 테스트를 쉽게 작성할 수 있다.

53. ### React의 한계는?

    1. React는 프레임워크가 아닌, view 라이브러리이다.
    2. 웹 개발을 처음 접하는 초보자에게 러닝 커브가 존재한다.
    3. 기존 MVC 프레임워크에 React를 통합하려면 몇 가지 추가 구성이 필요하다.
    4. 인라인 템플릿과 JSX로 인해 코드 복잡성이 증가한다.
    5. 너무 많은 작은 컴포넌트는 엔지니어링 또는 보일러 플레이트로 이어진다.

54. ### React v16에서 error boundaries란 무엇인가?

    *Error boundaries*는 하위 컴포넌트의 모든 위치에서 JavaScript 오류를 catch하고, 오류를 기록하며, 오류가 발생한 컴포넌트 트리 대신 폴백(fallback) UI를 표시하는 컴포넌트이다.

    클래스 컴포넌트는 `componentDidCatch(error, info)` 또는 `static getDerivedStateFromError()`라는 새로운 라이프 사이클 메서드를 정의하면 error boundary가 된다.

    ```jsx harmony
    class ErrorBoundary extends React.Component {
      constructor(props) {
        super(props)
        this.state = { hasError: false }
      }

      componentDidCatch(error, info) {
        // You can also log the error to an error reporting service
        logErrorToMyService(error, info)
      }

      static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

      render() {
        if (this.state.hasError) {
          // You can render any custom fallback UI
          return <h1>{'Something went wrong.'}</h1>
        }
        return this.props.children
      }
    }
    ```

    그런 다음 일반 컴포넌트를 사용하면 된다.

    ```jsx harmony
    <ErrorBoundary>
      <MyWidget />
    </ErrorBoundary>
    ```

55. ### React v15에서는 어떻게 error boundaries 조작하나?

    React v15에서는 `unstable_handleError` 메서드를 사용하여 *error boundaries* 에 대한 매우 기본적인 지원을 제공한다. React v16에서 `componentDidCatch`로 이름이 변경되었다.

56. ### 정적 타입 검사에 권장되는 방법은?

    일반적으로 우리는 React 애플리케이션에서 *타입 검사*를 위해 *PropTypes 라이브러리*를 사용한다. (React v15.5 이후 `React.PropTypes`는 `prop-types` 패키지로 옮겨짐.) 큰 코드 기반의 경우, 컴파일 타임에 타입검사를 하고 자동 완성 기능을 제공하는 Flow나 TypeScript 같은 *정적 타입 검사기*를 사용하는 것이 좋다.

57. ### `react-dom` 패키지 사용법은?

    `react-dom` 패키지는 앱의 최상위 레벨에서 사용할 수 있는 *DOM-관련 메서드*를 제공한다. 대부분의 컴포넌트는 이 모듈을 사용할 필요가 없다. 이 패키지의 일부 메서드는 아래와 같다.

    1. `render()`
    2. `hydrate()`
    3. `unmountComponentAtNode()`
    4. `findDOMNode()`
    5. `createPortal()`

58. ### `react-dom`의 render 메서드란?

    이 메서드는 React 엘리먼트를 제공된 컨테이너의 DOM에 렌더링하고 컴포넌트에 대한 참조를 반환하는 데 사용된다. React 엘리먼트가 이전에 컨테이너로 렌더링 된 경우, 해당 엘리먼트에 대한 업데이트를 수행하고 필요에 따라 최신 변경 사항을 반영하기 위해 DOM을 변경한다.

    ```
    ReactDOM.render(element, container[, callback])
    ```

    선택적 콜백이 제공되면, 컴포넌트가 렌더링 되거나 업데이트 됐을 때 실행된다.

59. ### ReactDOMServer란?

    `ReactDOMServer` 객체를 사용하면 컴포넌트를 정적 마크업(일반적으로 노드 서버에서 사용한다.)으로 렌더링할 수 있다. 이 객체는 주로 *서버 사이드 렌더링*(SSR) 에 사용된다. 아래의 메서드들은 서버와 브라우저 환경에서 모두 사용할 수 있다.

    1. `renderToString()`
    2. `renderToStaticMarkup()`

    예를 들어, 일반적으로 Express, Hapi, 또는 Koa와 같은 노드 기반 웹 서버를 실행하고 `renderToString`를 호출하여 루트 컴포넌트를 문자열로 렌더링한 다음 응답으로 보낸다. 

    ```javascript
    // using Express
    import { renderToString } from 'react-dom/server'
    import MyPage from './MyPage'

    app.get('/', (req, res) => {
      res.write('<!DOCTYPE html><html><head><title>My Page</title></head><body>')
      res.write('<div id="content">')
      res.write(renderToString(<MyPage/>))
      res.write('</div></body></html>')
      res.end()
    })
    ```

60. ### React에서 innerHTML를 사용하는 방법?

    `dangerouslySetInnerHTML`는 브라우저 DOM에서 `innerHTML`를 사용하기 위한 React의 대체 속성이다. `innerHTML`과 같이, 크로스-사이트 스크립팅(XSS) 공격을 고려하여 이 속성을 사용하는 것은 위험하다. `__html` 객체를 키로 전달하고 HTML 텍스트를 값으로 전달하면 된다.

    이 예제에서 MyComponent는 HTML 마크업 설정을 위해 `dangerouslySetInnerHTML` 속성을 사용한다.

    ```jsx harmony
    function createMarkup() {
      return { __html: 'First &middot; Second' }
    }

    function MyComponent() {
      return <div dangerouslySetInnerHTML={createMarkup()} />
    }
    ```

61. ### React에서 스타일을 사용하는 방법?

    `style` 속성은 CSS 문자열 대신에 camelCased 속성이 있는 JavaScript 객체를 사용한다. 이것은 DOM 스타일 JavaScript 속성과 일치하며, 보다 효율적이고, XSS 보안 취약점을 방지한다.

    ```jsx harmony
    const divStyle = {
      color: 'blue',
      backgroundImage: 'url(' + imgUrl + ')'
    };

    function HelloWorldComponent() {
      return <div style={divStyle}>Hello World!</div>
    }
    ```

    스타일 키는 JavaScript에서 DOM 노드의 속성(e.g. `node.style.backgroundImage`)에 액세스하는 것과 일관성을 유지하기 위해서 camelCased로 작성한다.

62. ### React에서 이벤트가 어떻게 다른가?

    React 엘리먼트의 이벤트 처리에는 다음과 같은 문법적 차이가 있다.

    1. React 이벤트 핸들러는 소문자가 아닌 camelCase를 사용하여 명명된다.
    2. JSX에서는 문자열이 아닌 이벤트 핸들러로 함수를 전달한다.

63. ### 생성자에서 `setState()`를 사용하면 어떻게 되나?

    `setState()`를 사용하면, React에 객체 state를 할당하는 것과 별개로 컴포넌트와 모든 자식을 리렌더링한다. 다음과 같은 오류가 발생한다. *Can only update a mounted or mounting component.* 그래서 `this.state`를 사용하여 생성자 내부의 변수를 초기화해야 한다.

64. ### 키로 인덱스를 사용하면?

    React가 엘리먼트를 추적할 수 있도록 키는 안정적이고 예측 가능하며 고유해야 한다.

    아래의 코드 조각에서 각 엘리먼트의 키는 표현되는 데이터에 묶이지 않고 순서를 기반으로 한다. 이것은 React가 할 수 있는 최적화를 제한한다.

    ```jsx harmony
    {todos.map((todo, index) =>
      <Todo
        {...todo}
        key={index}
      />
    )}
    ```

    유니크한 키에 엘리먼트 데이터를 사용하는 경우, todo.id가 이 목록에서 유일하고 안정적이라고 가정하면, React는 요소를 재평가 할 필요없이 엘리먼트를 재정렬 할 수 있다.

    ```jsx harmony
    {todos.map((todo) =>
      <Todo {...todo}
        key={todo.id} />
    )}
    ```

65. ### `componentWillMount()` 메서드에서 `setState()`를 사용하는 것은 좋은가?

    `componentWillMount()` 라이프 사이클 메서드에서 비동기 초기화를 하지 않는게 좋다. `componentWillMount()`는 마운트가 발생하기 직전에 호출된다. `render()` 전에 호출되기 때문에 메서드에서 state를 설정하면 리렌더링 되지 않는다. 다음과 같은 메서드로 사이드 이펙트나 구독을 피하면된다. `componentWillMount()` 대신에 `componentDidMount()`에서 컴포넌트 초기화에 대한 비동기 호출을 한다.
 
    ```jsx harmony
    componentDidMount() {
      axios.get(`api/todos`)
        .then((result) => {
          this.setState({
            messages: [...result.data]
          })
        })
    }
    ```

66. ### 초기 state에 props를 사용하면 어떻게 되나?

    컴포넌트를 새로 고침 없이 컴포넌트의 props를 변경하면, 생성자 함수가 절대로 컴포넌트의 현재 state를 업데이트하지 않으므로 새로운 props 값이 표시되지 않는다. props로 state 초기화하는 것은 컴포넌트가 처음 만들어질 때만 실행된다. 

    아래의 컴포넌트는 업데이트된 입력값을 표시하지 않는다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          records: [],
          inputValue: this.props.inputValue
        };
      }

      render() {
        return <div>{this.state.inputValue}</div>
      }
    }
    ```

    render 메서드 안에서 props를 사용하면 값이 업데이트된다.

    ```jsx harmony
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)

        this.state = {
          record: []
        }
      }

      render() {
        return <div>{this.props.inputValue}</div>
      }
    }
    ```

67. ### 컴포넌트를 조건부로 렌더링하는 방법?

    경우에 따라 일부 state에 따라 다른 컴포넌트를 렌더링하려고 한다. JSX는 `false` 또는 `undefined`를 렌더링하지 않아 조건부 *단락*을 사용하여 특정 조건이 true인 경우에만 컴포넌트의 주어진 부분을 렌더링할 수 있다.

    ```jsx harmony
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address &&
          <p>{address}</p>
        }
      </div>
    )
    ```

    `if-else` 조건이 필요하면 *삼항 연산자*를 사용하면 된다.

    ```jsx harmony
    const MyComponent = ({ name, address }) => (
      <div>
        <h2>{name}</h2>
        {address
          ? <p>{address}</p>
          : <p>{'Address is not available'}</p>
        }
      </div>
    )
    ```

68. ### DOM 엘리먼트에서 spread props를 조심해야하는 이유는?

    *spread props* 를 사용할 때 알 수 없는 HTML 속성을 추가할 위험이 있다. 이는 나쁜 습관이다. 대신 우리는 `...rest` 연산자로 props destructuring을 사용할 수 있으므로, 필요한 props만 추가할 수 있다. 예를 들어,

    ```jsx harmony
    const ComponentA = () =>
      <ComponentB isDisplay={true} className={'componentStyle'} />

    const ComponentB = ({ isDisplay, ...domProps }) =>
      <div {...domProps}>{'ComponentB'}</div>
    ```

69. ### React에서 데코레이터를 사용하는 방법?

    컴포넌트를 함수로 전달하는 것과 동일하게, *class* 컴포넌트를 *꾸밀 수* 있다. **데코레이터**는 컴포넌트 기능을 수정하는 유연하고 읽기 쉬운 방법이다.

    ```jsx harmony
    @setTitle('Profile')
    class Profile extends React.Component {
        //....
    }

    /*
      title은 문서 제목으로 설정될 문자열이다.
      WrappedComponent는 우리의 데코레이터가 위의 예제에서 볼 수 있듯이 컴포넌트 클래스 바로 위에 놓는다.
    */
    const setTitle = (title) => (WrappedComponent) => {
      return class extends React.Component {
        componentDidMount() {
          document.title = title
        }

        render() {
          return <WrappedComponent {...this.props} />
        }
      }
    }
    ```

    **Note:** 데코레이터는 ES7에 포함되지 않았지만, 현재 *stage 2 proposal*이다.

70. ### 컴포넌트를 어떻게 메모하나?

    함수형 컴포넌트에 사용할 수 있는 메모 라이브러리가 있다. 예를 들어 `moize` 라이브러리는 다른 컴포넌트에 컴포넌트를 메모할 수 있다.

    ```jsx harmony
    import moize from 'moize'
    import Component from './components/Component' // this module exports a non-memoized component

    const MemoizedFoo = moize.react(Component)

    const Consumer = () => {
      <div>
        {'I will memoize the following entry:'}
        <MemoizedFoo/>
      </div>
    }
    ```

71. ### Server Side Rendering 또는 SSR 구현방법?

    React는 이미 노드 서버에서 렌더링을 처리할 수 있도록 준비되어 있다. DOM 렌더러의 특수 버전을 사용할 수 있으며 클라이언트 측과 동일한 패턴을 따른다.

    ```jsx harmony
    import ReactDOMServer from 'react-dom/server'
    import App from './App'

    ReactDOMServer.renderToString(<App />)
    ```

    이 메서드는 일반 HTML을 문자열로 출력하며, 서버 응답의 일부로 페이지 본문 내에 배치할 수 있다. 클라이언트 측에서 React는 사전 렌더링된 컨텐츠를 탐지하고 중단된 부분을 완벽하게 파악한다.

72. ### React에서 production 모드를 사용하는 방법?

    Webpack의 `DefinePlugin` 메서드를 사용해서 `NODE_ENV`를 `production` 환경으로 설정해야 propType 유효성 검사 및 추가 경고와 같은 사항을 제거할 수 있다. 이와는 별개로, Uglify의 개발 코드와 주석을 제거하는 데드 코드(dead-code) 제거 기능을 사용하여 번들 크기를 크게 줄일 수 있다.

73. ### CRA란 무엇이며 장점은?

    `create-react-app` CLI 툴은 별도의 구성단계 없이 빠르게 React 애플리케이션을 만들고 실행할 수 있다.

    *CRA*로 Todo 앱을 만들어보자

    ```console
    # Installation
    $ npm install -g create-react-app

    # Create new project
    $ create-react-app todo-app
    $ cd todo-app

    # Build, test and run
    $ npm run build
    $ npm run test
    $ npm start
    ```
    React 앱을 제작하는 데 필요한 모든 것이 포함되어 있다.

    1. React, JSX, ES6, 및 Flow 문법 지원.
    2. object spread operator와 같은 ES6를 넘어선 언어 확장 기능.
    3. 자동 접두어가 붙은 CSS로, -webkit- 이나 다른 접두사는 필요 없다.
    4. coverage를 지원하는 내장된 빠른 대화형 단위 테스트 러너.
    5. 일반적인 실수에 대해서 경고하는 라이브 개발 서버.
    6. hashes와 sourcemaps을 사용하여 production 용 JS, CSS 및 images를 묶는 빌드 스크립트

74. ### 마운팅의 라이프 사이클 메서드 순서는?

    라이프 사이클 메서드는 컴포넌트 인스턴스가 생성되어 DOM에 삽입될 때 다음과 같은 순서로 호출된다.

    1. `constructor()`
    2. `static getDerivedStateFromProps()`
    3. `render()`
    4. `componentDidMount()`

75. ### React v16에서 더 이상 사용되지 않는 라이프 사이클 메서드는?

    다음 라이프 사이클 메소드는 안전하지 않은 코딩 방법이며 비동기 렌더링에서는 더욱 문제 될 것이다.

    1. `componentWillMount()`
    2. `componentWillReceiveProps()`
    3. `componentWillUpdate()`

    React v16.3에서 위의 메서드들은 `UNSAFE_` 접두어가 별칭으로 붙어주기 시작했으며, React v17에서 접두어가 없는 버전은 제거된다.

76. ### getDerivedStateFromProps() 라이프 사이클 메서드의 사용 목적은?

    새로운 정적 `getDerivedStateFromProps()` 라이프 사이클 메서드는 컴포넌트가 인스턴스화된 후뿐만 아니라 리렌더링 되기 전에 호출된다. update state를 object로 돌려줄 수도 있고, 새로운 props가 state 업데이트를 하지 않아도 되는 것을 나타내기 위해 `null`을 리턴할 수 있다.

    ```javascript
    class MyComponent extends React.Component {
      static getDerivedStateFromProps(props, state) {
        // ...
      }
    }
    ```

    이 라이프 사이클 메서드는 `componentDidUpdate()`와 `componentWillReceiveProps()`의 모든 사용 사례를 커버한다.

77. ### getSnapshotBeforeUpdate() 라이프 사이클 메서드의 사용 목적은??

    새로운 `getSnapshotBeforeUpdate()` 라이프 사이클 메서드는 DOM 업데이트 직전에 호출된다. 이 메서드의 반환 값은 세 번째 매개 변수로 `componentDidUpdate()`에 전달된다.

    ```javascript
    class MyComponent extends React.Component {
      getSnapshotBeforeUpdate(prevProps, prevState) {
        // ...
      }
    }
    ```

    이 라이프 사이클 메서드는 `componentDidUpdate()`와 `componentWillUpdate()`의 모든 사용 사례를 커버한다.

78. ### Hooks는 렌더링 props와 고차원 컴포넌트를 대체한다?

    렌더링 props와 고차원 컴포넌트 모두 하나의 자식만 렌더링하지만, 대부분의 경우 Hooks는 트리에서 중첩을 줄임으로써 제거하는 더 간단한 방법이다.

79. ### 컴포넌트를 명명하는데 권장되는 방법은?

    `displayName`을 사용하는 대신 참조로 컴포넌트의 이름을 지정하는 것이 좋다.

    컴포넌트 명명에 `displayName`를 사용하는 경우.

    ```javascript
    export default React.createClass({
      displayName: 'TodoApp',
      // ...
    })
    ```

    **권장되는** 접근 방법:

    ```javascript
    export default class TodoApp extends React.Component {
      // ...
    }
    ```

80. ### 컴포넌트 클래스에서 권장되는 메서드 순서는?

     *마운팅*에서 *렌더링 단계*까지 *권장되는* 메서드 순서는 아래와 같다. 

    1. `static` 메서드
    2. `constructor()`
    3. `getChildContext()`
    4. `componentWillMount()`
    5. `componentDidMount()`
    6. `componentWillReceiveProps()`
    7. `shouldComponentUpdate()`
    8. `componentWillUpdate()`
    9. `componentDidUpdate()`
    10. `componentWillUnmount()`
    11. `onClickSubmit()` 또는 `onChangeDescription()`과 같은 핸들러 또는 이벤트 핸들러를 클릭. 
    12. `getSelectReason()` 또는 `getFooterContent()`와 같은 렌더링을 위한 getter 메서드
    13. `renderNavigation()` 또는 `renderProfilePicture()`와 같은 선택적 렌더링 메서드
    14. `render()`

81. ### 스위칭 컴포넌트란?

    *스위칭 컴포넌트란*는 많은 컴포넌트 중 하나를 렌더링하는 컴포넌트이다. prop 값을 컴포넌트에 매핑하려면 object를 사용해야 한다.

    예를 들어, `page` prop을 기반으로 한 다른 페이지를 표시하는 스위칭 컴포넌트.

    ```jsx harmony
    import HomePage from './HomePage'
    import AboutPage from './AboutPage'
    import ServicesPage from './ServicesPage'
    import ContactPage from './ContactPage'

    const PAGES = {
      home: HomePage,
      about: AboutPage,
      services: ServicesPage,
      contact: ContactPage
    }

    const Page = (props) => {
      const Handler = PAGES[props.page] || ContactPage

      return <Handler {...props} />
    }

    // PAGES 객체의 키는 prop 타입에서 사용되어 dev-time errors를 잡아낼 수 있다.
    Page.propTypes = {
      page: PropTypes.oneOf(Object.keys(PAGES)).isRequired
    }
    ```

82. ### 왜 setState()에 함수를 전달해야 하나?

    `setState()`가 비동기 연산이기 때문이다. 성능상 이유로 React는 state를 일괄적으로 변경한다. 그래서 `setState()`가 호출되고 state가 즉시 변경되지 않는다. 즉 `setState()` 를 호출할 때 현재 상태에 의존해서는 안 되며 그 상태가 무엇인지 확신할 수 없게 된다. 해결방법은 이전 상태를 인수로 사용하기 위해 `setState()`에 함수를 전달하는 것이다. 이렇게 하면 `setState()`의 비동기 특성으로 인해 사용자가 액세스할 때 이전 상태 값을 가져오는 문제를 피할 수 있다.

    초기 count 값은 0이라고 가정해보자. 세 번의 연속 증가 연산을 하면, 값은 1만 증가한다.

    ```javascript
    // assuming this.state.count === 0
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    this.setState({ count: this.state.count + 1 })
    // this.state.count === 1, not 3
    ```

    `setState()`에 함수를 전달하면, count는 올바르게 증가한다.

    ```javascript
    this.setState((prevState, props) => ({
      count: prevState.count + props.increment
    }))
    // this.state.count === 3 as expected
    ```

83. ### React의 strict mode란?

    `React.StrictMode`는 애플리케이션의 잠재적인 문제점을 강조 표시하는데 유용한 컴포넌트이다. `<Fragment>`와 마찬가지로, `<StrictMode>`는 특정 DOM 엘리먼트에 렌더링하지 않는다. 자손에 대한 추가 점검과 경고를 활성화한다. 이러한 점검은 *개발 모드*에만 적용이 된다.

    ```jsx harmony
    import React from 'react'

    function ExampleApplication() {
      return (
        <div>
          <Header />
          <React.StrictMode>
            <div>
              <ComponentOne />
              <ComponentTwo />
            </div>
          </React.StrictMode>
          <Footer />
        </div>
      )
    }
    ```

    위의 예제에서, *strict mode* 검사는 `<ComponentOne>`와 `<ComponentTwo>` 컴포넌트에만 적용된다.

84. ### React Mixins이란?

    *Mixins*은 공통 기능을 갖도록 컴포넌트를 완전히 분리하는 방법이다. Mixins은 **사용하지 않아야 하며** *고차원 컴포넌트*나 *데코레이터*로 대체할 수 있다.

    가장 일반적으로 사용되는 mixins은 `PureRenderMixin`이다. props와 state가 이전 props, state와 얕게 동등할 때 불필요한 리렌더링을 방지하기 위해 일부 컴포넌트에서 사용할 수도 있다.

    ```javascript
    const PureRenderMixin = require('react-addons-pure-render-mixin')

    const Button = React.createClass({
      mixins: [PureRenderMixin],
      // ...
    })
    ````
    <!-- TODO: mixins은 더이상 사용되지 않는다. -->

85. ### 왜 isMounted()가 안티 패턴이며 적절한 해결책은?

    `isMounted()`의 주요 사용 사례는 컴포넌트가 마운트 해제된 후에 `setState()`를 호출하지 않도록 경고하는 것이다.

    ```javascript
    if (this.isMounted()) {
      this.setState({...})
    }
    ```

    `setState()`를 호출하기 전에 `isMounted()`를 검사하면 경고가 제거되지만, 경고의 목적도 상실된다. 컴포넌트가 마운트 해제된 후에 참조를 보유하고 있다고 생각하기 때문에 `isMounted()`를 사용하는 것은 코드 스멜이다.

    최적의 해결책은 컴포넌트가 마운트 해제된 후에 `setState()`가 호출될 수 있는 위치를 찾아 수정하는 것이다. 이러한 상황은 컴포넌트가 일부 데이터를 기다리며, 데이터가 도착하기 전에 마운트 해제될 때 콜백으로 인해 가장 일반적으로 발생한다. 이상적으로, 콜백은 마운트 해제 전에 `componentWillUnmount()`에서 취소해야 한다.

86. ### React에서 지원되는 Pointer Events는?

    *Pointer Events*는 모든 입력 이벤트를 처리하는 통일된 방법을 제공한다. 예전에는 마우스와 각각의 이벤트 리스너가 있었지만, 요즘에는 터치스크린이나 펜이 달린 휴대전화와 같이 마우스와 관련 없는 장치가 많다. 이러한 이벤트는 *Pointer Events* 사양을 지원하는 브라우저에서만 작동한다는 것을 기억해야 한다.

    *React DOM*에서 다음 이벤트 유형을 사용할 수 있다.

    1. `onPointerDown`
    2. `onPointerMove`
    3. `onPointerUp`
    4. `onPointerCancel`
    5. `onGotPointerCapture`
    6. `onLostPointerCaptur`
    7. `onPointerEnter`
    8. `onPointerLeave`
    9. `onPointerOver`
    10. `onPointerOut`

87. ### 왜 컴포넌트의 이름은 대문자로 시작하나?

    JSX를 사용하여 컴포넌트를 렌더링하는 경우, 해당 컴포넌트의 이름은 대문자로 시작해야 한다. 그렇지 않으면 React가 인식할 수 없는 태그로 오류를 발생시킨다. 이 규칙은 HTML 요소와 SVG 태그만 소문자로 시작할 수 있기 때문에 사용된다.

    이름이 소문자로 시작하는 컴포넌트 클래스를 정의할 수 있지만 가져올 때 대문자여야 한다. 아래와 같은 소문자는 괜찮다.

    ```jsx harmony
    class myComponent extends Component {
      render() {
        return <div />
      }
    }

    export default myComponent
    ```

    다른 파일을 가져올 때 대문자로 시작해야 한다.

    ```jsx harmony
    import MyComponent from './MyComponent'
    ```

88. ### React v16에서 사용자 정의 DOM 속성을 지원하나?

    그렇다. 과거에 React는 알 수 없는 DOM 속성을 무시하곤 했다. React가 인식하지 못하는 속성을 가진 JSX를 작성했다면 React는 그냥 건너뛸 것이다. 예를 들면, 다음과 같다.

    ```jsx harmony
    <div mycustomattribute={'something'} />
    ```

    React v15로 빈 div를 DOM에 렌더링한다.

    ```html
    <div />
    ```

    React v16에서는 알 수 없는 속성이 DOM에 저장된다.

    ```html
    <div mycustomattribute='something' />
    ```

    이것은 특정 브라우저 비표준 속성을 제공하고, 새로운 DOM API를 사용하고, 라이브러리와 통합할 때 유용하다.

89. ### constructor과 getInitialState의 차이점은?

    ES6의 클래스를 사용할 때는 생성자에서 상태를 초기화하고 `React.createClass()`를 사용할 때는  `getInitialState()` 메서드를 초기화해야 한다.

    ES6 클래스 사용 시

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        this.state = { /* initial state */ }
      }
    }
    ```

    `React.createClass()` 사용 시

    ```javascript
    const MyComponent = React.createClass({
      getInitialState() {
        return { /* initial state */ }
      }
    })
    ```

    **Note:** `React.createClass()`는 더 이상 사용되지 않으며 React v16에서 제거되었다. 대신에 자바스크립트 클래스를 사용해야 한다.

90. ### setState를 호출하지 않고도 컴포넌트 리렌더링이 가능한가?

    기본적으로, 컴포넌트의 state 또는 props가 변경되면 컴포넌트가 리렌더링이 된다. `render()` 메서드가 다른 데이터에 의존하는 경우, `forceUpdate()`를 호출하여 컴포넌트의 렌더링을 다시 해야 한다는 것을 React에게 알릴 수 있다.

    ```javascript
    component.forceUpdate(callback)
    ```

    `forceUpdate()`의 사용은 피하고 `render()`의 `this.props`과 `this.state`에서 읽기만 하는 것이 좋다.

91. ### ES6 클래스를 사용하는 React에서 super()와 super(props)의 차이점은?

    `constructor()`에서 `this.props`에 접근하려면 props를 `super()` 메서드에 전달해야 한다.

    `super(props)` 사용 시:

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super(props)
        console.log(this.props) // { name: 'John', ... }
      }
    }
    ```

    `super()` 사용 시:

    ```javascript
    class MyComponent extends React.Component {
      constructor(props) {
        super()
        console.log(this.props) // undefined
      }
    }
    ```

    `constructor()` 외부에서는 `this.props`에 대해서 같은 값을 표시한다.

92. ### JSX 내부에서 반복하는 방법?

    ES6 *화살표 함수* 구문과 함께 `Array.prototype.map`을 간단히 사용할 수 있다. 예를 들어, 객체의 `items` 배열은 다음과 같은 컴포넌트의 배열과 매핑된다.

    ```jsx harmony
    <tbody>
      {items.map(item => <SomeComponent key={item.id} name={item.name} />)}
    </tbody>
    ```

    `for` 반복문을 사용하여 반복할 수 없다.

    ```jsx harmony
    <tbody>
      for (let i = 0; i < items.length; i++) {
        <SomeComponent key={items[i].id} name={items[i].name} />
      }
    </tbody>
    ```

    JSX 태그가 *함수 호출*로 변환되어 표현식안에 명령문을 사용할 수 없기 때문이다. 이것은 *stage 1 proposal*에 `올라가 있기` 때문에 바뀔수 있다.

93. ### 속성 인용문에 props를 어떻게 넣나?

    React (또는 JSX)는 속성값 내부의 변수 보간을 지원하지 않는다. 아래의 표현은 작동하지 않는다.

    ```jsx harmony
    <img className='image' src='images/{this.props.image}' />
    ```

    그러나 JS 표현식을 중괄호 안에 전체 속성값으로 넣을 수 있다. 따라서, 아래 표현식이 작동한다.

    ```jsx harmony
    <img className='image' src={'images/' + this.props.image} />
    ```

    *템플릿 문자열*을 사용하면 다음과 같이 사용할 수 있다.

    ```jsx harmony
    <img className='image' src={`images/${this.props.image}`} />
    ```

94. ### 모양이 있는 React proptype array란?

    특정 모양의 컴포넌트에 객체 배열을 전달하려면 `React.PropTypes.arrayOf()`에 대한 인수로 `React.PropTypes.shape()`를 사용한다.

    ```javascript
    ReactComponent.propTypes = {
      arrayWithShape: React.PropTypes.arrayOf(React.PropTypes.shape({
        color: React.PropTypes.string.isRequired,
        fontSize: React.PropTypes.number.isRequired
      })).isRequired
    }
    ```

95. ### 클래스 속성을 조건부로 적용하는 방법은?

    따옴표 안에서 중괄호를 사용하면 문자열로 평가되기 때문에 중괄호를 사용하면 안 된다.

    ```jsx harmony
    <div className="btn-panel {this.props.visible ? 'show' : 'hidden'}">
    ```

    대신 중괄호를 바깥으로 옮겨야 한다. (클래스 이름들 사이에 공백을 넣는 것을 잊지 말아야 한다.)

    ```jsx harmony
    <div className={'btn-panel ' + (this.props.visible ? 'show' : 'hidden')}>
    ```

    *템플릿 문자열*도 작동한다.

    ```jsx harmony
    <div className={`btn-panel ${this.props.visible ? 'show' : 'hidden'}`}>
    ```

96. ### React와 ReactDOM의 차이점?

    `react` 패키지는 `React.createElement()`, `React.Component`, `React.Children`, 엘리먼트 컴포넌트 및 클래스와 관련된 기타 도우미가 포함되어 있다. 컴포넌트를 만들 때 필요한 동형 또는 보편적인 도우미라고 생각할 수 있다. `react-dom` 패키지에는 `ReactDOM.render()`가 포함되어 있고, `react-dom/server`에는 `ReactDOMServer.renderToString()`과 `ReactDOMServer.renderToStaticMarkup()`을 사용하여 *서버 사이드 렌더링*을 지원한다.

97. ### 왜 ReactDOM은 React와 분리되었나?

    React 팀은 모든 DOM 관련 기능을 *ReactDOM*이라는 별도의 라이브러리로 분리했다. React v0.14는 라이브러리가 분리된 첫 번째 릴리즈이다. `react-native`, `react-art`, `react-canvas`, `react-three` 같은 일부 패키지를 살펴보면, React의 아름다움과 본질은 브라우저나 DOM과는 관련이 없다는 것을 분명히 한다. React가 렌더링할 수 있는 더 많은 환경을 구축하기 위해, React 팀은 주 React 패키지를 `react`와 `react-dom` 두 개로 나눌 계획을 세웠다. 이는 React과 React Native의 웹 버전 간에 공유할 수 있는 컴포넌트를 작성하는 길을 열어주었다.

98. ### React 라벨 엘리먼트를 사용하는 방법은?

    표준 `for` 속성을 사용하여 텍스트 입력에 바인드된 `<label>` 엘리먼트를 렌더링하려고 하면, 해당 속성이 없는 HTML이 생성되고 콘솔에 경고가 인쇄된다.

    ```jsx harmony
    <label for={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```

    `for`는 JavaScript에서 예약된 키워드이므로, 대신 `htmlFor`을 사용해야 한다.

    ```jsx harmony
    <label htmlFor={'user'}>{'User'}</label>
    <input type={'text'} id={'user'} />
    ```

99. ### 여러 개의 인라인 스타일 객체를 결합하는 방법은?

    일반적인 React에서 사용하는 *spread 연산자*.

    ```jsx harmony
     <button style={{...styles.panel.button, ...styles.panel.submitButton}}>{'Submit'}</button>
    ```

    React Native를 사용한다면 배열 표기법을 사용할 수 있다.

    ```jsx harmony
    <button style={[styles.panel.button, styles.panel.submitButton]}>{'Submit'}</button>
    ```

100. ### 브라우저 크기를 조정할 때 뷰를 리렌더링하는 방법은?

     `componentDidMount()`에서 `resize` 이벤트를 수신하면, 크기(`너비` 및 `높이`)를 업데이트 할 수 있다. `componentWillUnmount()` 메서드에서 리스너를 제거해야 한다.

     ```javascript
     class WindowDimensions extends React.Component {
       constructor(props){
         super(props);
         this.updateDimensions = this.updateDimensions.bind(this);
       }
        
       componentWillMount() {
         this.updateDimensions()
       }

       componentDidMount() {
         window.addEventListener('resize', this.updateDimensions)
       }

       componentWillUnmount() {
         window.removeEventListener('resize', this.updateDimensions)
       }

       updateDimensions() {
         this.setState({width: window.innerWidth, height: window.innerHeight})
       }

       render() {
         return <span>{this.state.width} x {this.state.height}</span>
       }
     }
     ```

101. ### `setState()`와 `replaceState()` 메서드의 차이점은?

     `setState()`를 사용하면 현재 state와 이전 state가 병합된다. `replaceState()`는 현재 state를 버리고 사용자가 넣은 state로 바꾼다. Usually 어떤 이유로 이전의 모든 키를 제거해야 하는 경우가 아니면 `setState()`를 사용한다. `replaceState()`를 사용하는 대신 `setState()`에서 state를 `false`/`null`로 설정할 수도 있다.

102. ### state 변경을 인지하는 방법?

     state가 변경되면 다음의 라이프 사이클 메서드가 호출된다. 제공된 state와 props 값을 현재 state, props와 비교하여 의미 있는 것이 변경되었는지 확인할 수 있다.

     ```
     componentWillUpdate(object nextProps, object nextState)
     componentDidUpdate(object prevProps, object prevState)
     ```

103. ### React state에서 배열 엘리먼트를 제거하는 권장 방법은?

     더 나은 방법은 `Array.prototype.filter()` 메서드를 사용하는 것이다.

     예를 들어, state를 업데이트하기 위한 `removeItem()` 메서드를 생성해보자

     ```javascript
     removeItem(index) {
       this.setState({
         data: this.state.data.filter((item, i) => i !== index)
       })
     }
     ```

104. ### HTML 렌더링없이 React를 사용할 수 있나?

     최신버전 (>=16.2)에서 가능하다. 가능한 옵션은 아래와 같다.

     ```jsx harmony
     render() {
       return false
     }
     ```

     ```jsx harmony
     render() {
       return null
     }
     ```

     ```jsx harmony
     render() {
       return []
     }
     ```

     ```jsx harmony
     render() {
       return <React.Fragment></React.Fragment>
     }
     ```

     ```jsx harmony
     render() {
       return <></>
     }
     ```

     `undefined` 반환은 작동하지 않는다

105. ### React에서 JSON을 이쁘게 출력하는 방법?

     `<pre>` 태그를 사용하여 `JSON.stringify()`의 서식이 유지되도록 할 수 있다.

     ```jsx harmony
     const data = { name: 'John', age: 42 }

     class User extends React.Component {
       render() {
         return (
           <pre>
             {JSON.stringify(data, null, 2)}
           </pre>
         )
       }
     }

     React.render(<User />, document.getElementById('container'))
     ```

106. ### React에서 props를 업데이트할 수 없는 이유는?

     React 철학은 props가 *불변*이고 *하향식*이어야 한다는 것이다. 즉, 부모는 모든 props 값을 자식에게 보낼 수 있지만, 자식은 받은 props를 수정할 수 없다.

107. ### 페이지 로드 시 input 엘리먼트에 포커스를 주는 방법은?

     `input` 엘리먼트에 대한 *ref*를 생성하고 `componentDidMount()`에서 이를 사용한다.

     ```jsx harmony
     class App extends React.Component{
       componentDidMount() {
         this.nameInput.focus()
       }

       render() {
         return (
           <div>
             <input
               defaultValue={'Won\'t focus'}
             />
             <input
               ref={(input) => this.nameInput = input}
               defaultValue={'Will focus'}
             />
           </div>
         )
       }
     }

     ReactDOM.render(<App />, document.getElementById('app'))
     ```

108. ### state에서 객체를 업데이트 할 수 있는 방법은?

     1. **state와 병합 할 객체가 있는 `setState()`를 호출한다.**

         * `Object.assign()`를 사용하여 객체의 복사본을 만든다:

             ```javascript
             const user = Object.assign({}, this.state.user, { age: 42 })
             this.setState({ user })
             ```

         * *spread 연산자*를 사용한다.

             ```javascript
             const user = { ...this.state.user, age: 42 }
             this.setState({ user })
             ```

     2. **`setState()`를 함수와 같이 사용한다.**

         ```javascript
         this.setState(prevState => ({
           user: {
             ...prevState.user,
             age: 42
           }
         }))
         ```

109. ### 왜 함수가 `setState()` 객체보다 선호되는가?

     React는 여러 `setState()` 호출을 성능 향상을 위해 단일 업데이트로 일괄처리한다. `this.props`와 `this.state`가 비동기적으로 업데이트될 수 있음으로 다음 state를 계산할 때 해당 값을 신뢰해서는 안 된다.

     counter 예제는 예상대로 업데이트되지 않는다.

     ```javascript
     // Wrong
     this.setState({
       counter: this.state.counter + this.props.increment,
     })
     ```

     선호되는 접근법은 객체가 아닌 함수로 `setState()`를 호출하는 것이다. 이 함수는 첫 번째 인수로 이전 state를 받고 두 번째 인수로 업데이트가 적용된 props를 받는다.

     ```javascript
     // Correct
     this.setState((prevState, props) => ({
       counter: prevState.counter + props.increment
     }))
     ```

110. ### 브라우저 런타임에 React 버전을 어떻게 알 수 있나?

     `React.version`을 사용해서 버전을 얻을 수 있다.

     ```jsx harmony
     const REACT_VERSION = React.version

     ReactDOM.render(
       <div>{`React version: ${REACT_VERSION}`}</div>,
       document.getElementById('app')
     )
     ```

111. ### `create-react-app`에 polyfill을 포함시키는 방법은?

     1. **`core-js`에서 수동으로 가져오기**

         `polyfills.js`와 같은 파일을 만들고 root `index.js` 파일에서 import한다. `npm install core-js` 또는 `yarn add core-js`를 실행하고 특정 필수 기능을 import한다.

         ```javascript
         import 'core-js/fn/array/find'
         import 'core-js/fn/array/includes'
         import 'core-js/fn/number/is-nan'
         ```

     2. **Polyfill 서비스를 사용하기:**

         이 줄을 `index.html`에 추가, polyfill.io CDN을 사용하여 사용자 지정 브라우저 전용 polyfill을 검색한다.

         ```html
         <script src='https://cdn.polyfill.io/v2/polyfill.min.js?features=default,Array.prototype.includes'></script>
         ```

         위의 스크립트에서 `Array.prototype.includes` 기능은 기본 기능 집합에 포함되어 있지 않음으로 명시적으로 요청해야 한다.

112. ### create-react-app에서 http 대신 https를 사용하는 방법?

     `HTTPS=true` 설정만 사용하면 된다. `package.json` 스크립트 섹션을 편집할 수 있다.

     ```json
     "scripts": {
       "start": "set HTTPS=true && react-scripts start"
     }
     ```

     또는 `set HTTPS=true && npm start`를 실행하면 된다.

113. ### create-react-app에서 상대 경로 가져오기 사용을 피하는 방법?

     프로젝트 루트에 `.env`라는 파일을 만들고 경로를 import 하면 된다. 

     ```
     NODE_PATH=src/app
     ```

     개발 서버를 다시 시작하면, 상대 경로 없이 `src/app` 내부의 내용을 import 할 수 있다.

114. ### React Router용 Google 웹 로그 분석을 추가하는 방법은?

     `history` 객체에 리스너를 추가하여 각각의 페이지 view를 기록한다.

     ```javascript
     history.listen(function (location) {
       window.ga('set', 'page', location.pathname + location.search)
       window.ga('send', 'pageview', location.pathname + location.search)
     })
     ```

115. ### 매 초마다 컴포넌트를 업데이트 하는 방법은?

     변경을 감지하려면 `setInterval()`을 사용해야 하지만 오류 및 메모리 누수를 방지하려면 컴포넌트가 마운트 해제될 때 타이머를 지워야 한다.

     ```javascript
     componentDidMount() {
       this.interval = setInterval(() => this.setState({ time: Date.now() }), 1000)
     }

     componentWillUnmount() {
       clearInterval(this.interval)
     }
     ```

116. ### React에서 인라인 스타일에 벤더 접두사는 어떻게 적용하나?

     React는 *벤더 접두사*를 자동으로 **적용하지 않는다**. 벤더 접두사를 수동으로 추가해야 한다.

     ```jsx harmony
     <div style={{
       transform: 'rotate(90deg)',
       WebkitTransform: 'rotate(90deg)', // note the capital 'W' here
       msTransform: 'rotate(90deg)' // 'ms' is the only lowercase vendor prefix
     }} />
     ```

117. ### React와 ES6를 사용해서 컴포넌트를 가져오고 내보내는 방법은?

     컴포넌트를 내보내려면 default를 사용하면 된다.

     ```jsx harmony
     import React from 'react'
     import User from 'user'

     export default class MyProfile extends React.Component {
       render(){
         return (
           <User type="customer">
             //...
           </User>
         )
       }
     }
     ```

      export 지정자를 사용하면 MyProfile이 멤버가 되어 이 모듈로 내보낼 수 있으며, 다른 컴포넌트에 이름을 언급하지 않고도 가져올 수 있다. 

118. ### React 컴포넌트 이름이 대문자로 시작해야 하는 이유는?

     JSX에서 소문자 태그 이름은 HTML 태그로 간주한다. 그러나 점으로 표시된 대문자 및 소문자 태그 이름(속성 접근자)은 없다.

     1. `<component />`는 `React.createElement('component')`로 컴파일된다. (i.e, HTML tag)
     2. `<obj.component />`는 `React.createElement(obj.component)`로 컴파일된다.
     3. `<Component />`는 `React.createElement(Component)`로 컴파일된다.

119. ### 컴포넌트 생성자는 왜 한 번만 불리나?

     React의 *reconciliation* 알고리즘에서는 정반대 정보가 없다고 가정하는데, 사용자 지정 컴포넌트가 후속 렌더링의 같은 위치에 나타나면, 이전 컴포넌트와 동일 하므로 이전 인스턴스를 새로 작성하지 않고 다시 사용한다.

120. ### React에서 상수를 정의하는 방법은?

     ES7 `static` 필드를 사용하여 상수를 정의할 수 있다.

     ```javascript
     class MyComponent extends React.Component {
       static DEFAULT_PAGINATION = 10
     }
     ```

     *Static fields*는 *Class Fields* 스테이지 3 제안의 일부이다.

121. ### React에서 프로그래밍 방식으로 클릭 이벤트를 발생시키는 방법은?

     ref prop를 사용하여 콜백을 통해 기본 `HTMLInputElement` 객체에 대한 참조를 가져와서, 참조를 클래스 속성으로 저장한 다음, 해당 참조의 `HTMLElement.click` 메서드를 사용하여 이벤트 핸들러에서 클릭을 트리거 할 수 있다.

     1. render 메서드 안에서 ref를 만든다.

         ```jsx harmony
         <input ref={input => this.inputElement = input} />
         ```

     2. 이벤트 핸들러에 클릭 이벤트를 적용한다.

         ```javascript
         this.inputElement.click()
         ```

122. ### async/await를 평범한 React에서 사용할 수 있나?

     React에서 `async`/`await`을 사용하려면, *Babel* 및 [transform-async-to-generator](https://babeljs.io/docs/en/babel-plugin-transform-async-to-generator) 플러그인이 필요하다. React Native는 Babel과 변경 세트를 구성해야 한다.

123. ### React의 일반적인 폴더 구조는?

     React 프로젝트 파일 구조는 일반적으로 사용되는 2가지 방법이 있다.

     1. **기능 또는 경로별로 그룹화**

         프로젝트를 구조화하는 일반적인 방법의 하나는 기능이나 경로별로 그룹화된 CSS, JS, 및 테스트를 함께 배치하는 것이다.

         ```
         common/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ APIUtils.js
         └─ APIUtils.test.js
         feed/
         ├─ index.js
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         └─ FeedAPI.js
         profile/
         ├─ index.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         ├─ ProfileHeader.css
         └─ ProfileAPI.js
         ```

     2. **파일 타입으로 그룹화**

         프로젝트를 구조화하는 다른 보편적인 방법은 유사한 파일끼리 그룹화하는 것이다.

         ```
         api/
         ├─ APIUtils.js
         ├─ APIUtils.test.js
         ├─ ProfileAPI.js
         └─ UserAPI.js
         components/
         ├─ Avatar.js
         ├─ Avatar.css
         ├─ Feed.js
         ├─ Feed.css
         ├─ FeedStory.js
         ├─ FeedStory.test.js
         ├─ Profile.js
         ├─ ProfileHeader.js
         └─ ProfileHeader.css
         ```

124. ### 인기 애니메이션 패키지는?

     *React Transition Group*과 *React Motion*이 React 생태계에서 가장 인기 있는 애니메이션 패키지이다.

125. ### 스타일 모듈의 이점은?

     컴포넌트에서 스타일 값을 하드 코딩 하는 것은 좋지 않다. 다른 UI 컴포넌트에서 사용될 가능성이 있는 값은 자체 모듈로 뽑아내야 한다.

     예를 들어, 이러한 스타일은 별도의 컴포넌트로 뽑아낼 수 있다.

     ```javascript
     export const colors = {
       white,
       black,
       blue
     }

     export const space = [
       0,
       8,
       16,
       32,
       64
     ]
     ```

     그런 다음 다른 컴포넌트에서 개별적으로 가져온다.

     ```javascript
     import { space, colors } from './styles'
     ```

126. ### 인기있는 React-관련 linters는?

     ESLint는 인기 있는 JavaScript linter이다. 특정 코드 스타일을 분석할 수 있는 플러그인이 있다. React에서 가장 일반적으로 사용되는 패키지 중 하나는 `eslint-plugin-react` npm 패키지다. 기본적으로, 반복자에게 있는 키부터 전체 prop 타입까지 검사하는 규칙을 사용하여 가장 좋은 사례를 여러 번 확인할 것이다. 또 다른 인기 있는 플러그인은 `eslint-plugin-jsx-a11y`로, 접근성과 관련된 일반적인 문제를 해결하는 데 도움이 된다. JSX는 일반 HTML과 약간 다른 구문을 제공하기 때문에 `alt` 텍스트나 `tabindex`와 관련된 문제는 일반적인 플러그인으로 찾아낼 수 없다.

127. ### AJAX 호출하는 방법과 어느 컴포넌트 라이프 사이클 메서드에서 AJAX 호출을 해야하나?

     Axios, jQuery AJAX 및 브라우저 내장 `fetch`와 같은 AJAX libraries를 사용할 수 있다. `componentDidMount()` 라이프 사이클 메서드에서 데이터를 가져와야 한다. 데이터를 검색할 때 `setState()`를 사용하여 컴포넌트를 업데이트 할 수 있다.

     예를 들어, 직원 목록은 API에서 가져와서 로컬 state에 설정한다.

     ```jsx harmony
     class MyComponent extends React.Component {
       constructor(props) {
         super(props)
         this.state = {
           employees: [],
           error: null
         }
       }

       componentDidMount() {
         fetch('https://api.example.com/items')
           .then(res => res.json())
           .then(
             (result) => {
               this.setState({
                 employees: result.employees
               })
             },
             (error) => {
               this.setState({ error })
             }
           )
       }

       render() {
         const { error, employees } = this.state
         if (error) {
           return <div>Error: {error.message}</div>;
         } else {
           return (
             <ul>
               {employees.map(item => (
                 <li key={employee.name}>
                   {employee.name}-{employees.experience}
                 </li>
               ))}
             </ul>
           )
         }
       }
     }
     ```

128. ### render props란?

     **Render Props**는 값이 함수인 prop을 사용하여 컴포넌트 간 코드를 공유하는 간단한 기술이다. 아래의 컴포넌트는 React 엘리먼트를 반환하는 render props를 사용한다.

     ```jsx harmony
     <DataProvider render={data => (
       <h1>{`Hello ${data.target}`}</h1>
     )}/>
     ```

     React Router와 DownShift 같은 라이브러리는 이 패턴을 사용한다.

## React Router

1.   ### React Router란?

     React Router는 React 위에 구축된 강력한 라우팅 라이브러리로 URL을 페이지에 표시된 내용과 동기화된 상태로 유지하면서 애플리케이션에 새로운 화면과 플로우를 추가할 수 있다.

2.   ### React Router가 history 라이브러리와 다른점은?

     React Router는 브라우저의 `window.history`와 브라우저 해쉬 기록의 상호 작용을 처리하는 `history` 라이브러리를 감싸는 래퍼이다. 또한 모바일 히스토리를 제공하여 모바일 앱 개발(React Native) 및 Node 단위 테스트와 같이 글로벌 히스토리가 없는 환경에 유용하다.

3.   ### Router v4의 `<Router>` 컴포넌트는 무엇인가?

     React Router v4는 아래의 3개의 `<Router>` 컴포넌트를 제공한다.

     1. `<BrowserRouter>`
     2. `<HashRouter>`
     3. `<MemoryRouter>`

     위의 컴포넌트는 *browser*, *hash* 및 *memory* history 인스턴스를 생성한다. React Router v4는 `router` 객체의 컨텍스트를 통해서 사용 가능한 라우터와 연결된 `history` 인스턴스의 속성과 메서드를 사용할 수 있도록 한다.

4.   ### `history`의 `push()`, place()` 메서드의 목적은?

     history 인스턴스에는 탐색을 위한 두가지 메서드가 있다.

     1. `push()`
     2. `replace()`

     history를 방문한 위치의 배열로 생각하면 `push()`는 배열에 새 위치를 추가하고, `replace()`는 배열의 현재 위치를 새로운 위치로 바꾼다.

5.   ### React Router v4를 사용하여 프로그래밍 방식으로 어떻게 탐색하나?

     컴포넌트내에서 프로그래밍 방식의 라우팅 / 탐색을 수행하는 세 가지 방법이 있다.

     1. **`withRouter()` 고차 함수 사용**

        `withRouter()` 고차 함수는 history 객체를 컴포넌트의 prop로 삽입된다. 이 객체는 `push()` 및 `replace()` 메서드를 제공한다.

         ```jsx harmony
         import { withRouter } from 'react-router-dom' // this also works with 'react-router-native'

         const Button = withRouter(({ history }) => (
           <button
             type='button'
             onClick={() => { history.push('/new-location') }}
           >
             {'Click Me!'}
           </button>
         ))
         ```

     2. **`<Route>` 컴포넌트와 렌더링 props 패턴 사용**

         The `<Route>` 컴포넌트는 `withRouter()`와 같은 prop을 전달하므로, history prop을 통해 history 메서드에 접근할 수 있다.

         ```jsx harmony
         import { Route } from 'react-router-dom'

         const Button = () => (
           <Route render={({ history }) => (
             <button
               type='button'
               onClick={() => { history.push('/new-location') }}
             >
               {'Click Me!'}
             </button>
           )} />
         )
         ```

     3. **context 사용**

         이 옵션은 권장되지 않으며 불안정한 API로 처리된다.

         ```jsx harmony
         const Button = (props, context) => (
           <button
             type='button'
             onClick={() => {
               context.history.push('/new-location')
             }}
           >
             {'Click Me!'}
           </button>
         )

         Button.contextTypes = {
           history: React.PropTypes.shape({
             push: React.PropTypes.func.isRequired
           })
         }
         ```

6.   ### React Router v4에서 쿼리 매개 변수를 얻는 방법은?

     다른 구현을 지원하기 위해 수년 동안 사용자 요청이 있었기 때문에 쿼리 문자열을 구문 분석하는 기능은 React Router v4에서 제거되었다. 그래서 사용자가 원하는 구현을 선택하도록 결정되었다. 권장되는 방법은 쿼리 문자열 라이브러리를 사용하는 것이다.

     ```javascript
     const queryString = require('query-string');
     const parsed = queryString.parse(props.location.search);
     ```

     네이티브를 원한다면 `URLSearchParams`를 사용할 수도 있다.

     ```javascript
     const params = new URLSearchParams(props.location.search)
     const foo = params.get('name')
     ```

     IE11에서는 *polyfill*를 사용해야한다.

7.   ### 왜 "Router may have only one child element"라는 경고 메시지가 나오나?

     `<Switch>`는 라우터를 독점적으로 렌더링한다는 점에서 고유하므로 `<Switch>` 블록에 라우터를 감싸야 한다.

     먼저 `Switch`를 import 해준다.

     ```javascript
     import { Switch, Router, Route } from 'react-router'
     ```

     그런 다음 `<Switch>` 블록 내에서 경로를 정의한다.

     ```jsx harmony
     <Router>
       <Switch>
         <Route {/* ... */} />
         <Route {/* ... */} />
       </Switch>
     </Router>
     ```

8.   ### React Router v4의 `history.push` 메서드에 매개 변수를 전달하는 방법은?

      네비게이션하는 동안 `history` 객체에 props를 전달할 수 있다.

     ```javascript
     this.props.history.push({
       pathname: '/template',
       search: '?name=sudheer',
       state: { detail: response.data }
     })
     ```

     `search` 속성은 `push()` 메서드에서 쿼리 매개변수를 전달하는데 사용된다.

9.   ### *default* 또는 *NotFound* 페이지 구현 방법?

     `<Switch>`는 일치하는 첫 번째 하위 `<Route>`를 렌더링한다. 경로가 없는 `<Route>`는 항상 일치한다. 따라서 아래와 같은 경로 속성을 삭제하면 된다.

     ```jsx harmony
     <Switch>
       <Route exact path="/" component={Home}/>
       <Route path="/user" component={User}/>
       <Route component={NotFound} />
     </Switch>
     ```

10.  ### React Router v4에서 history를 얻는 방법은

     1. `history` 객체를 export 한 후 프로젝트 전체를 import 하는 모듈을 작성하면 된다.

         예를 들어, `history.js` 파일을 만든다.

         ```javascript
         import { createBrowserHistory } from 'history'

         export default createBrowserHistory({
           /* pass a configuration object here if needed */
         })
         ```

     2. 기본으로 제공되는 라우터 대신 `<Router>` 컴포넌트를 사용해야 한다. `index.js` 파일 내에서 `history.js`를 import 한다.

         ```jsx harmony
         import { Router } from 'react-router-dom'
         import history from './history'
         import App from './App'

         ReactDOM.render((
           <Router history={history}>
             <App />
           </Router>
         ), holder)
         ```

     3. 내장된 history 객체와 유사한 `history` 객체의 push 메서드를 사용할 수 있다.

         ```javascript
         // some-other-file.js
         import history from './history'

         history.push('/go-here')
         ```

11.  ### 로그인 후 자동 리디렉션을 수행하는 방법은?

     `react-router` 패키지는 React Router에서 `<Redirect>` 컴포넌트를 제공한다. `<Redirect>`을 렌더링하면 새로운 위치로 이동한다. 서버 사이드 리디렉션과 마찬가지로 새로운 위치는 history 스택의 현재 위치를 무시한다.

     ```javascript
     import React, { Component } from 'react'
     import { Redirect } from 'react-router'

     export default class LoginComponent extends Component {
       render() {
         if (this.state.isLoggedIn === true) {
           return <Redirect to="/your/redirect/page" />
         } else {
           return <div>{'Login Please'}</div>
         }
       }
     }
     ```

## React Internationalization

1.   ### What is React Intl?

     The *React Intl* library makes internalization in React straightforward, with off-the-shelf components and an API that can handle everything from formatting strings, dates, and numbers, to pluralization. React Intl is part of *FormatJS* which provides bindings to React via its components and API.

2.   ### What are the main features of React Intl?

     1. Display numbers with separators.
     2. Display dates and times correctly.
     3. Display dates relative to "now".
     4. Pluralize labels in strings.
     5. Support for 150+ languages.
     6. Runs in the browser and Node.
     7. Built on standards.

3.   ### What are the two ways of formatting in React Intl?

     The library provides two ways to format strings, numbers, and dates: react components or an API.

     ```jsx harmony
     <FormattedMessage
       id={'account'}
       defaultMessage={'The amount is less than minimum balance.'}
     />
     ```

     ```javascript
     const messages = defineMessages({
       accountMessage: {
         id: 'account',
         defaultMessage: 'The amount is less than minimum balance.',
       }
     })

     formatMessage(messages.accountMessage)
     ```

4.   ### How to use `<FormattedMessage>` as placeholder using React Intl?

     The `<Formatted... />` components from `react-intl` return elements, not plain text, so they can't be used for placeholders, alt text, etc. In that case, you should use lower level API `formatMessage()`. You can inject the `intl` object into your component using `injectIntl()` higher-order component and then format the message using `formatMessage()` available on that object.

     ```jsx harmony
     import React from 'react'
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => {
       const placeholder = intl.formatMessage({id: 'messageId'})
       return <input placeholder={placeholder} />
     }

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

5.   ### How to access current locale with React Intl?

     You can get the current locale in any component of your application using `injectIntl()`:

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const MyComponent = ({ intl }) => (
       <div>{`The current locale is ${intl.locale}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

6.   ### How to format date using React Intl?

     The `injectIntl()` higher-order component will give you access to the `formatDate()` method via the props in your component. The method is used internally by instances of `FormattedDate` and it returns the string representation of the formatted date.

     ```jsx harmony
     import { injectIntl, intlShape } from 'react-intl'

     const stringDate = this.props.intl.formatDate(date, {
       year: 'numeric',
       month: 'numeric',
       day: 'numeric'
     })

     const MyComponent = ({intl}) => (
       <div>{`The formatted date is ${stringDate}`}</div>
     )

     MyComponent.propTypes = {
       intl: intlShape.isRequired
     }

     export default injectIntl(MyComponent)
     ```

## React Testing

1.   ### What is Shallow Renderer in React testing?

     *Shallow rendering* is useful for writing unit test cases in React. It lets you render a component *one level deep* and assert facts about what its render method returns, without worrying about the behavior of child components, which are not instantiated or rendered.

     For example, if you have the following component:

     ```javascript
     function MyComponent() {
       return (
         <div>
           <span className={'heading'}>{'Title'}</span>
           <span className={'description'}>{'Description'}</span>
         </div>
       )
     }
     ```

     Then you can assert as follows:

     ```jsx harmony
     import ShallowRenderer from 'react-test-renderer/shallow'

     // in your test
     const renderer = new ShallowRenderer()
     renderer.render(<MyComponent />)

     const result = renderer.getRenderOutput()

     expect(result.type).toBe('div')
     expect(result.props.children).toEqual([
       <span className={'heading'}>{'Title'}</span>,
       <span className={'description'}>{'Description'}</span>
     ])
     ```

2.   ### What is `TestRenderer` package in React?

     This package provides a renderer that can be used to render components to pure JavaScript objects, without depending on the DOM or a native mobile environment. This package makes it easy to grab a snapshot of the platform view hierarchy (similar to a DOM tree) rendered by a ReactDOM or React Native without using a browser or `jsdom`.

     ```jsx harmony
     import TestRenderer from 'react-test-renderer'

     const Link = ({page, children}) => <a href={page}>{children}</a>

     const testRenderer = TestRenderer.create(
       <Link page={'https://www.facebook.com/'}>{'Facebook'}</Link>
     )

     console.log(testRenderer.toJSON())
     // {
     //   type: 'a',
     //   props: { href: 'https://www.facebook.com/' },
     //   children: [ 'Facebook' ]
     // }
     ```

3.   ### What is the purpose of ReactTestUtils package?

     *ReactTestUtils* are provided in the `with-addons` package and allow you to perform actions against a simulated DOM for the purpose of unit testing.

4.   ### What is Jest?

     *Jest* is a JavaScript unit testing framework created by Facebook based on Jasmine and provides automated mock creation and a `jsdom` environment. It's often used for testing components.

5.   ### What are the advantages of Jest over Jasmine?

     There are couple of advantages compared to Jasmine:

     - Automatically finds tests to execute in your source code.
     - Automatically mocks dependencies when running your tests.
     - Allows you to test asynchronous code synchronously.
     - Runs your tests with a fake DOM implementation (via `jsdom`) so that your tests can be run on the command line.
     - Runs tests in parallel processes so that they finish sooner.

6.   ### Give a simple example of Jest test case

     Let's write a test for a function that adds two numbers in `sum.js` file:

     ```javascript
     const sum = (a, b) => a + b

     export default sum
     ```

     Create a file named `sum.test.js` which contains actual test:

     ```javascript
     import sum from './sum'

     test('adds 1 + 2 to equal 3', () => {
       expect(sum(1, 2)).toBe(3)
     })
     ```

     And then add the following section to your `package.json`:

     ```json
     {
       "scripts": {
         "test": "jest"
       }
     }
     ```

     Finally, run `yarn test` or `npm test` and Jest will print a result:

     ```console
     $ yarn test
     PASS ./sum.test.js
     ✓ adds 1 + 2 to equal 3 (2ms)
     ```

## React Redux

1.   ### flux란?

     *Flux*는 전통적인 MVC 패턴의 대체품으로 사용되는 *애플리케이션 디자인 패러다임*이다. 이것은 단순히 프레임워크나 라이브러리가 아니라 React와 단방향 데이터 흐름의 개념을 보완하는 새로운 종류의 아키텍처이다. Facebook은 React로 작업할 때 이 패턴을 내부적으로 사용한다.

     디스패처 간 워크플로우는 다음과 같이 고유한 입력 및 출력으로 구성 요소를 저장하고 볼 수 있다.

     ![flux](images/flux.png)

2.   ### Redux란?

     *Redux*는 *Flux 디자인 패턴*을 기반으로하는 JavaScript 앱을 위한 예측 가능한 상태 컨테이너이다. Redux는 React와 함께 또는 다른 뷰 라이브러리와 함께 사용할 수 있다. 크기가 작고(2kB 정도) 종속성이 없다.

3.   ### Redux의 핵심 원칙은?

     Redux는 세 가지 기본원칙을 따른다.

     1. **진실의 단일 소스(Single source of truth):** 전체 애플리케이션의 state는 단일 저장소 내 Object Tree에 저장된다. 단일 state 트리를 사용하면 시간이 지남에 따른 변경사항을 추적하고 응용 프로그램을 디버그 또는 검사하기에 쉽다.
     2. **State는 읽기 전용:** state를 변경하는 유일한 방법은 무슨 일이 있었는지 설명한 객체인 action을 내보내는 것이다. 뷰나 네트워크 콜백이 state에 직접 쓰지 않는다.
     3. **Changes are made with pure functions:** 작업에 의해 state 트리가 변환되는 action을 지정하려면 reducer를 작성해야 한다. Reducers는 이전의 state와 action을 파라미터로 사용하고, 다음의 state를 return 하는 순수함수이다.

4.   ### Flux와 비교한 Redux의 단점은?

     단점 대신에 Flux를 통해 Redux을 사용하면 더럽히는 일이 거의 없다.

     1. **Mutation을 피하는 방법을 배워야 한다.:** Flux는 데이터 변경에 대해 의견이 많지 않지만, Redux는 mutation을 좋아하지 않으며 Redux를 보완하는 많은 패키지는 state를 절대로 변경하지 않는 것을 가정한다. `redux-immutable-state-invariant`, Immutable.js와 같은 개발 전용 패키지를 사용하거나 팀에게 변경하지 않는 코드를 작성하도록 지시하여 적용할 수 있다.
     2. **packages를 신중하게 선택해야 한다.:** Flux는 실행 취소 / 다시 실행, 지속성 또는 양식과 같은 문제를 명시적으로 해결하려고 시도하지 않지만, Redux에는 미들웨어 및 저장소 향상기와 같은 익스텐션이 있으며 풍부한 에코 시스템을 생성했다.
     3. **아직 좋은 흐름 통합은 없다.:** Flux는 현재 Redux가 지원하지 않는 매우 인상적인 정적 유형 검사를 수행 할 수 있다.

5.   ### `mapStateToProps()`과 `mapDispatchToProps()`의 차이점은?

     `mapStateToProps()`는 컴포넌트가 다른 컴포넌트에 의해 업데이트된 state를 받아오는데 도와주는 유틸리티이다.

     ```javascript
     const mapStateToProps = (state) => {
       return {
         todos: getVisibleTodos(state.todos, state.visibilityFilter)
       }
     }
     ```

     `mapDispatchToProps()`는 컴포넌트가 응용프로그램 state 변경을 일으키는 dispatching action 이벤트를 발생시키는데 도와주는 유틸리티이다.

     ```javascript
     const mapDispatchToProps = (dispatch) => {
       return {
         onTodoClick: (id) => {
           dispatch(toggleTodo(id))
         }
       }
     }
     ```
     
     `mapDispatchToProps`에 대해서 항상 "객체 약식(object shorthand)" 양식을 사용하는 것을 추천한다.
        
     Redux는 (…args) => dispatch(onTodoClick(…args))와 같은 다른 함수로 래핑하고 해당 래퍼 함수를 ​​컴포넌트의 prop으로 전달합니다.
      
      ```javascript
       const mapDispatchToProps = ({
         onTodoClick
       })
      ```

6.   ### reducer에서 action을 전달할 수 있나?

     reducer 내에서 action을 전달하는 것은 **anti-pattern**이다. 리듀서는  *사이드 이펙트(side effects)* 가 없어야 한다. 단순히 action payload를 소화하고 새로운 state 객체를 반환한다. reducer 내에 리스너를 추가하고 action을 전달하면, 연쇄적으로 action 및 다른 사이드 이펙트가 발생할 수 있다.

7.   ### 컴포넌트 외부의 Redux store에 접근하는 방법은?

     `createStore()`로 작성된 모듈에서 store를 내보내면 된다. 또한, 전역 window 객체를 오염시키지 않아야 한다.

     ```javascript
     store = createStore(myReducer)

     export default store
     ```

8.   ### MVW 패턴의 단점은 무엇인가?

     1. DOM 조작은 비용이 많이 들어서 애플리케이션이 느리고 비효율적으로 작동하게 한다.
     2. 순환 종속성으로 인해, 모델과 뷰를 중심으로 한 복잡한 모델이 생성된다.
     3. 구글 같은 공동작업 응용프로그램에서는 많은 데이터 변경이 발생한다.
     4. 엄청 많은 코드를 추가하지 않고서는 쉽게 되돌릴 방법이 없다.

9.   ### Redux와 RxJS의 비슷한 점은?

     이 라이브러리들은 다른 목적을 가진다는 점에서 매우 다르지만, 모호한 유사점을 가진다.

     Redux는 애플리케이션 전체에서 state를 관리하기 위한 도구이다. 일반적으로 UI 아키텍처로 사용된다. 이것을 Angular의 절반에 해당하는 대안이라고 생각하자. RxJS는 reactive 프로그래밍 라이브러리이다. 일반적으로 JavaScript에서 비동기 작업을 수행하는 도구로 사용된다. 이것을 Promises의 대안이라고 생각하자. Redux는 store가 reactive 하기 때문에 Reactive 패러다임을 사용한다. Store는 멀리서 행동을 관찰하고 스스로 변화시킨다. RxJS는 또한 Reactive 패러다임을 사용하지만, 아키텍처를 대체하는 것이 아닌 패턴을 달성하기 위한 기본 설계 블록, Observables를 제공한다.

10.  ### 로드 시점에 action을 전달하는 방법은?

    `componentDidMount()` 메서드에서 action을 전달할 수 있고 `render()` 메서드에서 데이터를 확인할 수 있다.

     ```javascript
     class App extends Component {
       componentDidMount() {
         this.props.fetchData()
       }

       render() {
         return this.props.isLoaded
           ? <div>{'Loaded'}</div>
           : <div>{'Not Loaded'}</div>
       }
     }

     const mapStateToProps = (state) => ({
       isLoaded: state.isLoaded
     })

     const mapDispatchToProps = { fetchData }

     export default connect(mapStateToProps, mapDispatchToProps)(App)
     ```

11.  ### React Redux에서 `connect()`를 사용하는 방법은?

     container에서 store를 사용하려면 다음 두 단계를 수행해야 한다.

     1. **`mapStateToProps() 사용하기`:** store의 state 변수를 지정한 props에 매핑한다
     2. **위의 props와 컨테이너를 연결하기:** `mapStateToProps` 함수로 반환한 객체가 컨테이너에 연결되어 있다. `react-redux`에서 `connect()`를 가져올 수 있다.

         ```jsx harmony
         import React from 'react'
         import { connect } from 'react-redux'

         class App extends React.Component {
           render() {
             return <div>{this.props.containerData}</div>
           }
         }

         function mapStateToProps(state) {
           return { containerData: state.data }
         }

         export default connect(mapStateToProps)(App)
         ```

12.  ### Redux에서 state를 재설정하는 방법은?

     `combineReducers()` 으로 만들어진 reducer의 action 처리를 위임하는 *root reducer* 를 애플리케이션에 작성해야 한다.

     예를 들어, `USER_LOGOUT` action 후 초기 state를 리턴하기 위해 `rootReducer()` 를 사용하여야 한다. 알다시피, reducer는 action과 관계없이 첫 번째 인수로 `undefined` 로 호출될 때 초기 상태를 반환해야 한다.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         state = undefined
       }

       return appReducer(state, action)
     }
     ```

     `redux-persist`를 사용하는 경우, storage를 정리해야 할 수 있다. `redux-persist` 는 state 엔진을 storage 엔진에 보관한다. 먼저, 적절한 storage 엔진을 가져와서 state 키를 정의하지 않고 정리하기 전에 state를 구문 분석해야 한다.

     ```javascript
     const appReducer = combineReducers({
       /* your app's top-level reducers */
     })

     const rootReducer = (state, action) => {
       if (action.type === 'USER_LOGOUT') {
         Object.keys(state).forEach(key => {
           storage.removeItem(`persist:${key}`)
         })

         state = undefined
       }

       return appReducer(state, action)
     }
     ```

13.  ### Redux connect 데코레이터에서 `at` 기호의 목적은?

     **@** 기호는 실제로 데코레이터를 나타내는데 사용되는 JavaScript 표현식이다. *데코레이터* 를 사용하면 디자인 타임에 클래스와 속성에 주석을 달고 수정할 수 있다.

     데코레이터를 사용하는 것과 사용하지 않고 Redux를 설정하는 예를 살펴보자.

     * **데코레이터가 없을 경우:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         class MyApp extends React.Component {
           // ...define your main app here
         }

         export default connect(mapStateToProps, mapDispatchToProps)(MyApp)
         ```

     * **데코레이터가 있을 경우:**

         ```javascript
         import React from 'react'
         import * as actionCreators from './actionCreators'
         import { bindActionCreators } from 'redux'
         import { connect } from 'react-redux'

         function mapStateToProps(state) {
           return { todos: state.todos }
         }

         function mapDispatchToProps(dispatch) {
           return { actions: bindActionCreators(actionCreators, dispatch) }
         }

         @connect(mapStateToProps, mapDispatchToProps)
         export default class MyApp extends React.Component {
           // ...define your main app here
         }
         ```

     위의 예제들는 데코레이터 사용을 제외하고는 거의 비슷하다. 데코레이터 구문은 아직 JavaScript 런타임에 내장되어 있지 않다. 실험 중이며 변경될 수 있다. 현재 데코레이터 지원을 위해서 babel을 사용하면 된다.

14.  ### React context와 React Redux의 차이점은?

     응용 프로그램에 **Context** 를 바로 사용할 수 있으며 설계된 중첩된 컴포넌트에 데이터를 전달하는 데 유용하다. 반면 **Redux** 는 훨씬 강력하고 Context API가 제공하지 않는 많은 기능을 제공한다. 또한, React Redux 는 내부적으로 Context를 사용하지만, 이 사실을 public API에 알리지 않는다.

15.  ### Redux state 함수가 reducer라고 불리는 이유는?

     Reducers는 항상 state의 누적을 반환한다(모든 이전과 현재의 action을 기반으로 한다). 그러므로, state를 줄이는 역할을 한다. Redux reducer가 호출될 때마다 state 및 action이 매개변수로 전달된다. 그런 다음 state는 action에 따라 감속(또는 누적)되고 다음 state가 반환된다. action 컬렉션 및 결과적인 최종 state를 얻기 위해 이러한 state를 수행할 store의 초기 상태를 *줄일 수 있다*.

16.  ### Redux에서 AJAX를 요청하는 방법은?

     비동기 action을 정의할 수 있는 `redux-thunk` 미들웨어를 사용할 수 있다.

     *fetch API* 를 사용하여 특정 계정을 AJAX 호출로 가져오는 예시를 들어보자.

     ```javascript
     export function fetchAccount(id) {
       return dispatch => {
         dispatch(setLoadingAccountState()) // Show a loading spinner
         fetch(`/account/${id}`, (response) => {
           dispatch(doneFetchingAccount()) // Hide loading spinner
           if (response.status === 200) {
             dispatch(setAccount(response.json)) // Use a normal function to set the received state
           } else {
             dispatch(someError)
           }
         })
       }
     }

     function setAccount(data) {
      return { type: 'SET_Account', data: data }
     }
     ```

17.  ### Redux store에 모든 컴포넌트의 state를 유지해야 하나?

      Redux store에 데이터를 유지하고, 컴포넌트 내부에 UI 관련 state를 유지하면 된다.

18.  ### Redux store에 접근하는 올바른 방법은?

     컴포넌트에서 store에 접근하는 가장 좋은 방법은 `connect()` 함수를 사용하여 기존 컴포넌트를 감싸는 새로운 컴포넌트를 만드는 것이다. 이러한 패턴을 *Higher-Order Components* 라고 하며, 일반적으로 React에서 컴포넌트의 기능을 확장하는데 선호되는 방법이다. 이를 통해 state 및 action 생성자를 컴포넌트에 매핑하고 store 업데이트 시 자동으로 전달할 수 있다.

     connect를 사용한 `<FilterLink>` 컴포넌트 예시를 보자.

     ```javascript
     import { connect } from 'react-redux'
     import { setVisibilityFilter } from '../actions'
     import Link from '../components/Link'

     const mapStateToProps = (state, ownProps) => ({
       active: ownProps.filter === state.visibilityFilter
     })

     const mapDispatchToProps = (dispatch, ownProps) => ({
       onClick: () => dispatch(setVisibilityFilter(ownProps.filter))
     })

     const FilterLink = connect(
       mapStateToProps,
       mapDispatchToProps
     )(Link)

     export default FilterLink
     ```

     성능 최적화가 상당히 적고 일반적으로 버그가 발생할 가능성이 작기 때문에 Redux 개발자는 항상 Context API를 사용하여 저장소에 접근하는 것보다는 `connect()` 를 사용하는 것이 좋다.

     ```javascript
     class MyComponent {
       someMethod() {
         doSomethingWith(this.context.store)
       }
     }
     ```

19.  ### React Redux에서 컴포넌트와 컨테이너의 차이점은?

     **Component** 는 애플리케이션의 presentational 부분을 묘사하는 클래스 또는 함수형 컴포넌트이다.

     **Container** 는 Redux store에 연결된 컴포넌트에 대한 비공식 용어이다. 컨테이너는 Redux state 업데이트 및 *dispatch* action을 구독하며 일반적으로 DOM 요소를 렌더링하지 않는다. 그들은 presentational 자식 컴포넌트에 렌더링을 위임한다.

20.  ### Redux에서 상수의 목적은 무엇인가?

     상수를 사용하면 IDE를 사용할 때 프로젝트 전체에서 특정 기능의 모든 사용법을 쉽게 찾을 수 있다. 오타같은 경우 `ReferenceError` 를 던져주어 버그 발생을 사전에 방지한다.

     보통 하나의 파일로 저장한다 (`constants.js` 또는 `actionTypes.js`).

     ```javascript
     export const ADD_TODO = 'ADD_TODO'
     export const DELETE_TODO = 'DELETE_TODO'
     export const EDIT_TODO = 'EDIT_TODO'
     export const COMPLETE_TODO = 'COMPLETE_TODO'
     export const COMPLETE_ALL = 'COMPLETE_ALL'
     export const CLEAR_COMPLETED = 'CLEAR_COMPLETED'
     ```

     Redux에서는 두 곳에서 사용한다.

     1. **action을 작성할 때**

         `actions.js` 을 보자.

         ```javascript
         import { ADD_TODO } from './actionTypes';

         export function addTodo(text) {
           return { type: ADD_TODO, text }
         }
         ```

     2. **reducer 안에서**

         `reducer.js` 를 만들어 보자.

         ```javascript
         import { ADD_TODO } from './actionTypes'

         export default (state = [], action) => {
           switch (action.type) {
             case ADD_TODO:
               return [
                 ...state,
                 {
                   text: action.text,
                   completed: false
                 }
               ];
             default:
               return state
           }
         }
         ```

21.  ### `mapDispatchToProps()`를 작성하는 다른 방법은?

    `mapDispatchToProps()`에서 *action creators*를 `dispatch()`에 바인딩하는 몇 가지 방법이 있다. 가능한 옵션은 아래와 같다.

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: () => dispatch(action())
     })
     ```

     ```javascript
     const mapDispatchToProps = (dispatch) => ({
      action: bindActionCreators(action, dispatch)
     })
     ```

     ```javascript
     const mapDispatchToProps = { action }
     ```

    세 번째 옵션은 첫 번째 옵션의 약어이다.

22.  ### `mapStateToProps()` 과 `mapDispatchToProps()` 에서 `ownProps` 매개 변수를 사용하는 방법은?

     `ownProps` 매개 변수가 지정되면, React Redux는 컴포넌트에 전달된 props를 *connect* 함수로 전달한다. 따라서, 연결된 컴포넌트를 사용하는 경우,

     ```jsx harmony
     import ConnectedComponent from './containers/ConnectedComponent';

     <ConnectedComponent user={'john'} />
     ```

     `mapStateToProps()`과 `mapDispatchToProps()` 함수 내에서 `ownProps` 는 객체가 된다.

     ```javascript
     { user: 'john' }
     ```

     이 객체를 사용하여 해당 함수에서 무엇을 반환할지 결정할 수 있다.

23.  ### Redux 최상위 디렉토리를 구성하는 방법은?

     대부분의 응용 프로그램에는 아래와 같은 여러 최상위 디렉터리가 있다.

     1. **Components**: Redux를 인식하지 못하는 *dumb* 컴포넌트에 사용된다.
     2. **Containers**: Redux에 연결된 *smart*  컴포넌트에 사용된다.
     3. **Actions**: 모든 action creator에 사용되며, 파일 이름이 앱의 일부이다. 
     4. **Reducers**: 모든 reducer에 사용되며, 파일 이름은 state 키이다.
     5. **Store**: store 초기화에 사용된다.

     이 구조는 중소규모의 앱에 적합하다.

24.  ### redux-saga란?

     `redux-saga`는 React/Redux 애플리케이션에서 side-effect(데이터 가져오기 같은 비동기식 및 브라우저 캐시 접근과 같이 불쾌한 것)를 더욱 쉽고 효과적으로 처리하는 것을 목표로 하는 라이브러리이다.

     NPM에서 사용 가능하다.

     ```console
     $ npm install --save redux-saga
     ```

25.  ### redux-saga의 정신 모델은?

     *Saga* 는 응용 프로그램에서 별도의 thread와 유사하며, side-effect 의 주된 원인이다. `redux-saga` 는 redux *middleware*로, 이 thread는 일반적인 Redux action으로 메인 응용 프로그램에서 시작, 일시 중지 및 취소 할 수 있으며, 전체 Redux 응용 프로그램 state에 접근할 수 있으며, Redux action도 전달할 수 있다.

26.  ### redux-saga에서 `call()`과 `put()`의 차이점은?

     `call()`과 `put()` 둘 다 effect 생성함수이다. `call()` 함수는 effect 설명을 작성하는 데 사용되며 미들웨어가 promise를 호출하도록 한다. `put()` 함수는 effect를 작성하여 미들웨어가 action을 store에 전달하도록 해준다.

     특정 사용자 데이터를 가져오는데 effect가 어떻게 작동하는지 예를 들어보자.

     ```javascript
     function* fetchUserSaga(action) {
       // `call` function accepts rest arguments, which will be passed to `api.fetchUser` function.
       // Instructing middleware to call promise, it resolved value will be assigned to `userData` variable
       const userData = yield call(api.fetchUser, action.userId)

       // Instructing middleware to dispatch corresponding action.
       yield put({
         type: 'FETCH_USER_SUCCESS',
         userData
       })
     }
     ```

27.  ### Redux Thunk란?

     *Redux Thunk* 미들웨어는 action 대신 함수를 리턴하는 action 생성자를 작성하도록 해준다. thunk는 action의 dispatch를 지연시키거나 특정한 조건을 만족한 경우 dispatch 해야 하는 곳에 사용된다. 내부 함수는 store 메서드 `dispatch()`와 `getState()`를 매개변수로 받는다.

28.  ### `redux-saga`와 `redux-thunk`의 차이점은?

     *Redux Thunk*와 *Redux Saga*는 side effects를 처리한다. 대부분의 시나리오에서 Thunk는 *Promises*를 사용하여 처리하고 Saga는 *Generators*를 사용한다. Thunk는 사용하기 쉽고 Promises는 많은 개발자에게 친숙하다. Sagas/Generators는 더 강력하지만, 학습을 할 필요가 있다. 그러나 두 미들웨어는 공존할 수 있어서 필요할 때 Thunks로 시작하고 필요할 때 Sagas를 소개할 수 있다.

29.  ### Redux DevTools이란?

     *Redux DevTools*는 핫 리로딩, action 리플레이 및 사용자 정의 UI 가능한 UI가 있는 Redux의 실시간 편집하는 시간 여행 환경이다. Redux DevTools 설치 와 프로젝트 통합을 방해하지 않으려면, Chrome 및 Firefox 용 Redux DevTools Extension 사용을 고려해야 한다.

30.  ### Redux DevTools의 기능에는 무엇이 있나?

     1. 모든 state와 action payload를 검사할 수 있다.
     2. action을 *취소하여* 시간을 되돌릴 수 있다.
     3. reducer 코드를 변경하면, 각 *단계별* action이 다시 평가된다.
     4. reducers가 throw되면, 어떤 action이 발생했는지와 오류가 무엇인지 알 수 있다.
     5. `persistState()` store enhancer를 사용하게 되면, 페이지를 다시 로드해도 디버그 세션을 유지할 수 있다.

31.  ### Redux selectors가 무엇이며 사용해야하는 이유는?

     *Selectors*는 Redux state를 인수로 사용하며 일부 데이터를 component에 전달하는 함수이다.

     예를 들어, state에서 사용자 세부 사항을 얻으려면 아래와 같이 하면 된다.

     ```javascript
     const getUserData = state => state.user.data
     ```

32.  ### Redux Form이란?

     *Redux Form*은 React 및 Redux와 함께 작동하며 React의 양식에서 Redux를 사용하여 모든 state를 저장할 수 있다. Redux Form은 원시 HTML5 입력과 함께 사용할 수 있으며, Material UI, React Widgets 및 React Bootstrap과 같은 일반적인 UI 프레임워크와도 잘 작동한다.

33.  ### Redux Form의 주요 기능은?

       1. Redux store를 통한 필드 값 지속.
       2. 유효성 검사 (sync/async) 및 제출.
       3. 필드 값의 형식화, parsing 및 표준화.

34.  ### Redux에 여러 미들웨어를 추가하는 방법은?

     `applyMiddleware()`를 사용할 수 있다.

     예를 들어, `redux-thunk`와 `logger`를 추가하여 `applyMiddleware()`에 인수로 전달할 수 있다.

     ```javascript
     import { createStore, applyMiddleware } from 'redux'
     const createStoreWithMiddleware = applyMiddleware(ReduxThunk, logger)(createStore)
     ```

35.  ### Redux에서 초기 state를 설정하는 방법은?

     createStore에 두번째 인자로 초기 state를 전달해야한다.

     ```javascript
     const rootReducer = combineReducers({
       todos: todos,
       visibilityFilter: visibilityFilter
     })

     const initialState = {
       todos: [{ id: 123, name: 'example', completed: false }]
     }

     const store = createStore(
       rootReducer,
       initialState
     )
     ```

36.  ### Relay와 Redux의 차이점은?

     Relay와 Redux는 둘 다 단일 저장소를 사용한다는 점에서 유사하다. 가장 큰 차이점은 relay는 서버에서 시작된 state만 관리하고 상태에 대한 모든 접근을 *GraphQL* queries(데이터 읽기) 및 mutations(데이터 변경)를 통해서 한다. Relay는 데이터를 캐시하고 변경된 데이터만 가져오고 더 이상 가져오지 않기 때문에 데이터 가져오기를 최적화할 수 있다.

## React Native

1.   ### What is the difference between React Native and React?

     **React** is a JavaScript library, supporting both front end web and being run on the server, for building user interfaces and web applications.

     **React Native** is a mobile framework that compiles to native app components, allowing you to build native mobile applications (iOS, Android, and Windows) in JavaScript that allows you to use React to build your components, and implements React under the hood.

2.   ### How to test React Native apps?

     React Native can be tested only in mobile simulators like iOS and Android. You can run the app in your mobile using expo app (https://expo.io) Where it syncs using QR code, your mobile and computer should be in same wireless network.

3.   ### How to do logging in React Native?

     You can use `console.log`, `console.warn`, etc. As of React Native v0.29 you can simply run the following to see logs in the console:

     ```
     $ react-native log-ios
     $ react-native log-android
     ```

4.   ### How to debug your React Native?

     Follow the below steps to debug React Native app:

     1. Run your application in the iOS simulator.
     2. Press `Command + D` and a webpage should open up at `http://localhost:8081/debugger-ui`.
     3. Enable *Pause On Caught Exceptions* for a better debugging experience.
     4. Press `Command + Option + I` to open the Chrome Developer tools, or open it via `View` -> `Developer` -> `Developer Tools`.
     5. You should now be able to debug as you normally would.

## React supported libraries & Integration

192. ### reselect이란 무엇이며 어떻게 작동하나?

     *Reselect*는 *메모이제이션* 개념을 사용하는 **selector library** (Redux 용)이다. 원래 Redux와 같은 애플리케이션 state에서 파생된 데이터를 계산하기 위해 작성되었지만, 아키텍쳐나 라이브러리에는 연결할 수 없다.

     Reselect은 마지막 호출의 마지막 입/출력 사본을 유지하고, 입력 중 하나가 변경된 경우에만 결과를 다시 계산한다. 동일한 입력이 동시에 두 번 제공되면, Reselect는 캐시된 출력을 반환한다. 메모 및 캐시는 완전히 사용자 정의할 수 있다.

193. ### Flow란?

     *Flow*는 JavaScript에서 타입 오류를 잡아내기 위해 설계된 *정적 타입 검사기* 이다. Flow 타입은 기존 타입 시스템보다 훨씬 세밀한 차이를 표현할 수 있다. 예를 들어, Flow는 대부분의 타입 시스템과 달리 `null`과 관련된 오류를 찾아내는 데 도움이 된다.

194. ### Flow와 PropTypes의 차이점은?

     Flow는 언어의 상위 집합을 사용하는 *정적 분석 도구* (정적 검사기)로, 모든 코드에 타입 어노테이션을 추가하여 컴파일 타임에 전체 버그 클래스를 잡을 수 있다. PropTypes은 React에 패치된 *기본 타입 검사기* (런타임 검사기)이다. 주어진 컴포넌트에 전달되는 props 타입 이외의 것은 확인할 수 없다. 전체 프로젝트에 유연한 타입검사를 원할 경우 Flow / TypeScript가 적합하다.

195. ### React에서 Font Awesome icons를 어떻게 사용하나?

     아래의 예제는 React에 Font Awesome을 포함시키는 것이다.

     1. `font-awesome` 설치한다.

     ```console
     $ npm install --save font-awesome
     ```

     1. `index.js` 파일에 `font-awesome` Import한다.

     ```javascript
     import 'font-awesome/css/font-awesome.min.css'
     ```

     1. `className`에 Font Awesome 클래스를 추가한다.

     ```javascript
     render() {
       return <div><i className={'fa fa-spinner'} /></div>
     }
     ```

196. ### React Dev Tools이란?

     *React Developer Tools* 를 사용하면 컴포넌트 props와 state를 포함한 컴포넌트 계층을 검사할 수 있다. 브라우저 확장 (Chrome과 Firefox 용), 독립실행형 앱(Safari, IE, 와 React Native 등의 다른 환경에서 작동하는)으로 있다. 

     다른 브라우저 또는 환경에서 사용 가능한 공식 확장
     1. **Chrome extension**
     2. **Firefox extension**
     3. **Standalone app** (Safari, React Native, etc)

197. ### 로컬 파일을 연 Chrome에서 DevTools이 로딩되지 않는 이유는?

     브라우저에서 로컬 HTML 파일(`file://...`)을 연 경우 먼저 *Chrome Extensions*을 열고 `Allow access to file URLs`을 선택해야 한다.

198. ### React에서 Polymer를 사용하는 방법은?

     1. Polymer 엘리먼트를 만든다.

         ```jsx harmony
         <link rel='import' href='../../bower_components/polymer/polymer.html' />
         Polymer({
           is: 'calender-element',
           ready: function() {
             this.textContent = 'I am a calender'
           }
         })
         ```

     2. Polymer 컴포넌트 HTML 태그를 HTML 문서로 가져와서 만든다. (예 : React 애플리케이션의 `index.html`로 가져오십시오.)

         ```html
         <link rel='import' href='./src/polymer-components/calender-element.html'>
         ```

         1. JSX 파일에서 해당 엘리먼트를 사용한다.

         ```javascript
         import React from 'react'

         class MyComponent extends React.Component {
           render() {
             return (
               <calender-element />
             )
           }
         }

         export default MyComponent
         ```

199. ### Vue.js보다 React의 장점은 무엇인가?

     React가 Vue.js에 비해 아래와 같은 장점이 있다.

     1. 대규모 앱 개발에 있어서 더 많은 유연성을 제공한다.
     2. 테스트하기 쉽다.
     3. 모바일 앱 제작에 적합하다.
     4. 더 많은 정보와 유용한 솔루션을 가지고 있다.

200. ### React와 Angular의 차이점은?

     | React | Angular |
     | ----- | ------- |
     | React는 라이브러리이며 View 단만 있다. | Angular는 프레임워크이며 완전한 MVC 기능이 있다. |
     | React는 서버 측에서 렌더링할 수 있다. | AngularJS는 클라이언트 측에서만 렌더링 되지만 Angular 2 이상에서 서버 측에서 렌더링이 된다. |
     | React는 혼란스러울 수 있는 JS를 HTML처럼 보이는 JSX를 사용한다. | Angular는 HTML에 대한 템플릿 접근 방식을 따르므로 코드가 더 짧고 이해하기 쉽다. |
     | 모바일 애플리케이션을 빌드하기 위한 React 유형인 React Native는 더 빠르고 안정적이다. | Ionic, Angular의 모바일 네이티브 앱은 상대적으로 덜 안정적이며 느리다. |
     | React에서 데이터는 한 방향으로만 흐르므로 디버깅이 쉽다. | Angular에서는 데이터가 양방향으로 흐른다. 즉 자식과 부모 사이에 양방향 데이터 바인딩이 있음으로 디버깅이 어려운 경우가 많다. |

201. ### DevTools에 React 탭이 표시되지 않는 이유는?

     페이지가 로딩되면, *React DevTools*가 `__REACT_DEVTOOLS_GLOBAL_HOOK__`이라는 전역을 설정한 후 초기화 중에 React가 해당 hook과 통신한다.  웹사이트가 React를 사용하지 않거나 React가 DevTool과 통신하지 못하면 탭이 표시되지 않는다.

202. ### Styled Components란?

     `styled-components`는 React 애플리케이션 스타일링을 위한 JavaScript 라이브러리이다. 스타일과 컴포넌트 간의 매핑을 제거하고 JavaScript로 보강된 실제 CSS를 작성할 수 있다.

203. ### Styled Components의 예시는?

     각각에 대해 특정 스타일로 `<Title>`과 `<Wrapper>` 컴포넌트를 만들어 보자.

     ```javascript
     import React from 'react'
     import styled from 'styled-components'

     // Create a <Title> component that renders an <h1> which is centered, red and sized at 1.5em
     const Title = styled.h1`
       font-size: 1.5em;
       text-align: center;
       color: palevioletred;
     `

     // Create a <Wrapper> component that renders a <section> with some padding and a papayawhip background
     const Wrapper = styled.section`
       padding: 4em;
       background: papayawhip;
     `
     ```

     `Title`과 `Wrapper`는 이제 서로 다른 react component처럼 렌더링 할 수 있는 컴포넌트이다.

     ```jsx harmony
     <Wrapper>
       <Title>{'Lets start first styled component!'}</Title>
     </Wrapper>
     ```

204. ### Relay란?

     Relay는 React View 계층을 사용하여 웹 애플리케이션에 데이터 계층과 클라이언트-서버 통신을 제공하기 위한 JavaScript 프레임워크이다.

205. ### `create-react-app` 애플리케이션에서 TypeScript를 사용하는 방법?
     
     react-scripts@2.1.0 이상부터, typescript를 기본적으로 지원한다. 아래와 같이 `--typescript` 옵션을 전달할 수 있다.

     ```bash
     npx create-react-app my-app --typescript

     # or

     yarn create react-app my-app --typescript
     ```
     
     그러나 더 낮은 버전의 react scripts의 경우 새 프로젝트를 만드는 동안 `--scripts-version` 옵션을 `react-scripts-ts`로 제공하여라. `react-scripts-ts`는 표준 `create-react-app` 프로젝트 파이프라인을 취하고 TypeScript를 믹스로 가져오기 위한 조정 세트이다.

     이제 프로젝트 레이아웃은 다음과 같아야 한다.

     ```
     my-app/
     ├─ .gitignore
     ├─ images.d.ts
     ├─ node_modules/
     ├─ public/
     ├─ src/
     │  └─ ...
     ├─ package.json
     ├─ tsconfig.json
     ├─ tsconfig.prod.json
     ├─ tsconfig.test.json
     └─ tslint.json
     ```

## Miscellaneous

1.   ### Reselect 라이브러리의 주요 기능은?

       1. Selectors는 파생된 데이터를 계산하여, Redux가 가능한 최소의 state를 저장할 수 있도록 한다.
       2. Selectors는 효율적이다. selector는 인자 중 하나도 변화가 없다면 재계산을 하지 않는다.
       3. Selectors는 composable하다. 다른 selector에 대한 입력으로 사용할 수 있다.

2.   #### Reselect 사용법에 대한 예시는?

     Reselect의 간단한 사용법으로는 다른 수량의 선적 주문을 계산해보자.

     ```javascript
     import { createSelector } from 'reselect'

     const shopItemsSelector = state => state.shop.items
     const taxPercentSelector = state => state.shop.taxPercent

     const subtotalSelector = createSelector(
       shopItemsSelector,
       items => items.reduce((acc, item) => acc + item.value, 0)
     )

     const taxSelector = createSelector(
       subtotalSelector,
       taxPercentSelector,
       (subtotal, taxPercent) => subtotal * (taxPercent / 100)
     )

     export const totalSelector = createSelector(
       subtotalSelector,
       taxSelector,
       (subtotal, tax) => ({ total: subtotal + tax })
     )

     let exampleState = {
       shop: {
         taxPercent: 8,
         items: [
           { name: 'apple', value: 1.20 },
           { name: 'orange', value: 0.95 },
         ]
       }
     }

     console.log(subtotalSelector(exampleState)) // 2.15
     console.log(taxSelector(exampleState))      // 0.172
     console.log(totalSelector(exampleState))    // { total: 2.322 }
     ```

3.   ### Redux에서 action이란?

     *Actions*은 응용프로그램에서 store로 데이터를 보내는 일반 JavaScript 객체나 정보의 payload이다. 이것들은 store에 대한 유일한 정보 소스이다. Actions에는 수행 중인 action 유형을 나타내는 type 속성이 있어야 한다.

     새로운 할 일 항목 추가를 나타내는 동작에 대한 예시이다.

     ```
     {
       type: ADD_TODO,
       text: 'Add todo item'
     }
     ```

4.   ### React의 ES6 클래스는 static object와 함께 사용 가능한가?

     안된다, `statics`은 `React.createClass()`에서만 작동한다.

     ```javascript
     someComponent= React.createClass({
       statics: {
         someMethod: function() {
           // ..
         }
       }
     })
     ```

     그러나 ES6+ classes 안에서 static을 사용하거나 아래와 같이 클래스 외부에서 작성할 수 있다.

     ```javascript
     class Component extends React.Component {
       static propTypes = {
         // ...
       }

       static someMethod() {
         // ...
       }
     }
     ```
     ```javascript
     class Component extends React.Component {
        ....
     }

     Component.propTypes = {...}
     Component.someMethod = function(){....}
     ```

5.   ### Redux는 React에서만 사용 가능한가?

     Redux는 모든 UI 계층의 데이터 저장소로 사용할 수 있다. 주 사용처는 React와 React Native이지만, Angular, Angular 2, Vue, Mithril 등에서 사용할 수 있다. Redux는 다른 코드에서 사용할 수 있는 subscription 메커니즘을 제공한다.

6.   ### Redux를 사용하기 위한 특별한 빌드 도구가 필요한가?

     Redux는 ES6로 작성되었으며 Webpack과 Babel을 사용하여 ES5로 변환되어있다. JavaScript 빌드 프로세스에 관련 없이 사용할 수 있어야 한다. 또한 Redux는 빌드 프로세스 없이 직접 사용할 수 있는 UMD 빌드를 제공한다.

7.   ### Redux Form `initialValues`는 state에서 어떻게 업데이트하나?

     `enableReinitialize : true` 설정을 추가해야 한다.

     ```javascript
     const InitializeFromStateForm = reduxForm({
       form: 'initializeFromState',
       enableReinitialize : true
     })(UserEdit)
     ```

     `initialValues` prop가 업데이트되면, form도 업데이트된다.

8.   ### React PropTypes이 하나의 prop에서 다른 타입들을 허용하는 방법은?

     `PropTypes`의 `oneOfType()` 메소드를 사용할 수 있다.

     예를 들어, height 속성은 아래와 같이 `string` 또는 `number` 타입으로 정의될 수 있다.

     ```javascript
     Component.PropTypes = {
       size: PropTypes.oneOfType([
         PropTypes.string,
         PropTypes.number
       ])
     }
     ```

9.   ### SVG file을 react 컴포넌트로 가져올 수 있나?

     SVG를 파일로 로드하는 대신에 컴포넌트로 직접 가져올 수 있다. 해당 기능은 `react-scripts@2.0.0` 또는 그 이상에서 사용 가능하다.

     ```jsx harmony
     import { ReactComponent as Logo } from './logo.svg'

     const App = () => (
       <div>
         {/* Logo is an actual react component */}
         <Logo />
       </div>
     )
     ```

     **Note**: import에서 중괄호를 잊어서는 안된다.

10.  ### 인라인 ref 콜백 또는 함수를 권장하지 않는 이유는?

     ref 콜백이 인라인 함수로 정의된 경우 업데이트 중에 두 번 호출된다. (먼저 null로, DOM 요소로 다시 호출됨)
    렌더링마다 함수의 새 인스턴스가 생성되므로 React는 이전 참조를 지우고 새 참조를 설정해야 하기 때문이다.

     ```jsx
     class UserForm extends Component {
       handleSubmit = () => {
         console.log("Input Value is: ", this.input.value)
       }


       render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={(input) => this.input = input} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

    그러나 컴포넌트가 마운트될 때 ref 콜백이 한 번 호출되기를 기대한다. 빠른 수정은 ES7 클래스 구문을 사용하여 함수를 정의하는 것이다.

     ```jsx
     class UserForm extends Component {
      handleSubmit = () => {
        console.log("Input Value is: ", this.input.value)
      }

      setSearchInput = (input) => {
        this.input = input
      }

      render () {
        return (
          <form onSubmit={this.handleSubmit}>
            <input
              type='text'
              ref={this.setSearchInput} /> // Access DOM input in handle submit
            <button type='submit'>Submit</button>
          </form>
        )
      }
     }
     ```

11.  ### react에서 render hijacking이란?

     render hijacking의 개념은 컴포넌트가 다른 컴포넌트에서 출력할 내용을 제어하는 기능이다. 실제로 컴포넌트를 Higher-Order component로 감싸서 나타낸다. 감싸게 되면 추가 props 주입하거나 다른 변경사항을 수행하여 렌더링 논리가 변경될 수 있다. 실제로 hijacking을 사용하지 않지만 HOC를 사용하면 컴포넌트가 다른 방식으로 동작하게 된다.

12.  ### HOC 팩토리 구현이란?
     
     React에서 HOC을 구현하는 방법은 크게 2가지이다. 1. Props Proxy (PP)와 2. Inheritance Inversion (II). *WrappedComponent*를 조작하기 위한 다양한 접근법이 있다.

     **Props Proxy**

     이 접근법에서 HOC render 메서드는 WrappedComponent 타입의 React Element를 반환한다. 우리는 HOC가 받은 props를 전달하므로, **Props Proxy**라고 불린다.

     ```jsx

     function ppHOC(WrappedComponent) {
      return class PP extends React.Component {
        render() {
          return <WrappedComponent {...this.props}/>
        }
      }
     }
     ```
     **Inheritance Inversion**

     이 접근법에서 반환된 HOC 클래스(Enhancer)가 WrappedComponent를 확장한다. 일부 Enhancer 클래스를 확장하는 WrappedComponent 대신 Enhancer에 의해 수동으로 확장되므로 Inheritance Inversion이라고 불린다. 이러한 방식을 통해 그들 사이의 관계는 **inverse**해진다.

     ```jsx
     function iiHOC(WrappedComponent) {
      return class Enhancer extends WrappedComponent {
        render() {
          return super.render()
        }
      }
     }
     ```
13.  ### React 컴포넌트에 숫자를 전달하는 방법은?

     중괄호({})를 통해서 숫자를 전달해야 한다. 여기서 문자열은 따옴표로 묶는다.

     ```jsx
        React.render(<User age={30} department={"IT"} />, document.getElementById('container'));
     ```
14.  ### 모든 state를 Redux에서 관리를 해야 하나? react 내부 state를 사용해야 하나?
     
     개발자의 결정에 달려있다. 즉 응용 프로그램을 구성하는 state의 종류와 각 state의 위치를 결정하는 것은 개발자의 작업이다. 일부 사용자는 애플리케이션의 직렬화 및 제어 가능한 버전을 유지하기 위해 Redux로 모든 단일 데이터를 유지하는 것을 선호한다. 다른 사람들은 컴포넌트의 내부 state를 “이 드롭다운이 현재 열려있습니까”와 같이 중요하지 않거나 UI state를 유지하는 것을 선호한다.

     아래는 어떤 종류의 데이터를 Redux에 넣어야 하는지 결정하는 규칙이다.
     1. 응용 프로그램의 다른 부분이 데이터를 관리하나?
     2. 원본 데이터를 기반으로 추가 파생 데이터를 작성할 수 있어야 하나?
     3. 여러 컴포넌트를 구동하는데 동일한 데이터가 사용되나?
     4. 이 state를 주어진 시점 (즉, 시간여행 디버깅)으로 복원할 수 있는 가치가 있나?
     5. 데이터를 캐시 하고 싶은가(예 : 데이터를 다시 요청하는 대신 state가 있는 경우 사용하나)?

15.  ### React에서 registerServiceWorker의 목적은?

     React는 기본적으로 별다른 구성없이 service worker를 생성할 수 있다. service worker는 자산 및 기타 파일을 캐싱하여 사용자가 오프라인 상태이거나 네트워크 속도가 느린 경우에도 화면을 볼 수 있도록 해주는 웹 API이다. 이는 더 나은 사용자 경험을 구축하는데 도움이된다. 사이트에 오프라인 기능을 추가할 수 있다.

     ```jsx
        import React from 'react';
        import ReactDOM from 'react-dom';
        import App from './App';
        import registerServiceWorker from './registerServiceWorker';

        ReactDOM.render(<App />, document.getElementById('root'));
        registerServiceWorker();
     ```
16.  ### React의 memo 함수란?

      **PureComponent 또는 shouldComponentUpdate** 사용시 입력 props가 동일하다면, 클래스 컴포넌트의 렌더링이 제한될 수 있다. 이제는 함수형 컴포넌트를 **React.memo**로 감싸서 동일한 기능을 수행할 수 있다.
     ```jsx
     const MyComponent = React.memo(function MyComponent(props) {
      /* only rerenders if props change */
     });
     ```
17.  ### React의 lazy function란?
     React.lazy 함수를 사용하면 dynamic import로 일반 컴포넌트를 렌더링할 수 있다. 컴포넌트가 렌더링 될 때 OtherComponent를 포함한 번들을 자동으로 로드한다. React 컴포넌트를 포함한 기본 내보내기가 있는 모듈로 해석되는 Promise를 리턴해야한다.
     ```jsx
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
      return (
        <div>
          <OtherComponent />
        </div>
      );
     }
     ```
     **Note:**
     React.lazy 및 Suspense는 아직 server-side 렌더링에 사용할 수 없다. 서버 렌더링 앱에서 code-splitting을 수행하려는 경우 여전히 React Loadable이 권장된다.

18.  ### setState를 사용하는데 있어 불필요한 업데이트를 방지하는 방법은?
     state의 현재 값과 기존의 값을 비교하여 리렌더링을 할지 말지 결정할 수 있다. 값이 같다면 **null**을 반환하여 리렌더링을 멈추고 그렇지 않으면 최신의 state 값을 반환한다. 예를 들어, 사용자 프로필 정보는 아래와 같이 조건부로 렌더링이 이루어진다.
     ```jsx
     getUserProfile = user => {
       const latestAddress = user.address;
       this.setState(state => {
         if (state.address === latestAddress) {
           return null;
         } else {
           return { title: latestAddress };
         }
       });
     };
     ```
19.  ### React 16버전에서 Array, Strings와 Numbers를 렌더링하는 방법은?
     **Arrays**: 이전 릴리즈와 다르게, React 16에서 **render** 메서드가 단일 엘리먼트를 반환할 필요는 없다. 배열을 반환함으로써 별도의 묶어주는 엘리먼트 없이 여러 형제 요소를 반환할 수 있다. 예를 들어, 아래의 개발자 목록을 보자.
     ```jsx
     const ReactJSDevs = () => {
       return [
         <li key="1">John</li>,
         <li key="2">Jackie</li>,
         <li key="3">Jordan</li>
       ];
     }
     ```
     배열을 다른 배열 컴포넌트에 병합할 수 있다.
     ```jsx
     const JSDevs = () => {
       return (
         <ul>
           <li>Brad</li>
           <li>Brodge</li>
           <ReactJSDevs/>
           <li>Brandon</li>
         </ul>
       );
     }
     ```
     **Strings과 Numbers:** render 메서드에서 문자열과 숫자 타입을 반환할 수 있다.
     ```jsx
     render() {
      return 'Welcome to ReactJS questions';
     }
     // Number
     render() {
      return 2018;
     }
     ```
20.  ### React 클래스에서 클래스 필드 선언 구문을 사용하는 방법은?
     클래스 선언문을 사용하여 React Class 컴포넌트를 훨씬 간결하게 만들 수 있다. 생성자를 사용하지 않고 지역 state를 초기화할 수 있으며, 별도의 바인딩 없이 화살표 함수를 사용해서 클래스 메서드를 선언할 수 있다. 바인딩 없는 생성자와 메서드를 사용하지 않고 state에 대한 클래스 필드 선언을 보여주는 카운터 예제를 보자.
     ```jsx
     class Counter extends Component {
       state = { value: 0 };

       handleIncrement = () => {
         this.setState(prevState => ({
           value: prevState.value + 1
         }));
       };

       handleDecrement = () => {
         this.setState(prevState => ({
           value: prevState.value - 1
         }));
       };

       render() {
         return (
           <div>
             {this.state.value}

             <button onClick={this.handleIncrement}>+</button>
             <button onClick={this.handleDecrement}>-</button>
           </div>
         )
       }
     }
     ```
21.  ### hooks이란?
     Hooks란 클래스를 작성하지 않고도 state와 다른 React 기능을 사용할 수 있는 새로운 기능이다. useState hook 예제를 살펴보자.
     ```jsx
     import { useState } from 'react';

     function Example() {
       // 새로운 state 변수를 선언하며, "count"라고 불린다.
       const [count, setCount] = useState(0);

       return (
         <div>
           <p>You clicked {count} times</p>
           <button onClick={() => setCount(count + 1)}>
             Click me
           </button>
         </div>
       );
     }
     ```
22.  ### hooks를 위해서 지켜야 하는 규칙은 무엇인가?

     hooks를 사용하기 위해서 2가지 규칙을 따라야한다.
     1. react 함수의 최상위에서만 Hooks를 호출한다. 예로, 반복문, 조건문 또는 중첩 함수내에서 Hooks를 호출하면 안 된다. 이렇게 하면 컴포넌트가 렌더링 될 때마다 Hooks가 동일한 순서로 호출되고, 여러 useState 및 useEffect 호출간에 Hooks state가 보장된다.
     2. Hooks는 React 함수에서만 호출한다. 예로, 일반적인 JavaScript 함수에서 Hooks를 호출하면 안 된다.

23.  ### hooks가 프로젝트의 규칙을 준수하도록 하는 방법은?
     React 팀은 두가지 규칙을 적용하는 **eslint-plugin-react-hooks**라는 ESLint 플러그인을 출시했다. 아래의 명령을 사용하여 플러그인을 프로젝트에 추가할 수 있다.
     ```javascript
     npm install eslint-plugin-react-hooks@next
     ```
     ESLint config 파일에 아래 구성을 적용한다.
     ```javascript
     // Your ESLint configuration
     {
       "plugins": [
         // ...
         "react-hooks"
       ],
       "rules": {
         // ...
         "react-hooks/rules-of-hooks": "error"
       }
     }
     ```
     **Note:** 이 플러그인은 Create React App에서 기본값으로 사용하도록 설계되어있다.

24.  ### Flux와 Redux의 차이점은?
     아래에 Flux와 Redux의 주요한 차이점이 있다.

     | Flux | Redux |
     | ----- | ------- |
     | State는 변한다. | State은 불변하다. |
     | Store는 state와 변경로직을 포함한다. | Store와 변경로직은 분리되어있다. |
     | 멀티 store가 있다. | 하나의 store만 있다. |
     | 모든 stores는 연결이 끊어지고 평평하다. | 수직적 reducer가 있는 단일 store이다. |
     | 싱글톤 dispatcher가 있다. | dispatcher 개념이 없다. |
     | React 컴포넌트는 store를 구독한다. | Container 컴포넌트는 connect 함수를 사용한다. |
25.  ### React Router V4의 장점은?
     다음은 React Router V4 모듈의 주요 장점이다.
     1. React Router v4(version 4)에서 API는 컴포넌트와 관련된 것이다. 라우터는 특정 하위 라우터 컴포넌트(`<Route>`)를 감싸는 단인 컴포넌트(`<BrowserRouter>`)로 시각화할 수 있다.
     2. history를 수동으로 설정할 필요 없다. 라우터 모듈을 `<BrowserRouter>` 컴포넌트로 경로를 줄임으로써 history를 관리한다.
     3. 특정 라우터 모듈(웹, 코어 또는 기본)만 추가하여 응용프로그램 크기가 줄었다.
26.  ### componentDidCatch 생명주기 메서드에 대해서 설명할 수 있나?
     **componentDidCatch** 생명주기 메서드는 하위 컴포넌트에서 오류가 발생하면 호출된다. 이 메서드는 2개의 매개변수를 받는다.

     1. error: - 보내진 에러 객체
     2. info: - 오류를 발생시킨 컴포넌트에 대한 정보를 포함한 componentStack key가 있는 객체

     메서드의 구조는 아래와 같다.
     ```javascript
     componentDidCatch(error, info)
     ```
27.  ### 어떤 에러 바운더리(error boundary)에서 잡지 못할까?
     아래의 경우는 오류 경계가 작동하지 않는 경우이다.
     1. Event handlers 안쪽일 경우
     2. **setTimeout이나 requestAnimationFrame** 콜백을 사용하는 비동기 코드
     3. Server side rendering을 할 경우
     4. 오류 경계 코드 자체에서 오류가 발생한 경우
28.  ### 이벤트 핸들러에 에러 바운더리가 필요하지 않은 이유는?
     에러 바운더리는 이벤트 핸들러내에서 오류를 잡아내지 못한다. 렌더링 메서드나 라이프 사이클 메서드와 다르게 이벤트 핸들러는 렌더링하는 동안 발생하거나 호출되지 않는다. 따라서 React는 이벤트 핸들러에서 이러한 종류의 오류를 복구하는 방법을 알고 있다.
     그래도 이벤트 핸들러내에서 오류를 잡아내야 한다면, 아래처럼 일반 Javascript try / catch 문을 사용하면 된다.
     
     ```javascript
     class MyComponent extends React.Component {
       constructor(props) {
         super(props);
         this.state = { error: null };
       }

       handleClick = () => {
         try {
           // Do something that could throw
         } catch (error) {
           this.setState({ error });
         }
       }

       render() {
         if (this.state.error) {
           return <h1>Caught an error.</h1>
         }
         return <div onClick={this.handleClick}>Click Me</div>
       }
     }
     ```
     위의 코드는 에러 바운더리 대신 바닐라 자바스크립트 try / catch 블록을 사용해서 오류를 잡아내고 있다.
29.  ### try catch 블록과 에러 바운더리의 차이점은?
     Try catch 블록은 명령 코드와 함께 작동하지만, 에러 바운더리는 선언 코드가 화면에 렌더링할 때이다.
     예를 들어, try catch 블록은 아래 명령 코드같이 사용된다.

     ```javascript
     try {
       showButton();
     } catch (error) {
       // ...
     }
     ```
     반면 에러 바운더리는 선언적 코드를 아래와 같이 감싼다.
     ```javascript
     <ErrorBoundary>
       <MyComponent />
     </ErrorBoundary>
     ```
     따라서 tree의 어딘가 **setState**로 인해서 **componentDidUpdate** 메서드에서 오류가 발생하면, 가장 가까운 에러 바운더리로 전파된다.

30.  ### react 16에서 잡히지 않는 오류의 동작은?
     React 16에서 에러 바운더리에 잡히지 않는 오류는 React 컴포넌트 tree를 마운트 해제한다. 이렇게 되는 이유는 손상된 UI를 완전히 제거하는 것보다 손상된 UI를 그대로 두는 것이 더 안 좋기 때문이다. 예를 들어, 결제 앱이 잘못된 금액을 표기하는 것보다 렌더링하지 않는 것이 낫다.

31.  ### 에러 바운더리의 적절한 위치는?
     에러 바운더리의 세분화는 프로젝트 필요에 따라 개발자에 따라 달라질 수 있다. 아래와 같은 접근법을 시행할 수 있다.

     1. 최상위 라우트 컴포넌트를 감싸서 전체 응용 프로그램에 대한 일반적인 에러 메시지를 표시할 수 있다.
     2. 각각의 컴포넌트를 에러 바운더리로 감싸서 나머지 응용 프로그램이 충돌하지 않도록 보호할 수 있다.

32.  ### 에러 바운더리에서 컴포넌트 스택 추적의 장점은?

     에러 메시지, 자바스크립트 스택과 별개로, React16은 에러 바운더리 개념을 사용하여 파일 이름과 행 번호를 포함한 컴포넌트 스택 추적을 표시한다. 예를 들어, BuggyCounter 컴포넌트는 아래와 같이 컴포넌트 스택 추적을 표시한다.

     ![stacktrace](images/error_boundary.png)

33.  ### 클래스 컴포넌트에 정의해야 하는 메서드는 무엇인가?

     render() 메서드는 클래스 컴포넌트에서 유일하게 필요한 메서드이다. 즉, render 메서드를 제외한 모든 메서드는 클래스 컴포넌트에서 선택사항이다.

34.  ### render 메서드의 return 가능한 타입은?

     아래는 render 메서드에서 사용되거나 return 되는 리스트입니다.

     1. **React elements:** React가 DOM 노드를 렌더링하도록 지시하는 Elements다. `<div/>` 와 같은 html elements와 사용자 정의 elements가 포함된다.
     2. **Arrays and fragments:** 여러 elements를 렌더링하기 위해 이를 감싼 배열과 Fragments를 반환한다.
     3. **Portals:** 자식은 다른 DOM 하위 트리로 렌더링한다.
     4. **String and numbers:** DOM에서 문자열과 숫자를 모두 텍스트 노드로 렌더링한다.
     5. **Booleans or null:** 아무것도 렌더링하지 않지만, 조건부로 콘텐츠를 렌더링할 때 사용된다.

35.  ### constructor의 주요 목적은?

     constructor는 주로 두 가지 목적으로 사용된다.

     1. this.state에 객체를 할당하여 로컬 상태를 초기화하기 위해서
     2. 이벤트 핸들러 메서드를 인스턴스에 바인딩하기 위해서 
     
     예를 들어 아래의 코드는 두 가지 경우를 모두 다루고 있다.
     
     ```javascript
     constructor(props) {
       super(props);
       // Don't call this.setState() here!
       this.state = { counter: 0 };
       this.handleClick = this.handleClick.bind(this);
     }
     ```

241. ### React 컴포넌트의 생성자를 정의해야 하나?
     
     필수는 아니다. 즉, state를 초기화 하지 않고, 메서드를 바인딩하지 않는다면, React 컴포넌트에 생성자를 구현할 필요 없다.

   **[⬆ Back to Top](#table-of-contents)**
    
242. ### default props란?

     defaultProps는 컴포넌트 클래스의 속성이며 클래스의 기본 props를 설정한다. undefined props에 사용되지만, null props에는 사용되지 않는다. 예를 들어, 버튼 컴포넌트의 색상 default prop 만들어보자.

     ```javascript
     class MyButton extends React.Component {
       // ...
     }

     MyButton.defaultProps = {
       color: 'red'
     };

     ```

     props.color가 없다면 기본값은 '빨간색'으로 설정된다. 즉, color props에 접근하려고 할 때마다 기본값이 사용된다.

     ```javascript
     render() {
        return <MyButton /> ; // props.color will be set to red
      }
     ```
     **Note:** null 값을 제공하면 null 값이 유지된다.

   **[⬆ Back to Top](#table-of-contents)**
    
243. ### componentWillUnmount에서 setState를 호출하면 안되는 이유는?

     컴포넌트 인스턴스가 마운트 해제되면 다시 마운트될 수 없음으로, componentWillUnmount()에서 setState()를 호출하면 안 된다.

   **[⬆ Back to Top](#table-of-contents)**
    
244. ### getDerivedStateFromError의 목적은?

     이 라이프사이클 메서드는 하위 컴포넌트가 오류를 발생한 후 호출된다. 매개 변수로 오류를 수신하고 state를 업데이트하기 위한 값을 반환한다. 라이프사이클 메서드의 사용법은 아래와 같다.

     ```javascript
     static getDerivedStateFromError(error)
     ```

     위의 라이프사이클 메서드를 사용하여 오류 바운더리 사용 예시는 아래와 같습니다.

     ```javascript
     class ErrorBoundary extends React.Component {
       constructor(props) {
         super(props);
         this.state = { hasError: false };
       }

       static getDerivedStateFromError(error) {
         // Update state so the next render will show the fallback UI.
         return { hasError: true };
       }

       render() {
         if (this.state.hasError) {
           // You can render any custom fallback UI
           return <h1>Something went wrong.</h1>;
         }

         return this.props.children;
       }
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
245. ### 리렌더링할 때 메서드의 순서는?

     props 또는 state의 변경으로 업데이트가 발생할 수 있다. 아래의 메서드는 컴포넌트를 리렌더링할 때 호출되는 순서이다.
     
     1. static getDerivedStateFromProps()
     2. shouldComponentUpdate()
     3. render()
     4. getSnapshotBeforeUpdate()
     5. componentDidUpdate()


   **[⬆ Back to Top](#table-of-contents)**
    
246. ### 에러 핸들링 중 호출되는 메서드는?
     
     아래는 메서드는 렌더링 도중 라이프사이클 메서드 또는 하위 컴포넌트의 생성자에서 오류가 발생하면 호출된다.
     
     1. static getDerivedStateFromError()
     2. componentDidCatch()

   **[⬆ Back to Top](#table-of-contents)**
    
247. ### displayName 클래스 속성의 목적은?

     displayName 문자열은 메시지 디버깅에 사용된다. 일반적으로 컴포넌트를 정의하는 함수 또는 클래스 이름에서 유추되므로 명시적으로 설정할 필요 없다. 디버깅 목적으로 다른 이름을 표시하거나 HOC를 작성할 때 명시적으로 설정할 수 있다.
     예를 들어, 디버깅을 쉽게 하려면 withSubscription HOC의 결과임을 알리는 displayName을 선택한다.

     ```javascript
     function withSubscription(WrappedComponent) {
       class WithSubscription extends React.Component {/* ... */}
       WithSubscription.displayName = `WithSubscription(${getDisplayName(WrappedComponent)})`;
       return WithSubscription;
     }

     function getDisplayName(WrappedComponent) {
       return WrappedComponent.displayName || WrappedComponent.name || 'Component';
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
248. ### react 응용프로그램의 브라우저 지원은 어디까지인가?

     React는 Internet Explorer 9 이상을 포함하여 널리 사용되는 모든 브라우저를 지원하지만, 일부 IE 9 및 IE 10과 같은 이전 브라우저에서는 폴리필이 필요하다. **es5-shim과 es5-sham** 폴리필을 사용하면 ES5 메서드들을 지원하지 않는 이전 브라우저에서 사용 가능하다.

   **[⬆ Back to Top](#table-of-contents)**
    
249. ### unmountComponentAtNode 메서드의 목적은?

     이 메서드는 react-dom 패키지에서 사용 가능하며, DOM에 마운트된 React 컴포넌트를 제거하고 이벤트 핸들러와 state를 정리한다. 컨테이너에 컴포넌트가 마운트되지 않은 경우 이 함수를 호출하면 아무 작업도 하지 않는다. 컴포넌트가 마운트 해제된 경우 true, 마운트 해제할 컴포넌트가 없는 경우 false를 반환한다. 메서드 사용법은 다음과 같다.

     ```javascript
     ReactDOM.unmountComponentAtNode(container)
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
250. ### code-splitting이란?

     Code-Splitting은 Webpack과 Browserify와 같은 번들러에서 지원하는 기능으로 런타임에 동적으로 로드할 수 있는 여러 번들을 만들 수 있다. react 프로젝트는 동적 import() 기능을 통해 code splitting을 지원한다.
     예를 들어, 아래와 같은 스니핏 코드에서는 moduleA.js와 모든 고유한 종속성을 사용자가 '로드' 버튼을 클릭했을 때 로드하는 별도의 chuck로 만든다. 
     
     **moduleA.js**
     ```javascript
     const moduleA = 'Hello';

     export { moduleA };
     ```

     **App.js**
     ```javascript
     import React, { Component } from 'react';

     class App extends Component {
       handleClick = () => {
         import('./moduleA')
           .then(({ moduleA }) => {
             // Use moduleA
           })
           .catch(err => {
             // Handle failure
           });
       };

       render() {
         return (
           <div>
             <button onClick={this.handleClick}>Load</button>
           </div>
         );
       }
     }

     export default App;

     ```

   **[⬆ Back to Top](#table-of-contents)**
    
251. ### strict mode의 장점은?
     `<StrictMode>`는 아래와 같은 경우에 유용하다.

     1. **안전하지 않은 라이프사이클 메서드를 가진** 컴포넌트를 식별해준다.
     2. **레거시 문자열 참조** API 사용에 대한 경고를 해준다.
     3. 예상치 못한 **부작용**을 감지한다.
     4. **레거시 컨텍스트** API를 감지한다.
     5. 더 이상 사용되지 않는 findDOMNode 사용에 대해 경고를 해준다.

   **[⬆ Back to Top](#table-of-contents)**
    
252. ### Keyed Fragments란?

     명시적 `<React.Fragment>` 구문으로 선언된 Fragments에는 key가 있을 수 있다. 일반적으로 사용하는 경우는 아래와 같이 컬렉션을 배열에 매핑한다.

     ```javascript
     function Glossary(props) {
       return (
         <dl>
           {props.items.map(item => (
             // Without the `key`, React will fire a key warning
             <React.Fragment key={item.id}>
               <dt>{item.term}</dt>
               <dd>{item.description}</dd>
             </React.Fragment>
           ))}
         </dl>
       );
     }
     ```

     **Note:** key는 Fragment에 전달할 수 있는 유일한 속성이다. 앞으로는, 이벤트 핸들러와 같은 추가 속성이 지원될 수 있다.

   **[⬆ Back to Top](#table-of-contents)**
    
253. ### React는 모든 HTML 속성을 지원하나?

     React 16 버전에서, 표준과 사용자 정의 DOM 속성 모두 지원한다. React 컴포넌트는 종종 사용자 정의와 DOM 관련 props를 모두 사용하므로, React는 DOM API와 마찬가지로 camelCase 규칙을 사용한다. 표준 HTML 속성을 사용하고 props를 사용하지 않은 예시이다.

     ```javascript
     <div tabIndex="-1" />      // Just like node.tabIndex DOM API
     <div className="Button" /> // Just like node.className DOM API
     <input readOnly={true} />  // Just like node.readOnly DOM API
     ```

     props는 특별한 경우는 제외하고 해당 HTML 속성과 유사하게 작동한다. 또한 모든 SVG 속성을 지원한다.

   **[⬆ Back to Top](#table-of-contents)**
    
254. ### HOC의 한계는?

     고차 컴포넌트는 장점과는 무관하게 몇 가지 경고 사항이 있습니다.

     1. **render 메서드 안에서 사용해서는 안 된다. :** 컴포넌트의 redner 메서드 내에서 HOC를 적용하는 것은 좋지 않다.

        ```javascript
        render() {
          // 새로운 버전의 EnhancedComponent가 렌더링할 때마다 생성된다.
          // EnhancedComponent1 !== EnhancedComponent2
          const EnhancedComponent = enhance(MyComponent);
          // That causes the entire subtree to unmount/remount each time!
          return <EnhancedComponent />;
        }
        ```

        위의 코드는 컴포넌트를 다시 마운트하면 해당 컴포넌트 및 모든 하위 컴포넌트의 state를 잃어버려 성능에 영향을 미친다. 대신 컴포넌트가 한 번만 작성되도록 컴포넌트 정의 외부에서 HOC를 적용하면 된다.
     2. **static 메서드를 복사해야 한다. :** HOC를 새로운 컴포넌트에 적용할 때 새로운 컴포넌트에는 원본 컴포넌트의 static 메서드가 없다.

        ```javascript
        // staic 메서드 정의
        WrappedComponent.staticMethod = function() {/*...*/}
        // HOC 적용
        const EnhancedComponent = enhance(WrappedComponent);

        // enhanced component는 static 메서드를 가지고 있지 않다.
        typeof EnhancedComponent.staticMethod === 'undefined' // true
        ```

        반환하기 전에 메서드를 컨테이너에 복사하여 해결할 수 있다.

        ```javascript
        function enhance(WrappedComponent) {
          class Enhance extends React.Component {/*...*/}
          // Must know exactly which method(s) to copy :(
          Enhance.staticMethod = WrappedComponent.staticMethod;
          return Enhance;
        }
        ```
     3. **Refs가 전달되지 않는다. :** HOC의 경우 모든 props를 래핑 된 컴포넌트로 전달해야 하지만 refs는 적용되지 않는다. ref는 실제로 key와 비슷한 props이 아니기 때문이다. 이 경우에는 React.forwardRef API 사용하면 된다.

   **[⬆ Back to Top](#table-of-contents)**
    
255. ### 개발자 도구에서 forwardRefs를 디버깅하는 방법은?

     **React.forwardRef** 는 렌더링 함수를 매개 변수로 받고 있으며, 개발자 도구는 이 함수를 사용하여 ref 전달 컴포넌트에 표시할 내용을 결정한다. 예를 들어, 렌더링 함수의 이름을 지정하지 않거나 displayName 속성을 사용하지 않으면 개발자 도구에서 ”ForwardRef”로 표시된다.

     ```javascript
     const WrappedComponent = React.forwardRef((props, ref) => {
       return <LogProps {...props} forwardedRef={ref} />;
     });
     ```

     그러나 렌더링 함수의 이름을 지정하게 되면 **”ForwardRef(myFunction)”**으로 나타난다.

     ```javascript
     const WrappedComponent = React.forwardRef(
       function myFunction(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }
     );
     ```
     
     대안으로, forwardRef 함수에 displayName 속성을 설정할 수 있다.

     ```javascript
     function logProps(Component) {
       class LogProps extends React.Component {
         // ...
       }

       function forwardRef(props, ref) {
         return <LogProps {...props} forwardedRef={ref} />;
       }

       // Give this component a more helpful display name in DevTools.
       // e.g. "ForwardRef(logProps(MyComponent))"
       const name = Component.displayName || Component.name;
       forwardRef.displayName = `logProps(${name})`;

       return React.forwardRef(forwardRef);
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
256. ### 컴포넌트 props의 기본값은 true인가?
     
     prop에 아무 값도 전달하지 않는다면, 기본값은 true이다. 이 동작은 HTML의 동작과 일치하게 할 수 있다. 예를 들어 아래와 같은 표현식은 동일한 표현이다.

     ```javascript
     <MyInput autocomplete />

     <MyInput autocomplete={true} />
     ```
     **Note:** 이 방법은 ES6 객체 속기 (예, {name: name}의 약자는 {name})와 혼동할 수 있으므로 사용하지 않는 것이 좋다.

   **[⬆ Back to Top](#table-of-contents)**
    
257. ### NextJS는 무엇이며, 주요한 기능은?
     
     Next.js는 React로 만들어진 정적, 서버 렌더링 응용프로그램을 위한 대중적이고 가벼운 프레임 워크이다. 또한 스타일링과 라우팅 솔루션을 제공한다. 아래는 NextJS가 제공하는 주요 기능이다.

     1. 기본적으로 서버 렌더링
     2. 빠른 페이지 로딩을 위한 자동 코드 분할
     3. 간단한 클라이언트 사이드 라우팅(page기반)
     4. HMR을 지원하는 웹팩 기반 개발 환경
     5. Express 또는 다른 Node.js HTTP 서버로 구현할 수 있다.
     6. 고유한 Babel 및 Webpack 구성으로 사용자 정의가 가능하다.

   **[⬆ Back to Top](#table-of-contents)**
    
258. ### 이벤트 핸들러를 컴포넌트에 어떻게 전달하나?
     
     이벤트 핸들러 및 함수를 하위 컴포넌트에 props로 전달할 수 있다. 아래와 같이 자식 컴포넌트에서 사용할 수 있다.

     ```
     <button onClick={this.handleClick}>
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
259. ### render 메서드에서 화살표 함수를 사용하는 것이 좋은가?

     예, 사용할 수 있다. 콜백 함수에 매개 변수를 전달하는 가장 쉬운 방법이다. 그러나 사용하는 동안 성능을 최적화해야 한다.

     ```javascript
     class Foo extends Component {
       handleClick() {
         console.log('Click happened');
       }
       render() {
         return <button onClick={() => this.handleClick()}>Click Me</button>;
       }
     }
     ```
     **Note:** render 메서드에서 화살표 함수를 사용하면 컴포넌트가 렌더링 될 때마다 새로운 기능이 생성되어 성능에 영향을 줄 수 있다.

   **[⬆ Back to Top](#table-of-contents)**
    
260. ### 함수가 여러 번 호출되는 것을 방지하는 방법은?

     **onClick 또는 onScroll**과 같은 이벤트 핸들러를 사용하고 콜백이 너무 빨리 발생하지 않도록 하려면 콜백 실행 속도를 제한할 수 있다. 아래와 같은 방법으로 가능하다.

     1. **Throttling:** 시간을 기반으로 빈도에 따라 변경이 된다. 예를 들어, lodash의 _.throttle 함수를 사용하여 사용할 수 있다.
     2. **Debouncing:** 일정 기간 사용하지 않으면 변경 사항을 실행한다. 예를 들어, lodash의 _.debounce 함수를 사용하여 사용할 수 있다.
     3. **RequestAnimationFrame throttling:** requestAnimationFrame에 따라 변경된다. 예를 들어, lodash의 raf-schd 함수를 사용하여 사용할 수 있다.

   **[⬆ Back to Top](#table-of-contents)**
    
261. ### JSX가 Injection 공격은 막는 방법은?

     React DOM은 렌더링하기 전에 JSX에 포함된 모든 값은 escape 처리한다. 따라서 애플리케이션에 아무것도 주입되지 않는 것을 보장한다. 모든 것이 렌더링되기 전에 문자열로 변환된다. 예를 들어 아래와 같이 사용자 입력을 포함할 수 있다.

     ```javascript
     const name = response.potentiallyMaliciousInput;
     const element = <h1>{name}</h1>;
     ```

     이렇게 하면 애플리케이션에서 XSS(Cross-site-scripting) 공격을 방지할 수 있다.

   **[⬆ Back to Top](#table-of-contents)**
    
262. ### 렌더링 된 요소는 어떻게 업데이트하나?

     새로 작성된 요소를 ReactDOM의 render 메서드에 전달하여 UI(렌더링 된 요소로 표시)를 업데이트 할 수 있다. 예를 들어, 똑딱거리는 시계를 예로 들자면, render 메서드를 여러 번 호출하여 시간을 업데이트한다.

     ```javascript
     function tick() {
       const element = (
         <div>
           <h1>Hello, world!</h1>
           <h2>It is {new Date().toLocaleTimeString()}.</h2>
         </div>
       );
       ReactDOM.render(element, document.getElementById('root'));
     }

     setInterval(tick, 1000);
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
263. ### props가 읽기 전용이어야 하는 이유는?

     컴포넌트를 함수나 클래스로 선언할 때 자신의 props를 수정해서는 안 된다. 아래의 capital 함수를 예로 들어보자.

     ```javascript
     function capital(amount, interest) {
        return amount + interest;
     }
     ```
     
     위의 함수는 입력을 변경하지 않으면서 항상 동일한 입력에 대해 동일한 결과를 반환하기 때문에 "순수"하다고 한다. 따라서, React에는 "모든 React 컴포넌트는 props와 관련된 것은 순수함수처럼 작동해야 한다." 라는 단일 규칙을 가지고 있다.

   **[⬆ Back to Top](#table-of-contents)**
    
264. ### state updates가 어떻게 병합되나?

     컴포넌트에서 setState()를 실행하면, React 사용자가 제공한 object를 현재 state로 병합한다. 예를 들어, 게시물 및 댓글 세부 정보를 state 변수로 사용하는 페이스북 사용자를 살펴보자.

     ```javascript
       constructor(props) {
         super(props);
         this.state = {
           posts: [],
           comments: []
         };
       }
     ```

     아래와 같이 별도의 setState()를 호출하여 독립적으로 업데이트할 수 있다.

     ```javascript
      componentDidMount() {
         fetchPosts().then(response => {
           this.setState({
             posts: response.posts
           });
         });

         fetchComments().then(response => {
           this.setState({
             comments: response.comments
           });
         });
       }
     ```

     위의 코드 스니핏에서 언급했듯이 this.setState({comments})는 게시물 변수를 수정하거나 바꾸지 않고 comments 변수만 업데이트한다.

   **[⬆ Back to Top](#table-of-contents)**
    
265. ### 이벤트 핸들러에 인수를 어떻게 넘기나?
     
     반복 또는 루프를 도는 중에 추가적인 매개 변수를 이벤트 핸들러에 전달하는 것이 일반적이다. 화살표 함수 또는 메서드 바인드로 가능하다. 그리드에서 업데이트된 사용자 정보로 예를 들어 보자.

     ```javascript
     <button onClick={(e) => this.updateUser(userId, e)}>Update User details</button>
     <button onClick={this.updateUser.bind(this, userId)}>Update User details</button>
     ```

     두 가지 접근방식에서, 합성 인수 e는 두 번째 인자로 전달된다. 화살표 함수의 경우에는 명시적으로 전달해 주어야 하며, 메서드 바인드는 자동으로 전달된다.

   **[⬆ Back to Top](#table-of-contents)**
    
266. ### 컴포넌트 렌더링을 막는 방법은?
     
     특정 조건에 따라 null을 반환하여 컴포넌트가 렌더링 되지 않도록 할 수 있다. 아래와 같이 조건부로 컴포넌트를 렌더링할 수 할 수 있다.

     ```javascript
     function Greeting(props) {
       if (!props.loggedIn) {
         return null;
       }

       return (
         <div className="greeting">
           welcome, {props.name}
         </div>
       );
     }
     ```

     ```javascript
     class User extends React.Component {
       constructor(props) {
         super(props);
         this.state = {loggedIn: false, name: 'John'};
       }

       render() {
        return (
            <div>
              //Prevent component render if it is not loggedIn
              <Greeting loggedIn={this.state.loggedIn} />
              <UserDetails name={this.state.name}>
            </div>
        );
       }
     ```

     위의 예제에서, greeting 컴포넌트는 조건문을 적용하고 null 값을 반환하여 렌더링 부분은 건너뛴다.

   **[⬆ Back to Top](#table-of-contents)**
    
267. ### index를 키로 안전하게 사용하기 위한 조건은?

     index를 키로 안전하게 사용하기 위한 3가지 조건이 있다.

     1. 목록과 항목은 정적이다. 계산되지 않고 변경 않을 경우.
     2. 목록에 있는 항목들이 id가 없을 경우.
     3. 목록이 다시 정렬되거나 필터링 되지 않을 경우

   **[⬆ Back to Top](#table-of-contents)**
    
268. ### 키가 전체에서 고유해야 하나?

     배열 내에서 사용되는 키는 형제 사이에서 고유해야 하지만 전체적으로는 고유할 필요 없다. 즉, 두 개의 다른 배열에서 동일한 키를 사용할 수 있다. 예를 들어, 아래의 Book 컴포넌트는 다른 배열 두 개를 사용하고 있다.

     ```javascript
     function Book(props) {
       const index = (
         <ul>
           {props.pages.map((page) =>
             <li key={page.id}>
               {page.title}
             </li>
           )}
         </ul>
       );
       const content = props.pages.map((page) =>
         <div key={page.id}>
           <h3>{page.title}</h3>
           <p>{page.content}</p>
           <p>{page.pageNumber}</p>
         </div>
       );
       return (
         <div>
           {index}
           <hr />
           {content}
         </div>
       );
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
269. ### Form 처리에 가장 많이 사용되는 선택지는?

     Formik은 유효성 검사, 방문 페이지 추적, form 제출 처리와 같은 솔루션을 제공하는 react 라이브러리다. 구체적으로 다름과 같이 분류할 수 있다.

     1. form state 값 가져오기
     2. 유효성 검사와 오류 메시지
     3. form 제출 처리

     최소한의 API로 확장할 수 있고 성능이 뛰어난 form 헬퍼를 생성하여 귀찮은 것을 해결하는 데 사용된다.

   **[⬆ Back to Top](#table-of-contents)**
    
270. ### redux form 라이브러리보다 formik의 장점은?

     다음은 redux form 라이브러리보다 formik을 권장하는 주요 이유이다.

     1. form state는 본질적으로 단기적이며 로컬이므로 Redux(또는 모든 종류의 Flux 라이브러리) 에서 추적할 필요가 없다.
     2. Redux-Form은 EVERY SINGLE KEYSTROKE에서 전체 최상위 Redux reducer를 여러 번 호출한다. 이렇게 하면 큰 앱의 입력 대기 시간이 늘어난다.
     3. Redux-Form은 22.5 kB로 축소된 gzip인 반면 Formik은 12.7 kB이다.

   **[⬆ Back to Top](#table-of-contents)**
    
271. ### 상속할 필요가 없는 이유는?

     React에서 컴포넌트 간 코드를 재사용하려면 상속 대신 composition을 사용하는 것이 좋다. Props와 composition 모두 명시적이고 안전한 방식으로 컴포넌트의 형태와 기능을 커스텀하는데 필요한 모든 유연성을 보장한다. 반면, 컴포넌트 간 UI가 아닌 기능을 재사용하려면, 별도의 JavaScript 모듈로 구분하는 것이 좋다. 이후 컴포넌트를 가져와 확장하지 않고 함수, 개체, 클래스를 사용한다.

   **[⬆ Back to Top](#table-of-contents)**
    
272. ### react 애플리케이션에서 웹 컴포넌트를 사용할 수 있나?

     react 애플리케이션에서 웹 컴포넌트를 사용할 수 있다. 많은 개발자가 이 조합을 사용하지 않더라도 웹 컴포넌트로 만들어진 다른 UI 컴포넌트를 사용하는 경우 특히 필요할 수 있다. 예를 들어 Vaadin 날짜 선택기 웹 컴포넌트를 사용하는 것을 보자.

     ```javascript
     import React, { Component } from 'react';
     import './App.css';
     import '@vaadin/vaadin-date-picker';
     class App extends Component {
       render() {
         return (
           <div className="App">
             <vaadin-date-picker label="When were you born?"></vaadin-date-picker>
           </div>
         );
       }
     }
     export default App;
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
273. ### dynamic import란?
     
     dynamic import() 문법은 현재 표준 문법이 아닌 ECMAScript 제안이다. 가까운 미래에 추가될 것이다(실제로 2020에 추가 예정). dynamic import()를 사용하여 code-splitting 할 수 있다. 덧셈 예를 들어보자.

     1. **Normal Import**
     ```javascript
     import { add } from './math';
     console.log(add(10, 20));
     ```
     2. **Dynamic Import**
     ```javascript
     import("./math").then(math => {
       console.log(math.add(10, 20));
     });
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
274. ### loadable 컴포넌트란?

     서버 렌더링 앱에서 code-splitting을 하는 경우, React.lazy와 Suspense를 아직 서버 측 렌더링에 사용할 수 없으므로 Loadable 컴포넌트를 사용하는 것이 좋다. Loadable을 사용하면 dynamic import를 일반 컴포넌트로 렌더링할 수 있다. 예를 들어보면,

     ```javascript
     import loadable from '@loadable/component'

     const OtherComponent = loadable(() => import('./OtherComponent'))

     function MyComponent() {
       return (
         <div>
           <OtherComponent />
         </div>
       )
     }
     ```

     이제 OtherComponent는 별도의 번들로 로드된다.

   **[⬆ Back to Top](#table-of-contents)**
    
275. ### suspense 컴포넌트란?

     dynamic import가 포함된 모듈의 부모 컴포넌트가 렌더링 될 때까지 로드가 되지 않은 경우 로딩 표시기를 사용하여 로드될 때까지 대체 컨텐츠를 표시한다. 이를 **Suspense** 컴포넌트를 사용하여 수행할 수 있다. 예를 들어 아래 코드는 suspense 컴포넌트를 사용한다.

     ```javascript
     const OtherComponent = React.lazy(() => import('./OtherComponent'));

     function MyComponent() {
       return (
         <div>
           <Suspense fallback={<div>Loading...</div>}>
             <OtherComponent />
           </Suspense>
         </div>
       );
     }
     ```
     위 코드에서 언급했듯이 Suspense는 Layzy 컴포넌트로 감싸진다.

   **[⬆ Back to Top](#table-of-contents)**
    
276. ### 라우트 기반의 코드 스플리팅이란?

     코드 스플리팅을 사용해 볼 좋은 장소 중 하나는 라우트다. 전체 페이지가 한 번에 렌더링 되므로 사용자가 페이지의 다른 요소와 동시에 상호 작용할 가능성이 없다. 이로 인해 사용자 경험이 방해받지 않는다. React.lazy와 함께 Reat Router 같은 라이브러리를 사용하여 경로 기반 웹 사이트를 예를 들어보자.

     ```javascript
     import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';
     import React, { Suspense, lazy } from 'react';

     const Home = lazy(() => import('./routes/Home'));
     const About = lazy(() => import('./routes/About'));

     const App = () => (
       <Router>
         <Suspense fallback={<div>Loading...</div>}>
           <Switch>
             <Route exact path="/" component={Home}/>
             <Route path="/about" component={About}/>
           </Switch>
         </Suspense>
       </Router>
     );
     ```

     위의 코드에서, 코드 스플리팅은 각 경로 수준에서 발생한다.

   **[⬆ Back to Top](#table-of-contents)**
    
277. ### context를 어떻게 사용하는지에 대한 예제

     **Context**는 React 컴포넌트 트리에서 **global**로 데이터를 공유하도록 설계되었다. 예를 들어, 아래 코드에서 Button 컴포넌트의 스타일을 지정하기 위해 "테마" prop을 수동으로 연결할 수 있다.

     ```javascript
     //Lets create a context with a default theme value "luna"
     const ThemeContext = React.createContext('luna');
     // Create App component where it uses provider to pass theme value in the tree
     class App extends React.Component {
       render() {
         return (
           <ThemeContext.Provider value="nova">
             <Toolbar />
           </ThemeContext.Provider>
         );
       }
     }
     // A middle component where you don't need to pass theme prop anymore
     function Toolbar(props) {
       return (
         <div>
           <ThemedButton />
         </div>
       );
     }
     // Lets read theme value in the button component to use
     class ThemedButton extends React.Component {
       static contextType = ThemeContext;
       render() {
         return <Button theme={this.context} />;
       }
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
278. ### context에서 기본값의 목적은?

     defaultValue 인수는 컴포넌트에 트리에서 일치하는 Provider가 없는 경우에 사용된다. 이는 컴포넌트를 감싸지 않고 분리하여 테스트하는데 도움이 될 수 있다. 아래 코드는 테마 기본값을 Luna로 제공한다.

     ```javascript
     const MyContext = React.createContext(defaultValue);
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
279. ### contextType은 어떻게 사용하나?

     ContextType은 context 객체를 소비하는데 사용된다. contextType 속성은 2가지 방식으로 사용된다.

     1. **클래스 속성으로 contextType:**
     클래스의 contextType 속성에는 React.createContext()로 만든 Context 객체를 할당할 수 있다. 그런 다음모든 라이프 사이클 메서드와 렌더링 함수에서 this.context를 사용하여 해당 contextType의 가장 가까운 현재 값을 사용할 수 있다. 아래와 같이 MyClass에 contextType 속성을 할당 할 수 있다.

     ```javascript
     class MyClass extends React.Component {
       componentDidMount() {
         let value = this.context;
         /* perform a side-effect at mount using the value of MyContext */
       }
       componentDidUpdate() {
         let value = this.context;
         /* ... */
       }
       componentWillUnmount() {
         let value = this.context;
         /* ... */
       }
       render() {
         let value = this.context;
         /* render something based on the value of MyContext */
       }
     }
     MyClass.contextType = MyContext;
     ```

     2. **Static field** 정적 클래스 필드를 사용하여 공용 클래스 필드 구문을 사용하는 contextType을 초기화할 수 있다.

     ```javascript
     class MyClass extends React.Component {
       static contextType = MyContext;
       render() {
         let value = this.context;
         /* render something based on the value */
       }
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
280. ### consumer란?

     Consumer란 context 변경을 구독하는 React 컴포넌트이다. 현재 context 값을 인수로 받고 react node를 반환하는 자식 함수가 필요하다. 함수에 전달된 value 인수는 트리에서 context에서 가장 가까운 Provider의 prop 값과 동일하다. 간단한 예를 보자.

     ```javascript
     <MyContext.Consumer>
       {value => /* render something based on the context value */}
     </MyContext.Consumer>
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
281. ### How do you solve performance corner cases while using context?
     The context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. For example, the code below will re-render all consumers every time the Provider re-renders because a new object is always created for value.
     ```javascript
     class App extends React.Component {
       render() {
         return (
           <Provider value={{something: 'something'}}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```
     This can be solved by lifting up the value to parent state,
     ```javascript
     class App extends React.Component {
       constructor(props) {
         super(props);
         this.state = {
           value: {something: 'something'},
         };
       }

       render() {
         return (
           <Provider value={this.state.value}>
             <Toolbar />
           </Provider>
         );
       }
     }
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
282. ### What is the purpose of forward ref in HOCs?
     Refs will not get passed through because ref is not a prop. It handled differently by React just like **key**. If you add a ref to a HOC, the ref will refer to the outermost container component, not the wrapped component. In this case, you can use Forward Ref API. For example, we can explicitly forward refs to the inner FancyButton component using the React.forwardRef API.
     The below HOC logs all props,
     ```javascript
     function logProps(Component) {
       class LogProps extends React.Component {
         componentDidUpdate(prevProps) {
           console.log('old props:', prevProps);
           console.log('new props:', this.props);
         }

         render() {
           const {forwardedRef, ...rest} = this.props;

           // Assign the custom prop "forwardedRef" as a ref
           return <Component ref={forwardedRef} {...rest} />;
         }
       }

       return React.forwardRef((props, ref) => {
         return <LogProps {...props} forwardedRef={ref} />;
       });
     }
     ```
     Let's use this HOC to log all props that get passed to our “fancy button” component,
     ```javascript
     class FancyButton extends React.Component {
       focus() {
         // ...
       }

       // ...
     }
     export default logProps(FancyButton);
     ```
     Now lets create a ref and pass it to FancyButton component. In this case, you can set focus to button element.
     ```javascript
     import FancyButton from './FancyButton';

     const ref = React.createRef();
     ref.current.focus();
     <FancyButton
       label="Click Me"
       handleClick={handleClick}
       ref={ref}
     />;
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
283. ### Is it ref argument available for all functions or class components?
     Regular function or class components don’t receive the ref argument, and ref is not available in props either. The second ref argument only exists when you define a component with React.forwardRef call.

   **[⬆ Back to Top](#table-of-contents)**
    
284. ### Why do you need additional care for component libraries while using forward refs?
     When you start using forwardRef in a component library, you should treat it as a breaking change and release a new major version of your library. This is because your library likely has a different behavior such as what refs get assigned to, and what types are exported. These changes can break apps and other libraries that depend on the old behavior.

   **[⬆ Back to Top](#table-of-contents)**
    
285. ### How to create react class components without ES6?
     If you don’t use ES6 then you may need to use the create-react-class module instead. For default props, you need to define getDefaultProps() as a function on the passed object. Whereas for initial state, you have to provide a separate getInitialState method that returns the initial state.
     ```javascript
     var Greeting = createReactClass({
       getDefaultProps: function() {
           return {
             name: 'Jhohn'
           };
         },
       getInitialState: function() {
           return {message: this.props.message};
         },
       handleClick: function() {
          console.log(this.state.message);
       },
       render: function() {
         return <h1>Hello, {this.props.name}</h1>;
       }
     });
     ```
     **Note:** If you use createReactClass then autobinding is available for all methods. i.e, You don't need to use .bind(this) with in constructor for event handlers.

   **[⬆ Back to Top](#table-of-contents)**
    
286. ### Is it possible to use react without JSX?
     Yes, JSX is not mandatory for using React. Actually it is convenient when you don’t want to set up compilation in your build environment. Each JSX element is just syntactic sugar for calling React.createElement(component, props, ...children). For example, let us take a greeting example with JSX,
     ```javascript
     class Greeting extends React.Component {
       render() {
         return <div>Hello {this.props.message}</div>;
       }
     }

     ReactDOM.render(
       <Greeting message="World" />,
       document.getElementById('root')
     );
     ```
     You can write the same code without JSX as below,
     ```javascript
     class Greeting extends React.Component {
       render() {
         return React.createElement('div', null, `Hello ${this.props.message}`);
       }
     }

     ReactDOM.render(
       React.createElement(Greeting, {message: 'World'}, null),
       document.getElementById('root')
     );
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
287. ### What is diffing algorithm?
     React needs to use algorithms to find out how to efficiently update the UI to match the most recent tree. The diffing algorithms is generating the minimum number of operations to transform one tree into another. However, the algorithms have a complexity in the order of O(n3) where n is the number of elements in the tree.
     In this case, for displaying 1000 elements would require in the order of one billion comparisons. This is far too expensive. Instead, React implements a heuristic O(n) algorithm based on two assumptions:
     1. Two elements of different types will produce different trees.
     2. The developer can hint at which child elements may be stable across different renders with a key prop.

   **[⬆ Back to Top](#table-of-contents)**
    
288. ### diffing 알고리즘에 적용되는 규칙은?

     서로 다른 트리를 비교할 때, React는 먼저 두 개의 root element를 비교한다. root element의 타입에 따라 동작이 다르다. reconciliation 알고리즘 중 아래의 규칙을 따른다.

     1. **다른 타입의 Elements:**
        root element가 다른 타입을 가질 때마다 React는 이전 트리를 분해하고 처음부터 새로운 트리를 만든다. 예를 들어, elements `<a>`는 `<img>`로, 또는 `<Article>`에서 `<Comment>`로 다른 타입의 element는 전체를 다시 작성한다.
     2. **동일한 타입의 DOM Elements:**
        동일한 타입의 두 React DOM element를 비교할 때 React는 두 속성을 모두 보고 동일한 기본 DOM 노드를 유지하며 변경된 속성만 업데이트한다. className 속성을 제외한 속성이 동일한 DOM element로 예제를 보자.
        ```javascript
        <div className="show" title="ReactJS" />

        <div className="hide" title="ReactJS" />
        ```
     3. **동일한 타입의 컴포넌트 Elements**
        컴포넌트가 업데이트 되면, 인스턴스는 동일하게 유지되므로 렌더링에서 state는 유지된다. React는 하위 element 인스턴스의 prop을 새 element와 일치하도록 업데이트하고 하위 인스턴스에서 componentWillReceiveProps()와 componentWillUpdate()를 호출한다. 그런 다음, render() 메서드가 호출되고 이전 결과와 새 결과에서 재귀적으로 diff 알고리즘이 이루어진다.
     4. **Children 재귀:**
        DOM 노드의 자식에 대해 재귀가 이루어질 때, React는 두 개의 자식 목록을 동시에 반복하고 차이가 있을 때마다 변이를 일으킨다. 예를 들어, 자식의 끝에 element를 추가할 때 두 트리를 변경시키는 게 유리하다.
        ```javascript
        <ul>
          <li>first</li>
          <li>second</li>
        </ul>

        <ul>
          <li>first</li>
          <li>second</li>
          <li>third</li>
        </ul>

        ```
     5. **keys 핸들링**
     React는 key 속성을 지원한다. 자식에 키가 있으면, React는 이 키를 사용하여 원래 트리의 자식을 다음 트리의 자식과 일치시킨다. 예를 들어, key를 추가하면 트리 변환이 효율적이다.
     ```javascript
     <ul>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>

     <ul>
       <li key="2014">Connecticut</li>
       <li key="2015">Duke</li>
       <li key="2016">Villanova</li>
     </ul>
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
289. ### When do you need to use refs?
     There are few use cases to go for refs
     1. Managing focus, text selection, or media playback.
     2. Triggering imperative animations.
     3. Integrating with third-party DOM libraries.

   **[⬆ Back to Top](#table-of-contents)**
    
290. ### Is it prop must be named as render for render props?
     Even though the pattern named render props, you don’t have to use a prop named render to use this pattern. i.e,  Any prop that is a function that a component uses to know what to render is technically a “render prop”. Lets take an example with the children prop for render props,
     ```javascript
     <Mouse children={mouse => (
       <p>The mouse position is {mouse.x}, {mouse.y}</p>
     )}/>
     ```
     Actually children prop doesn’t need to be named in the list of “attributes” in JSX element. Instead, you can keep it directly inside element,
     ```javascript
     <Mouse>
       {mouse => (
         <p>The mouse position is {mouse.x}, {mouse.y}</p>
       )}
     </Mouse>
     ```
     While using this above technique(without any name), explicitly state that children should be a function in your propTypes.
     ```javascript
     Mouse.propTypes = {
       children: PropTypes.func.isRequired
     };
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
291. ### What are the problems of using render props with pure components?
     If you create a function inside a render method, it negates the purpose of pure component. Because the shallow prop comparison will always return false for new props, and each render in this case will generate a new value for the render prop. You can solve this issue by defining the render function as instance method.

   **[⬆ Back to Top](#table-of-contents)**
    
292. ### How do you create HOC using render props?
     You can implement most higher-order components (HOC) using a regular component with a render prop. For example, if you would prefer to have a withMouse HOC instead of a <Mouse> component, you could easily create one using a regular <Mouse> with a render prop.
     ```javascript
     function withMouse(Component) {
       return class extends React.Component {
         render() {
           return (
             <Mouse render={mouse => (
               <Component {...this.props} mouse={mouse} />
             )}/>
           );
         }
       }
     }
     ```
     This way render props gives the flexibility of using either pattern.

   **[⬆ Back to Top](#table-of-contents)**
    
293. ### What is windowing technique?
     Windowing is a technique that only renders a small subset of your rows at any given time, and can dramatically reduce the time it takes to re-render the components as well as the number of DOM nodes created. If your application renders long lists of data then this technique is recommended. Both react-window and react-virtualized are popular windowing libraries which provides several reusable components for displaying lists, grids, and tabular data.

   **[⬆ Back to Top](#table-of-contents)**
    
294. ### How do you print falsy values in JSX?
     The falsy values such as false, null, undefined, and true are valid children but they don't render anything. If you still want to display them then you need to convert it to string. Let's take an example on how to convert to a string,
     ```javascript
     <div>
       My JavaScript variable is {String(myVariable)}.
     </div>
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
295. ### What is the typical use case of portals?
     React portals are very useful when a parent component has overflow: hidden or has properties that affect the stacking context(z-index,position,opacity etc styles) and you need to visually “break out” of its container. For example, dialogs, global message notifications, hovercards, and tooltips.

   **[⬆ Back to Top](#table-of-contents)**
    
296. ### How do you set default value for uncontrolled component?
     In React, the value attribute on form elements will override the value in the DOM. With an uncontrolled component, you might want React to specify the initial value, but leave subsequent updates uncontrolled. To handle this case, you can specify a **defaultValue** attribute instead of **value**.
     ```javascript
     render() {
       return (
         <form onSubmit={this.handleSubmit}>
           <label>
             User Name:
             <input
               defaultValue="John"
               type="text"
               ref={this.input} />
           </label>
           <input type="submit" value="Submit" />
         </form>
       );
     }
     ```
     The same applies for `select` and `textArea` inputs. But you need to use **defaultChecked** for `checkbox` and `radio` inputs.

   **[⬆ Back to Top](#table-of-contents)**
    
297. ### What is your favorite React stack?
     Even though the tech stack varies from developer to developer, the most popular stack is used in react boilerplate project code. It mainly uses Redux and redux-saga for state management and asynchronous side-effects, react-router for routing purpose, styled-components for styling react components, axios for invoking REST api, and other supported stack such as webpack, reselect, ESNext, Babel.
     You can clone the project https://github.com/react-boilerplate/react-boilerplate and start working on any new react project.

   **[⬆ Back to Top](#table-of-contents)**
    
298. ### What is the difference between Real DOM and Virtual DOM?
     Below are the main differences between Real DOM and Virtual DOM,

     | Real DOM | Virtual DOM |
     | ----- | ------- |
     | Updates are slow | Updates are fast |
     | DOM manipulation is very expensive. | DOM manipulation is very easy |
     | You can update HTML directly. | You Can’t directly update HTML |
     | It causes too much of memory wastage | 	There is no memory wastage|
     | Creates a new DOM if element updates | It updates the JSX if element update|


   **[⬆ Back to Top](#table-of-contents)**
    
299. ### How to add Bootstrap to a react application?
     Bootstrap can be added to your React app in a three possible ways
     1. Using the Bootstrap CDN:
        This is the easiest way to add bootstrap. Add both bootstrap CSS and JS resources in a head tag.
     2. Bootstrap as Dependency:
        If you are using a build tool or a module bundler such as Webpack, then this is the preferred option for adding Bootstrap to your React application
        ```javascript
        npm install bootstrap
        ``
     3. React Bootstrap Package:
        In this case, you can add Bootstrap to our React app is by using a package that has rebuilt Bootstrap components to work particularly as React components. Below packages are popular in this category,
        1. react-bootstrap
        2. reactstrap

   **[⬆ Back to Top](#table-of-contents)**
    
300. ### Can you list down top websites or applications using react as front end framework?
     Below are the `top 10 websites` using React as their front-end framework,

     1. Facebook
     2. Uber
     3. Instagram
     4. WhatsApp
     5. Khan Academy
     6. Airbnb
     7. Dropbox
     8. Flipboard
     9. Netflix
     10. PayPal

   **[⬆ Back to Top](#table-of-contents)**
    
301. ### Is it recommended to use CSS In JS technique in React?
     React does not have any opinion about how styles are defined but if you are a beginner then good starting point is to define your styles in a separate *.css file as usual and refer to them using className. This functionality is not part of React but came from third-party libraries. But If you want to try a different approach(CSS-In-JS) then styled-components library is a good option.

   **[⬆ Back to Top](#table-of-contents)**
    
302. ### Do I need to rewrite all my class components with hooks?
     No. But you can try Hooks in a few components(or new components) without rewriting any existing code. Because there are no plans to remove classes in ReactJS.

   **[⬆ Back to Top](#table-of-contents)**
    
303. ### How to fetch data with React Hooks?
     The effect hook called `useEffect` is used to fetch the data with axios from the API and to set the data in the local state of the component with the state hook’s update function.
     Let's take an example in which it fetches list of react articles from the API
     ```javascript
     import React, { useState, useEffect } from 'react';
     import axios from 'axios';

     function App() {
       const [data, setData] = useState({ hits: [] });

       useEffect(async () => {
         const result = await axios(
           'http://hn.algolia.com/api/v1/search?query=react',
         );

         setData(result.data);
       }, []);

       return (
         <ul>
           {data.hits.map(item => (
             <li key={item.objectID}>
               <a href={item.url}>{item.title}</a>
             </li>
           ))}
         </ul>
       );
     }

     export default App;
     ```
     Remember we provided an empty array as second argument to the effect hook to avoid activating it on component updates but only for the mounting of the component. i.e, It fetches only for component mount.

   **[⬆ Back to Top](#table-of-contents)**
    
304. ### Is Hooks cover all use cases for classes?
     Hooks doesn't cover all use cases of classes but there is a plan to add them soon. Currently there are no Hook equivalents to the uncommon **getSnapshotBeforeUpdate** and **componentDidCatch** lifecycles yet.

   **[⬆ Back to Top](#table-of-contents)**
    
305. ### What is the stable release for hooks support?
     React includes a stable implementation of React Hooks in 16.8 release for below packages
     1. React DOM
     2. React DOM Server
     3. React Test Renderer
     4. React Shallow Renderer

   **[⬆ Back to Top](#table-of-contents)**
    
306. ### Why do we use array destructuring (square brackets notation) in `useState`?
     When we declare a state variable with `useState`, it returns a pair — an array with two items. The first item is the current value, and the second is a function that updates the value. Using [0] and [1] to access them is a bit confusing because they have a specific meaning. This is why we use array destructuring instead.
     For example, the array index access would look as follows:
     ```javascript
      var userStateVariable = useState('userProfile'); // Returns an array pair
      var user = userStateVariable[0]; // Access first item
      var setUser = userStateVariable[1]; // Access second item
     ```
     Whereas with array destructuring the variables can be accessed as follows:
     ```javascript
     const [user, setUser] = useState('userProfile');
     ```

     **[⬆ Back to Top](#table-of-contents)**
    
307. ### What are the sources used for introducing hooks?
     Hooks got the ideas from several different sources. Below are some of them,
     1. Previous experiments with functional APIs in the react-future repository
     2. Community experiments with render prop APIs such as Reactions Component
     3. State variables and state cells in DisplayScript.
     4. Subscriptions in Rx.
     5. Reducer components in ReasonReact.

   **[⬆ Back to Top](#table-of-contents)**
    
308. ### How do you access imperative API of web components?
     Web Components often expose an imperative API to implement its functions. You will need to use a **ref** to interact with the DOM node directly if you want to access imperative API of a web component. But if you are using third-party Web Components, the best solution is to write a React component that behaves as a **wrapper** for your Web Component.

   **[⬆ Back to Top](#table-of-contents)**
    
309. ### What is formik?
     Formik is a small react form library that helps you with the three major problems,
     1. Getting values in and out of form state
     2. Validation and error messages
     3. Handling form submission


   **[⬆ Back to Top](#table-of-contents)**
    
310. ### What are typical middleware choices for handling asynchronous calls in Redux?
     Some of the popular middleware choices for handling asynchronous calls in Redux eco system are `Redux Thunk, Redux Promise, Redux Saga`.

   **[⬆ Back to Top](#table-of-contents)**
    
311. ### Is browsers understand JSX code?
     No, browsers can't understand JSX code. You need a transpiler to convert your JSX to regular Javascript that browsers can understand. The most widely used transpiler right now is Babel.

   **[⬆ Back to Top](#table-of-contents)**
    
312. ### Describe about data flow in react?
     React implements one-way reactive data flow using props which reduce boilerplate and is easier to understand than traditional two-way data binding.

   **[⬆ Back to Top](#table-of-contents)**
    
313. ### What is react scripts?
     The `react-scripts` package is a set of scripts from the create-react-app starter pack which helps you kick off projects without configuring. The `react-scripts start` command sets up the development environment and starts a server, as well as hot module reloading.

   **[⬆ Back to Top](#table-of-contents)**
    
314. ### What are the features of create react app?
     Below are the list of some of the features provided by create react app.
     1. React, JSX, ES6, Typescript and Flow syntax support.
     2. Autoprefixed CSS
     3. CSS Reset/Normalize  
     4. A live development server
     5. A fast interactive unit test runner with built-in support for coverage reporting
     6. A build script to bundle JS, CSS, and images for production, with hashes and sourcemaps
     7. An offline-first service worker and a web app manifest, meeting all the Progressive Web App criteria.


   **[⬆ Back to Top](#table-of-contents)**
    
315. ### What is the purpose of renderToNodeStream method?
     The `ReactDOMServer#renderToNodeStream` method is used to generate HTML on the server and send the markup down on the initial request for faster page loads. It also helps search engines to crawl your pages easily for SEO purposes.
     **Note:** Remember this method is not available in the browser but only server.

   **[⬆ Back to Top](#table-of-contents)**
    
316. ### What is MobX?
     MobX is a simple, scalable and battle tested state management solution for applying functional reactive programming (TFRP). For reactJs application, you need to install below packages,
     ```bash
     npm install mobx --save
     npm install mobx-react --save
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
317. ### What are the differences between Redux and MobX?
     Below are the main differences between Redux and MobX,

     | Topic | Redux | MobX |
     | ----- | ------- | ------- 
     | Definition| It is a javascript library for managing the application state | It is a library for reactively managing the state of your applications |
     | Programming | It is mainly written in ES6 | It is written in JavaScript(ES5) |
     | Data Store | There is only one large store exist for data storage | There is more than one store for storage |
     | Usage | Mainly used for large and complex applications | Used for simple applications |
     | Performance | Need to be improved | Provides better performance |
     | How it stores | Uses JS Object to store | Uses observable to store the data |


   **[⬆ Back to Top](#table-of-contents)**
    
318. ### Should I learn ES6 before learning ReactJS?
     No, you don’t have to learn es2015/es6 to learn react. But you may find many resources or React ecosystem uses ES6 extensively. Let's see some of the frequently used ES6 features,
     1. Destructuring: To get props and use them in a component
     ```javascript
     // in es 5
      var someData = this.props.someData
      var dispatch = this.props.dispatch

     // in es6
     const { someData, dispatch } = this.props
     ```
     2. Spread operator: Helps in passing props down into a component
     ```javascript
     // in es 5
     <SomeComponent someData={this.props.someData} dispatch={this.props.dispatch} />

     // in es6
     <SomeComponent {...this.props} />
     ```
     3. Arrow functions: Makes compact syntax
     ```javascript
     // es 5
     var users = usersList.map(function (user) {
      return <li>{user.name}</li>
     })
     // es 6
     const users = usersList.map(user => <li>{user.name}</li>);
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
319. ### What is Concurrent Rendering?
     The Concurrent rendering makes React apps to be more responsive by rendering component trees without blocking the main UI thread. It allows React to interrupt a long-running render to handle a high-priority event. i.e, When you enabled concurrent Mode, React will keep an eye on other tasks that need to be done, and if there's something with a higher priority it will pause what it is currently rendering and let the other task finish first. You can enable this in two ways,
     ```javascript
     // 1. Part of an app by wrapping with ConcurrentMode
     <React.unstable_ConcurrentMode>
       <Something />
     </React.unstable_ConcurrentMode>

     // 2. Whole app using createRoot
     ReactDOM.unstable_createRoot(domNode).render(<App />);
     ```

   **[⬆ Back to Top](#table-of-contents)**
    
320. ### What is the difference between async mode and concurrent mode?
     Both refers the same thing. Previously concurrent Mode being referred to as "Async Mode" by React team. The name has been changed to highlight React’s ability to perform work on different priority levels. So it avoids the confusion from other approaches to Async Rendering.

   **[⬆ Back to Top](#table-of-contents)**
    
321. ### Can I use javascript urls in react16.9?
     Yes, you can use javascript: URLs but it will log a warning in the console. Because URLs starting with javascript: are dangerous by including unsanitized output in a tag like <a href> and create a security hole.
     ```javascript
     const companyProfile = {
       website: "javascript: alert('Your website is hacked')",
     };
     // It will log a warning
     <a href={companyProfile.website}>More details</a>
     ```
     Remember that the future versions will throw an error for javascript URLs.
  
   **[⬆ Back to Top](#table-of-contents)**
   
322. ### What is the purpose of eslint plugin for hooks?
     The ESLint plugin enforces rules of Hooks to avoid bugs. It assumes that any function starting with ”use” and a capital letter right after it is a Hook. In particular, the rule enforces that,
     1. Calls to Hooks are either inside a PascalCase function (assumed to be a component) or another useSomething function (assumed to be a custom Hook).
     2. Hooks are called in the same order on every render.

   **[⬆ Back to Top](#table-of-contents)**

323. ### What is the difference between Imperative and Declarative in React?
     Imagine a simple UI component, such as a "Like" button. When you tap it, it turns blue if it was previously grey, and grey if it was previously blue.

     The imperative way of doing this would be:

     ```javascript
     if( user.likes() ) {
         if( hasBlue() ) {
             removeBlue();
             addGrey();
         } else {
             removeGrey();
             addBlue();
         }
     }
     ```
     Basically, you have to check what is currently on the screen and handle all the changes necessary to redraw it with the current state, including undoing the changes from the previous state. You can imagine how complex this could be in a real-world scenario.

     In contrast, the declarative approach would be:

     ```javascript
     if( this.state.liked ) {
         return <blueLike />;
     } else {
         return <greyLike />;
     }
     ```
     Because the declarative approach separates concerns, this part of it only needs to handle how the UI should look in a sepecific state, and is therefore much simpler to understand.

   **[⬆ Back to Top](#table-of-contents)**

324. ### What are the benefits of using typescript with reactjs?
     Below are some of the benefits of using typescript with Reactjs,
     1. It is possible to use latest JavaScript features
     2. Use of interfaces for complex type definitions
     3. IDEs such as VS Code was made for TypeScript
     4. Avoid bugs with the ease of readability and Validation
