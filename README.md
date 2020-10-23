# Interview-Preparation

Personal Interview Preparation for Frontend Position

### 참고 링크

- https://realmojo.tistory.com/300
- https://velog.io/@honeysuckle/%EC%8B%A0%EC%9E%85-%ED%94%84%EB%A1%A0%ED%8A%B8%EC%97%94%EB%93%9C-%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8-%EB%AA%A8%EC%9D%8C
- https://taegon.kim/archives/5770
- https://sunnykim91.tistory.com/121

### 렌더링

HTML, CSS, Javascript 등을 화면에 그래픽 형태로 출력하는 것

### 브라우저 렌더링 과정

1. 브라우저는 특정 URI로 request를 보내고 해당 주소의 서버로부터 HTML, CSS 등 데이터를 response로 받음
2. 브라우저에서 HTML 데이터는 HTML 파서가 파싱하여 DOM Tree를 만든다 CSS는 CSS 파서가 파싱하여 DOM Element와 함께 CSSOM Tree를 구성한다
3. 브라우저 렌더링 엔진은 DOM Tree와 CSSOM Tree로 Render Tree를 만든다
4. Viewport에 따른 layout 계산하고
5. Rendering Tree를 이용하여 브라우저에 그래픽으로 출력한다

참고 링크 : https://d2.naver.com/helloworld/59361

### OOP

- 프로그래밍을 객체화하여, 상태와 행위를 가진 객체들의 상호작용을 통하여 프로그래밍하는 방법
- Class: 객체의 상태와 행위 등 형태를 정의하는 것
- Object: Class의 속성을 가진 존재
- Method: 객체의 속성을 조작 또는 객체를 사용
- 장점: 재사용성, 수정의 용이, 유지보수, 가독성이 좋음, 클래스 단위로 모듈화 시켜서 사용할 수 있어 대형 프로젝트에 용이
- 캡슐화: 객체 외부에서 내부 상태를 접근하지 못하게하고 Method를 통해서만 접근 할 수 있도록 함 (getter, setter 이용)
- 추상화: 공통의 특성만 사용하고 불필요한 특성들을 제외시켜주는 것
- 상속: 다른 클래스의 속성과 Method를 가져와 사용할 수 있도록 하는 것
- 오버라이딩: 동일한 이름의 method를 재 정의 하는 것
- 오버로딩: 동일한 이름의 method를 파라미터의 갯수에 따라 다르게 동작하도록 하는 것

### 함수형 프로그래밍

- 프로그래밍을 하며 재사용하는 기능들을 함수들로 작성하여 부품처럼 함수를 조립하여 사용할 수 있도록 하는 프로그래밍 방법
- 함수형 프로그래밍의 장점은 기능별로 부품을 나누어 관리함으로써 가독성과 수정 및 유지보수에 유리하며 다른 함수의 값을 참조하지 않는 특징이 있어 상태공유로 인한 오류 발생을 방지할 수 있다.
- 순수함수란 입력받는 매개변수 외의 값에 접근하지 않는 함수

### 객체지향 프로그래밍과 함수형 프로그래밍의 차이점

- OOP는 오브젝트가 가진 함수를 호출하는 방식으로 작동하는 반면 FP는 함수를 호출하며 데이터를 매개변수로 입력하는 방식으로 작동
- 고정된 사물이 있다면 객체지향 프로그래밍을 사용하는 것이 유리 그렇지 않다면 오류 방지를 위해 함수형 프로그래밍을 사용

### HOC

- 다른 부품을 매개변수로 받아서 새로운 부품으로 반환하는 것

### 비동기 프로그래밍 (Asynchronous)

- AJAX: 웹페이지 전체를 다시 로딩하지 않고 웹페이지의 일부만을 갱신하여 빠르게 작동할 수 있도록하는 기법
- AJAX 장점: 웹페이지가 로드된 후에도 백그라운드에 서버와 데이터 통신을 할 수 있다

