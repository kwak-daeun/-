# 공부기록

## Spring MVC (Model, View, Controller)

### Spring MVC?

* Model / View / Controller 역할
* MVC 패턴의 목적은 Business Logic과 Presentation Logic을 분리하는 것이다.
  * Business Logic : 어떤 특정한 값을 얻기 위해 데이터 처리를 수행하는 응용프로그램의 일부(원하는 값을 얻기 위해 백엔드에서 일어나는 각종 처리)
  * Presentation Logic : 화면상의 디자인 구상을 위한 처리 (화면을 보여주기 위한 처리)
 * 역할별로 코드를 분리하여 하나의 파일에 코드가 모이는 것을 방지하기 때문에, 가독성과 코드 재사용이 증가한다.
 * 단점으로 View와 Model 사이의 높은 의존성 때문에 어플리케이이 커질수록 복잡해지고 유지보수가 어렵다.
 
 ### Model
 * Controller에서 View로 전달되는 데이터 객체이다.
 * Key-Value 형태를 가지며, 하나의(key-value)객체를 Model Attribute라고 한다.
 
 ### Controller
 * View와 Model 사이의 인터페이스 역할을 수행한다.
 * Request에따라 적절한 결과를 Model에 담아 View에 전달한다.
    (즉, View Name과 View에 출력할 Model을 반환한다.)
    
 ### View
 * Model 데이터 렌더링을 담당하여, HTML, Output을 생성한다.
 * 여러가지 템플 엔진이 존재한다.(ex. JSP, Thymleaf ...) 
