# Interview-Preparation
Personal Interview Preparation for Frontend Position

## 2020-08-21-Fri
https://velog.io/@honeysuckle/%EC%8B%A0%EC%9E%85-%ED%94%84%EB%A1%A0%ED%8A%B8%EC%97%94%EB%93%9C-%EB%A9%B4%EC%A0%91-%EC%A7%88%EB%AC%B8-%EB%AA%A8%EC%9D%8C

위 링크 참조하여 공부

### 렌더링
HTML, CSS, Javascript 등을 화면에 그래픽 형태로 출력하는 것

### 브라우저 렌더링 과정
1. 브라우저는 특정 URI로 request를 보내고 해당 주소의 서버로부터 HTML, CSS 등 데이터를 response로 받음
2. 받은 데이터로 DOM Tree와 CSSOM Tree를 구성함
3. DOM Tree와 CSSOM Tree로 Render Tree를 만듬
4. Viewport에 따른 layout 계산
5. Rendering Tree를 이용하여 브라우저에 그래픽으로 출력

### OOP에 대해 설명
* 프로그래밍을 객체화 하는 것으로 상태와 행위를 가진 객체를의 상호작용을 통하여 프로그래밍하는 방법
* Class: 객체의 상태와 행위 등 형태를 정의하는 것
* Object: Class의 속성을 가진 존재
* Method: 객체의 속성을 조작 또는 객체를 사용
* 장점: 재사용성, 수정의 용이, 유지보수, 가독성이 좋음, 클래스 단위로 모듈화 시켜서 사용할 수 있어 대형 프로젝트에 용이
* 캡슐화: 객체 외부에서 내부 상태를 접근하지 못하게하고 Method를 통해서만 접근 할 수 있도록 함 (getter, setter 이용)
* 추상화: 공통의 특성만 사용하고 불필요한 특성들을 제외시켜주는 것
* 상속: 다른 클래스의 속성과 Method를 가져와 사용할 수 있도록 하는 것
* 오버라이딩: 동일한 이름의 method를 재 정의 하는 것
* 오버로딩: 동일한 이름의 method를 파라미터의 갯수에 따라 다르게 동작하도록 하는 것