- Promise: 비동기 처리를 도와주는 함수들을 가진 객체
- Promise 작동: 함수가 실행된 후 resolve 함수가 실행된 후에 then 함수로 넘어간다 만약 resolve 함수가 아닌 reject 함수가 실행된다면 catch 함수를 실행한다.
- Promise 장점: Callback 함수 중첩을 방지할 수 있다

- Callback 함수: 동작이 완료된 이후에 실행하는 함수

- Promise와 Callback 차이: Callback은 간편하게 이후 동작을 작성 할 수 있지만 프로그램이 복잡해 지고 동작이 많아질 수로 Promise를 사용하는 것이 가독성에서 유리하다 가독성이 유리함은 유지보수의 유리함으로 이어진다

- Async, Await: 비동기 처리에 사용되는 패턴으로 async 내에서는 await 부분이 완료되어야 이후 프로그램이 작동하도록 되어 비동기 처리를 돕는다.

- 비동기 처리는 서버에서 데이터를 수신 할 때 많이 이용된다 시간이 더 오래걸리는 작업을 비동기 처리함으로써 페이지 로딩의 기다림을 줄일 수 있다.

### SPA (Single Page Application)

- 웹 페이지의 리소스를 최초에 모두 받아오고 새로운 페이지 구동시에 필요한 부분만 갱신하는 방식
- 장단점: 초기 구동 속도가 느린 대신 이후 작동 속도가 빠르다

### 자바스크립트의 Data Type 7가지

- Primitive Data Type: Number, String, Boolean, Null, Undefined, Symbol
- Object Data Type: Object
- Symbol은 새로 추가된 것으로 유일한 식별자를 생성할 때 사용

### Hoisting & Closure

- Hoisting:
  변수나 함수 선언을 코드의 가장 상단으로 올려주어 실행이 선언보다 먼저 위치하더라도 정상 작동하도록 하는 것
  실제로 코드가 끌어올려지는 것은 아니나 자바스크립트 파서가 내부적으로 끌어올려 파싱함
  변수에 할당한 함수 표현식은 호이스팅 적용되지 않음
  예) var myFuc = function() { console.log('Hello'); } // 호이스팅 적용 X
  변수가 함수보다 더 높게 호이스팅된다

- Closure:
  Lexical Scope인 자바스크립트는 함수가 선언되어질 때 Scope가 정해지므로 외부함수와 내부함수가 있을 때 외부함수가 선언될때 외부함수의 변수를 참조했다면 외부함수의 실행이 종료되어도 내부함수에서 외부 함수의 값에 접근 할 수 있는 것
  클로저를 사용하면 변수를 private하게 은닉하여 외부에서 변수에 접근 할 수 없게 할 수 있다
  클로저를 생성해놓고 참조를 제거하지 않으면 메모리가 들기 때문에 클로저 사용이 끝나면 참조를 제거하는 것이 좋다
  클로저에 대한 좋은 설명 사용 예 : https://hyunseob.github.io/2016/08/30/javascript-closure/

### Lexical Scoping & Dynamic Scoping

- Lexical Scoping: 함수의 선언에 따라 scope가 결정 되는 것
- Dynamic Scoping: 함수의 호출에 따라 scope가 결정 되는 것
  자바스크립트는 Lexical Scoping

### Execution Context

- 실행가능한 코드를 형상화하고 구분하는 추상적인 개념
- 실행 루틴을 stack 형태로 형상화 한 것

### this, call, apply, bind

- this는 호출하는 주체를 의미
- call, apply, bind는 Function.Prototype으로 부터 물려받은 method로 모든 함수에서 실행 가능한 method이다
- call, apply, bind를 통해 함수가 실행되어지는 this를 선택, 변경 할 수 있다
- bind는 호출하지 않고 this만 변경
- call, apply는 호출, 둘의 매개변수 받는 형식이 살짝 다름

### ES6

