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
2. 브라우저에서 HTML 데이터는 HTML 파서가 파싱하고 CSS 데이터는 CSS 파서가 파싱하여 각각 DOM Tree와 CSSOM Tree를 구성한다
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

CORS(Cross-Origin Resource Sharing)는 무엇인가 왜 이러한 방법이 정의 되었으며,

본인이 코드를 작성하면서 CORS와 관련하여서 경험하였던 이슈는 무엇인가
간단한 데이터를 클라이언트로만 관리 할수 있는가,
이와 관련해서 브라우저 에서 어떠한 것들을 지원하고 있는가,
예를 들면 소셜 로그인같은 것들에 대한 브라우저 종료시 발 생하는 문제에 대응 경험이 있는가

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
- 쿠키는 개수와 용량 제한이 있다 Web Storage는 제한이 없다.
- 쿠키는 만료일자를 지정 하는데 지정하지 않으면 세션쿠키가 된다.
- 영구 쿠키를 저장하려면 만료일자를 굉장히 길게 설정해야하고 Web Storage는 만료일자가 없이 영구적으로 저장된다.
- Web Storage 와 Cookie 모두 도메인 단위로 접근이 제한된다. 다른 도메인에서 저장된 데이터를 엑세스 할 수 없다.
- Local Storage는 windows 전역 객체의 LocalStorage 컬렉션을 통해 저장, 조회된다.
- Session Storage는 windows 전역 객체의 SessionStorage 컬렉션을 통해 저장, 조회된다. (Collections은 값을 저장하는 컨테이너)

### <script> 태그

- Script 태그를 html body 태그의 맨 아래에 위치 시키는 것을 권장하는 이유는 DOM 트리 생성이 완료된 후 DOM 조작을 하기 위함이다. DOM 트리 생성이 완료되지 않았는데 DOM을 조작 할 시 오류가 발생 할 수 있다.

### Javascript 엔진

- 크롬은 자바스크립트 엔진으로 V8 엔진, 렌더링 엔진으로 WebKit을 사용한다.
- 자바스크립트는 싱글 스레드 언어로 한번에 하나의 작업만 처리한다.
- 자바스크립트 엔진은 3개의 영역으로 나누어질 수 있다 ( Call Stack, Event Queue(Task Queue), Heap )
- Call Stack은 프로그램에서 현재의 위치를 기록하는 데이터 구조로 함수를 호출하면 stack의 위에 쌓이고(push) 결과값을 반환하면 스택에서 제거된다(pop)