- ECMA Script 6 는 자바스크립트 표준
- Babel = Transpiler
- 브라우저에서 최신 ES6 문법을 지원하지 않을 때 이전 버전의 문법으로 transpile 해주는 babel을 이용하여 호환 되도록 할 수 있다
- ES6 새롭게 추가된 것 (let, const, rest parameter, class, arrow function...)
  - let & const: let은 mutable하여 재선언, 재할당이 가능하지만, const로 선언된 변수는 immutable하여 재선언, 재할당이 불가능하다는 차이점이 있다
  - var와 let, const의 차이: var는 function scope를 가지고 있고 hoisting되고 let, const는 block scope를 가지고 있고 hoisting되지 않는다
  - rest parameter: ...을 변수 앞에 붙여서 parameter로 전달된 매개변수들을 배열 형태로 전달 받는다
  - class: 객체 형태의 함수
  - arrow function: 일반함수보다 간결하고, 자신을 포함하는 외부 scope로 부터 this 받아온다

### RESTful API

- REST 아키텍쳐 스타일을 따르는 API (Representational State Transfer)
- 서버와 클라이언트의 통신 방식 중 하나 (HTTP 프로토콜을 활용)
- URI로 자원을 나타내고 HTTP Method(GET, POST, PUT, DELETE)로 CRUD(Create, Read, Use, Delete) 작업을 수행하는 방식으로 구현된 API
- 서버에서 REST API를 사용하면 클라이언트는 유저와 관련된 사용자 인증이나 context 처리 등을 하기 때문에 클라이언트와 서버가 하는 일이 보다 명확하게 나누어져 개발 시에 서로간의 의존성이 줄어든다. 서버와 클라이언트 개발이 독립적으로 이루어질 수 있다.
- HTTP 프로토콜을 사용하기 때문에 별도의 인프라가 필요하지 않다는 장점
- REST API를 따르면 행위와 자원이 표현되기 때문에 의도를 파악하기가 쉽다. (특징 : Self Descriptiveness)
- REST의 특징 Uniform Interface는 URI로 지정한 리소스에 대한 조작을 통일되고 한정적인 인터페이스로 수행하는 아키텍쳐 스타일

### REST의 구성

- 자원 (Resource) - URI
- 행위 (Verb) - HTTP Method
- 표현 (Representation) - JSON, XML, TEXT, RSS 등

### API

- 프로그램과 또 다른 프로그램을 이어주는 매개체

### 보안, HTTP 통신

- 개발자 도구 콘솔로 인한 보안의 위협
- xss(Cross site scripting) 게시판 등에 자바스크립트 코드를 삽입해 정상적인 작동이 아닌 작동을 수행하도록 하는 것
- xss를 찾아내서 해당 response를 필터링하는 xss 보호 방법이 있음
- Wireshark는 네트워크 패킷을 분석하는 프로그램
- HTTP 통신은 서버와 클라이언트 간의 데이터 전송 프로토콜
- HTTP 통신의 문제점: 정보를 주고 받는 경우 정보 유출의 위험
- HTTPS는 SSL(TLS)라는 전송시 보안 프로토콜이 추가되어 더 안전 (HTTPS는 SEO 측면에서 더 좋기 때문에 더 많이 사용되어짐)

### CORS

- CORS(Cross-Origin Resource Sharing)는 서버에서 외부의 요청을 허용 할 경우 외부 도메인으로 AJAX 요청을 가능하게 하는 정책
- 다른 도메인에 리소스를 요청 할 경우 Cross Origin HTTP를 이용한다.
- 대부분의 브라우저들은 보안의 이유로 Cross Origin HTTP 요청을 제한한다. 이것을 Same Origin Policy라고 한다.
- Same Origin Policy에 따르면 프로토콜과 PORT가 같아야 한다.
- Cross Origin HTTP 헤더를 추가하여 타도메인간의 Cross Origin Resource Sharing을 허용 할 수 있다

### HTTP

- 서버와 클라이언트의 데이터 전송 프로토콜 (request, response로 데이터 전송)
- 캐시 기능을 이용하여 데이터를 저장해서 서버에 요청을 보내지 않고 저장된 데이터를 재사용 할 수 있다. 웹의 트래픽과 성능을 개선 할 수 있다.

### GET & POST

GET과 POST 메소드는 HTTP 메소드 중 가장 많이 사용됨

- GET 은 특정 리소스로부터 Data를 Request 할 때 사용
- POST 는 서버로 Data를 보내 Create, Update 할 때 사용

### Web Storage(Session & Local Storage) & Cookie

### 브라우저 저장소

- Web Storage는 문자열 뿐만 아니라 객체도 저장 가능하고, 클라이언트에서 서버로 보내는 모든 웹 요청에 함께 전송되는 쿠키와는 다르게 요청과 함께 보내지지 않아 네트워크 트래픽을 줄여준다. (Key, Value 형태로 저장)
- 쿠키는 개수와 용량 제한(4KB)이 있다 Web Storage는 제한이 없다.
- 쿠키는 만료일자를 지정 하는데 지정하지 않으면 세션쿠키가 된다.
- 영구 쿠키를 저장하려면 만료일자를 굉장히 길게 설정해야하고 Web Storage는 만료일자가 없이 영구적으로 저장된다.
- Web Storage 와 Cookie 모두 도메인 단위로 접근이 제한된다. 다른 도메인에서 저장된 데이터를 엑세스 할 수 없다.
- Local Storage는 windows 전역 객체의 LocalStorage 컬렉션을 통해 저장, 조회된다.
- Session Storage는 windows 전역 객체의 SessionStorage 컬렉션을 통해 저장, 조회된다. (Collections은 값을 저장하는 컨테이너)

### <script> 태그

- Script 태그를 html body 태그의 맨 아래에 위치 시키는 것을 권장하는 이유는 DOM 트리 생성이 완료된 후 DOM 조작을 하기 위함이다. DOM 트리 생성이 완료되지 않았는데 DOM을 조작 할 시 오류가 발생 할 수 있다.
- Script 태그를 상단에 위치하여도 defer속성을 이용하면 html 구문 분석 후 DOM 트리 구축이 완료된 후에 script 태그를 실행한다
- async 속성은 스크립트를 다운로드 하는 중에도 html 구문 분석을 할 수 있도록 해준다
- defer나 async를 이용하거나 body 태그의 맨 하단으로 script 태그를 위치시키는 것으로 빈화면 로딩 시간을 줄여 줄 수 있다.
- defer 와 async은 둘 다 비동기 적으로 script를 다운 받을 동안 동시에 html 파싱을 하게 된다. 차이점은 async는 다운로드 완료후 html 파싱을 멈추고 script를 실행하는 반면 defer는 script 다운이 완료되었더라도 html 파싱 완료를 기다린 후 script 실행을 한다.

### Javascript 엔진

- 크롬은 자바스크립트 엔진으로 V8 엔진, 렌더링 엔진으로 WebKit을 사용한다.
- 자바스크립트는 싱글 스레드 언어로 한번에 하나의 작업만 처리한다.
- 자바스크립트 엔진은 2개의 영역으로 나누어질 수 있다 ( Call Stack, Memory Heap ) / Event Queue(Task Queue) 는 브라우저 내부의 다른 영역이고 자바스크립트 V8 안에 존재하지는 않는다
- Call Stack은 프로그램에서 실행 중인 코드를 트래킹하는 데이터 구조로 함수를 호출하면 stack의 위에 쌓이고(push) 결과값을 반환하면 스택에서 제거된다(pop)
- Memory Heap은 동적으로 생성된 객체(변수, 함수)가 메모리에 할당되는 곳이다
- 자바스크립트는 하나의 Call Stack만을 가지고 있는데 이것의 문제점은 함수가 실행될 때 다른 함수를 실행 할 수 없다는 것인데 이것을 해결하기 위해 나중에 실행하는 Callback 함수를 사용한다. 비동기 Callback은 Call Stack에 바로 쌓이지 않고 Event Queue에 저장되었다가 Call stack이 비었을 때 실행된다.
- Event Queue는 Callback Event Queue라고도 불린다.
- Event Loop는 Call Stack과 Callback Event Queue의 상태를 확인하면서 Call Stack이 비면 Event Queue에서 하나씩 꺼내서 동작시키는 Loop이다. (Callback을 꺼내 동작시키는 것을 tick이라고 한다)
- Event Loop를 통해서 동시성(Concurrency)을 지원한다. (Event Loop는 브라우저의 구성요소 중 하나인 것 같다)
- Call Stack의 한정된 자원 용량이 넘치는 것을 Stack Overflow라고 한다
- Call Stack에 쌓인 작업들 중 시간이 오래 걸리는 작업은 완료 될 때까지 기다려야하는데 이를 Blocking이라고 한다
- javascript가 싱글 스레드임에도 웹사이트를 끊김 없이 사용 할 수 있는 이유는 asynchronous callback을 사용하기 때문
- setTimeout은 callstack에서 쌓엿다가 실행되면서 pop되고 Web APIs에서 timer 실행이 완료된 후 callback queue에 적재되고 call stack이 비었다면 event loop를 통해 call stack으로 tick 되어서 setTimeout 내부에 작성하였던 동작이 실행된다 (AJAX나 DOM 이벤트도 동일하게 Web API로 보내져서 작동한다)

### 가비지 컬렉터 (GC)

- 프로그램에서 동적으로 할당되었던 메모리 중 필요없어진 영역을 할당 해제시키는 기능
- 객체를 참조하는 대상이 하나도 없을 경우 가비지 컬렉션 대상으로 여기고 메모리에서 해제시킨다
- 클로저를 만들고 메모리 해제를 하지 않으면 메모리 누수 발생 (null 할당으로 해제 시킨다)

### Web Worker (웹 워커)

- 자바스크립트는 single thread로 동작하지만 web worker를 사용하면 multi thread를 활용 할 수 있다
- 시간이 오래 걸리는 연산 작업이 있을 경우 web worker에게 작업을 맡기고 메인 thread는 다른 작업을 수행하다가 web worker의 작업이 끝나면 DOM Update를 해주면 ui 클릭과 같은 동작을 연산 수행 중 할 수 있게 된다.
- web worker는 직접 DOM에 접근 할 수 없기 때문에 메인 thread와 메시를 주고 받아 통신한다
- CPU가 코어가 여러개여야 Web worker를 사용 할 수 있다
- 빅데이터 처리, 게임 개발 시에 사용 효과가 좋다

### Service Worker (서비스 워커)

- 주기적 백그라운드 동기화 및 푸시 알림 등 오프라인 웹 경험을 향상시킨다
- 브라우저가 백그라운드에서 실행시킨다
- 개발 중에 localhost를 사용 할 수 있지만 배포시 HTTPS에서만 등록되어 작동한다. HTTP에서는 작동하지 않는다
- PWA 개발 시에 사용

### Web APIs

- setTimeOut
- DOM Event 예: document.querySelector('button')와 같은 DOM 조작 이벤트
- AJAX : 브라우저가 가지고 있는 XmlHttpRequest 객체를 이용하여 전체 페이지를 새로고침하지 않고도 페이지의 일부만을 위한 데이터를 로드하는 기법, 자바스크립트의 비동기 통신, 서버와 클라이언트 간의 XML 데이터를 주고 받는다. (자바스크립트로 서버에 데이터 요청하는 것)
- 스크롤 같은 이벤트는 작은 동작에도 쉽게 발생하는데 이와 같은 이벤트가 너무 많이 callback queue에 쌓이게 되면 프로그램 성능에 영향을 주기 때문에 디바운싱(deboucing)을 통해서 이벤트가 큐에 쌓이는 속도를 느리게 조절하여 개선 할 수 있다
- 자바스크립트가 싱글 스레드임에도 멀티 스레드 처럼 작동 할 수 있는 이유 브라우저에 Web APIs와 Callback Event Queue가 있기 때문

### AJAX

- 비동기 방식을 사용하여 페이지를 리로드 할 때 이미지 텍스트 등 전체 리소스를 다시 불러오지 않고 필요한 부분만 요청하여 성능적으로 큰 장점이 있다.
- 클라이언트에서 서버로 데이터를 요청하고 결과를 받을 수 있다
- WEB 화면에서 페이지 전체를 새로고침하지 않고 부분적으로 데이터를 받아 올 때 사용할수있다
- XMLHttpRequest 객체를 통해 JSON이나 XML 데이터를 서버로부터 받아올수있다
- 웹페이지 속도 향상
- 다른 도메인과는 통신이 불가능 하다
- 사용법: XMLHttpRequest 객체 생성 후 url을 통해 요청하고 응답을 받으면 callback 함수로 응답 처리 (이 과정이 코드가 길어지는데 JQuery를 이용하여 더 간단한 코드로 작성 할 수 있다)

### 이벤트 버블링

- 이벤트 버블링은 하위 Element에서 상위 Element로 이벤트를 전달하는 것
- 이벤트 캡쳐는 이벤트가 발생했을때 상위 Element에서부터 해당 Element를 찾아내려가는 것
- event.stopPropogation() 함수를 사용하면 상위 Element로 이벤트를 전달하지 않고 해당 Element 이벤트만 실행 후에 멈춘다
- 이벤트 위임(Event Delegation)는 하위 요소에 이벤트를 붙이지 않고 상위 요소에서 하위 요소들의 이벤트를 관리하도록 하는 것

### SSR & CSR

- SSR은 서버사이드 렌더링의 약자로 요청시마다 새로고침이 일어나며 새로운 페이지를 서버에 요청하는 것
- CSR: Client Side Rendering
- SPA: Single Page Application (일반적인 컴퓨터보다 성능이 낮은 모바일 환경에 적합한 방식, 최초 한번 페이지를 전체 로딩 한 후 데이터만 변경하여 사용하는 앱), SSR에 비해 트래픽 감소, 서버는 JSON만 보내주며 클라이언트에서 자바스크립트가 html을 그리는 역할 수행 -> 이것이 Client Side Rendering
- 서버사이드렌더링은 뷰를 서버에서 렌더링하기때문에 첫 로딩이 빠르다
- SEO의 문제 (검색엔진최적화의 문제): 대부분의 웹 크롤러는 자바스크립트를 해석 할 수 없다. 자바스크립트로 이루어진 CSR을 해석하지 못하는 경우가 발생

### CSS Preprocessor

- 규모가 커져서 CSS를 관리하기 어려울 경우 CSS Preprocessor를 많이 사용한다 (Sass, Less, SCSS 등)
- CSS 전처리기를 사용하면 nesting이나 반복문 등 간단한 연산을 사용 할 수 있다는 장점이 있다
- 웹에서는 CSS만 동작하기 때문에 CSS로 바꿔주는 컴파일 과정을 거쳐야 한다

### use strict

- 자바스크립트를 해석 할 때 더 엄격한 규칙을 따르도록 함으로써 에러 발생을 좀 더 감소시킨다

### MVC

- Model, View, Controller
- model은 데이터를 가지고 있고 controller는 모델로부터 데이터를 가져와서 view를 통해 화면에 표시한다
- 각각 독립된 역할들만 수행하게 하여 유지보수에도 유리한 코드로 개발 할 수 있다

### Cross Browsing

- 웹페이지를 개발 할 때 모든 브라우저에서 호환되도록 하는 것

### Progressive Rendering

- 페이지 구성 요소의 표시 순서 우선 순위를 정한다.
- Lazy Loading : 자바스크립트를 이용하여 사용자가 스크롤 시에 필요한 부분을 로드

### 다국어 페이지 제공 방식

- SSR의 경우 클라이언트에서 서버로 HTTP를 보낼 때 Accepted-Language 헤더를 통하여 기본언어 설정 정보 보냄, 서버는 이 정보로 클라이언트에 해당 언어로 보내줌
- CSR는 해당 브라우저의 언어 설정을 가져와서 보여줌

### SEO

- 검색엔진이 자료를 수집하고 순위를 매기는 방식에 맞게 웹페이지를 구성하여 검색 시 상단에 보여지도록 하는 것
- SPA의 경우 CSR이기 때문에 SEO에서 불리 할 수 있음

### section과 article 태그 차이

- section은 비슷한 특성의 컨텐츠를 담는 구역을 설정
- article은 서로 관련이 없고 독립적인 내용을 담을 때 사용

### HTML5 태그

- <!DOCTYPE html> 브라우저에게 문서 형식을 알려준다
- 필수 태그 html head body
- meta 태그는 검색 엔진이 읽을 수 있는 태그이며 문서 설명에도 사용된다. 화면에 표시되어지는 것은 없다

### Semantic 태그

- 자신의 역할이나 의미를 개발자나 브라우저에게 표시하는 태그

### Box Model

- Content, padding, Border, Margin을 그림으로 나타낸 것

### Flexbox

- 레이아웃을 편하게 잡기 위한 CSS 속성
- 컨테이너와 아이템 구성으로 레이아웃을 지정한다

### ES6

- ES6에서 바뀐 것 Template Literal, Spread Operator, 화살표 함수, Class

### Babel

- 버전이 다른 자바스크립트 표준을 transpile 해준다

### Array & Linked List

- Array는 Random Access를 지원, Linked List는 Sequential Access를 지원
- 배열은 stack, linked list는 heap 영역에 저장된다

### Stack & Queue

- Stack LILO, Queue FIFO

### Binary Search Tree

- 이진 트리와 연결리스트의 결합으로 왼쪽에서부터 가장 작은 숫자로 정렬되어있다

### 프레임워크와 라이브러리의 차이
프레임워크는 정해진 골격안에서 원하는 기능을 구현
라이브러리는 따로 정해진 골격이 없고 필요한 기능에 따라서 골라 사용할 수 있다.

### 리액트 소개하기
- 페이스북에서 만든 자바스크립트 라이브러리 중 하나로 넷플릭스 에어비앤비 인스타그램에서도 사용되어지고 있다
- 리액트는 유저 인터페이스를 만들 때 사용하는 라이브러리
- 리액트는 라이브러리여서 도구처럼 사용하여 다른 라이브러리와 결합 가능
- 리액트는 MVC 패턴에서 사용자에게 보여지는 View 부분을 담당
- 사용자에게 UI를 보여주고 이벤트를 처리하는 역할을 함
- 모바일 환경의 리액트 네이티브, 일렉트론을 이용하면데스크톱 애플리케이션을 만들 수 있어서 다방면으로 사용 가능

### 시멘틱 마크업
- Semantic Tag들은 컨텐츠의 의미를 나타낸다
- 검색엔진, 스크린 리더, 개발자들이 이해하기 쉬워진다
- 스크린 리더: 시각 장애를 가지신 분들에게 내요을 음성으로 전달, 시멘틱 마크업을 적용하면 내용을 더 효과적으로 전달 할 수 있다
- div는 최대한 컨텐츠를 그룹화하는 용도로 사용하고 시멘틱 태크를 이용하려 노력하여 Semantic Web을 만들려고 하는 것이 좋다

### 프론트엔드 개발자에게 중요한 것
- 개발 스킬, 미적 감각, 툴과 기술에 대한 이해
- HTML, CSS
- 유의해야하는 점: 접근성(이용자 친화적으로 각 기기에서 최적화되어진 동적인 사이트 개발을 고려), 검색 엔진 최적화에 대한 고려

### CMS
- Content Management System -> Content Management Application(내용 관리 애플리케이션), Content Dispatch Application(내용 배포 애플리케이션)
- CMA: HTML에 들어갈 내용 관리 (변경, 제거 등)
- CDA: 웹 사이트의 모든 수치를 보고 편집할 수 있는 정보편집 프로그램 ex)형식 관리, 계정 제어, 데이터 색인,탐색, 키워드 컴색

### 라이브러리 선택시 고려할것들
### 번들러란
https://wormwlrm.github.io/2020/08/12/History-of-JavaScript-Modules-and-Bundlers.html
### 더이상 번들러를 사용하지 않는 이유
https://d2.naver.com/helloworld/4268738
### 이벤트 캡쳐링 사용방법
### 이벤트 버블링 멈추는 
