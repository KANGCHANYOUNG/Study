# Study
#  21/06/07/html/css

&lt;는 <를 의미,  &gt; > 
조건문은 기본적인 메커니즘은 자바와 동일
리팩토링이란 비효울적인 코드를 효율적으로 만들어서 가독성을 높이고 유지보수가 쉽도록 만드는 것이다.
id는 하나의 태그에만 적용될 수 있으므로 새롭게 만들어진 버튼에는 새로운 id값을 적용해줘야 한다.  

배열 
var fruits = ["apple", "banana"]; 
document.write(fruits[0]); 배열 값 접근
document.write(fruits.length); 배열 길이 
fruits.push("coconut"); 배열에 값 추가 (맨뒤에)

document.write('<li>1</li>');
var i = 0;
while (i < 3) {
  document.write('<li>2</li>');
  document.write('<li>3</li>');
  i = i + 1;
}
document.write('<li>4</li>');


#  21/06/07 수업
 
xxx.jsp - ui/ux - view 계층(넥,Flex)
가급적 java로 구현해야 재사용성과 단위테스트에 유용하며 독립성이 강한 형태로 나아갈 수 있게 만든다.
jsp가 되기 위해선 <%@apge%>가 기본이 되여야 하며 <head>부분에 css,js, jquery가 와야 한다. 공통 코드도 있어야 하며(include)로 있어야 한다.
본문은 body 태그에서 진행이 되며 처리가 되기 위해선 DOM Tree가 완성이 되어야 한다. $(document).ready(function) {}); 이걸 작성했을 떄 Dom Tree작성과 일치
$를 쓴다는거 자체가 jquery를 기반으로 실습을 한다고 생각하면 된다. 문서를 작성할때 document.write함수가 있다. document가 가르키는건 html문서 자체를 가르키는 함수이다.
document.write("tag") 
html문서 인터프리터 (기준) who? api에 따라 맞춰 나가야 한다. 
 
Front Controller xxx.jsp HttpServelt 
                 xxx.nhn DippatcherServlet"
표준 서블릿은 의존적이며 spring boot은 의존적이지 않다. ->파라미터를 통해서 확인가능하고 req,res가 있어야만 응답페이지를 처리할 수 있다면 그것은 의존적이다. 
 의존적이라는 것은 프레임워크 사상에 위배되며 독립적이지 않다.(단위,통합 테스트, 팀플 영역에대한 독립성) 
[Forward의 단점]
* URL이 클라이언트 어플리케이션과 항상 일치하지 않음
* 브라우저의 Refresh 버튼을 누를경우 정확하지 않은 요청이 발생할 수 있음
* 이미지 상대경로 지정시 문제가 될 수 있음

[Forward의 장점]
* 서버에서 처리되므로 Redirect보다 더 나은 성능
* 요청 Scope에 저장되어 있는 객체를 프리젠테이션 컴포넌트에 쉽게 이용가능 
 
 




3교시 

![2](https://user-images.githubusercontent.com/78460496/120951889-dc443480-c784-11eb-889f-6b28b04f1066.JPG)

![3](https://user-images.githubusercontent.com/78460496/120952461-0ba77100-c786-11eb-9d5c-cbe28ab05951.JPG)


Dom에 대한 생성, 시점이 우리가 얘기하는  Lifecycle이 연관이 있다. 
함수는 괄호로 생성하고 세미콜론은 생략하면 된다. 이런것들이 이제 내부에 올 수도 있고 외부에 있는 함수를 호출 할 수 있다.
아까 test2 undefined 같은 오류들을 조심해야 한다. easy ui를 쓸 때는 jQuery기반이고 직접접근이 아니라 $표시를 이용해 접근한다.
$(document).ready(function({ --> 익명 함수이다. 
});     
$("# dg_emp").datagrid(); -> 생성자
js기반은 기본적으로 오브젝트가 들어가 있다.

![4](https://user-images.githubusercontent.com/78460496/120952503-24b02200-c786-11eb-80db-e3a06089a0d5.JPG)


btn.addActionListener(new ActionListenenr({    @Override이다. 예외
 public void actionPerformed(Action a)
});
자바 스크립트 조건문 

 prompt() 함수 
 - 문자열을 입력할 때 사용

- 숫자를 입력 받아야 하는 경우는 문자열로 입력 받은 뒤 변환

- 첫번째 매개변수는 입력 창에서 띄워줄 메시지

- 두번째 매개변수는 입력 부분의 기본 값
06/06에서 알 수 있듯이 script태그를 사용하면 html내부에서 자바스크립트를 사용할 수 있다.
조건문 메커니즘은 자바와 비슷하나 변수선언에는 기본적으로 const를 사용하고, 재할당이 필요한 경우에 한정해 let 을 사용하는 것이 좋다.
---------
표준을 지키는 코딩을 할때는 선언부에 `use strict` let x = " "; 를 사용하는 것이 좋지만  외부 api를 사용하기엔 안좋다.

new String(") match, search lastIndexOf, SubString(1,3)
---------------------
새글 - list 댓글 - read   bm_no 채번 bm_post 차수 bm_step 글순번
 ui/ux (약속) -> 안전
메인, 팝업
결과처리(확인), 입력(수정), 비번입력, 목록 이런 것들을 고려해서 어떻게 처리할지 정해봐야한다.

상세받기
 답글쓰기 /수정/삭제/목록/ 
 writeForm#2 
-----------------------
HashMapBinder --> com.util --> spring지원 ->F/W ->프로시저 
-> json / 출력 (out.print()) <%=%>  --> document.write() --> Front -End
개발 패턴 action -> jsp,  jsp -> action ->jsp
 git 관리 
 
 
 




#  21/06/06 html/css/js 
1. Script 태그

HTML의 태그 중 하나인 script 태그 안에는 Javascript 코드를 쓸 수 있다.
<body>
  <script>
    document.write('hello, world!');
  </script>
</body>

하지만 자바 스크립트로 쓴 코드는 동적이고 html은 정적이다 1+1일 경우 자바스크립트는 연산후 2를 출력하지만 html은 1+1을 그대로 출력한다.

2. 이벤트(on Click)
<input type="button" value="hi" onclick="alert('hi')">

HTML 태그안에서 onclick 속성은 javascript 코드를 가지게 된다. onclick이 포함된 태그가 클릭되었을 떄 이 javascript코드에 따라서 웹 브라우저가
동작하는건데 위에 코드에서 웹브라우저는 alrer("hi")라는 코드를 기억하고 있다가, 사용자가 클릭하면 이를 실행해준다. 
이렇게 웹브라우저에서 일어난 사건을 이벤트(event)라고한다.
 <input type="text" onchange="alert('changed')"> input type=> 웹브라우저에 띄우는 화면? on이 붙은것들 event라고 생각해서 사용자와 상호 작용가능하게 만듬
 3. Console
Console창에 alert("생각해보기") 쓰고 엔터 누르면 경고창이 뜬다.

4. 변수와 대입 연산자 
var word ="hello"  => 변수 이름 앞에 var을 붙이면 좋다. 요즘 트렌드는 const를 넣어준다.

5. 웹 브라우저 backgroundcolor , 글씨 색깔 변경
  <body style="background-color: blue; color: gray;">
단순히 <body> 태그만 쓰는게 아닌   <body style="background-color: blue; color: gray;">
이런식으로 <body> 태그에서 두번 째 줄과 같이 style을 지정해주면 바뀐다. style 속성에 있 는 간단한 코드를 css라고 부르며 
  css은 디자인을 위한 언어이며 자바 스크립트랑 완전히 다른 언어이다..
 하지만 HTML은 한 번 표시되면 바뀌지 않는 정적인 언어이다. 즉 <body>  태그가 만들어지면, 저 style 속성  값을 바꿀 수 없다.

6.css 기본 + 선택자
css를 이용하면 웹페이지에 있는 요소들의 디자인을 바꿀 수 있 는데 이를 위해서는 바꾸고 싶은 태그에 style속성을 사용하면 된다. <!-- (<h1>Javascript<h1> -->
이렇게 하면 Javascript라는 글자가 나타나게 되는데 이때 글자의 색을 blue로 바꾸고 싶다면 다음과 같이 써주면 된다.
<!-- <h1 style="color:blue">Javascript<h1> -->
이때 이 color:blue라는 코드가 바로 css입니다.
index.css => import를 먼저 head에 박아준다. <link rel="stylesheet" href="index.css"> 
css 내부에서 element를 만들때 해당 태그일때는 태그 이름만 선언 ex) h1{} ""일떄는 #을 붙인다.   <section id="hello">
일 경우 #hello{} 클래스일 경우 . 을 붙혀준다. class는 중복될 수 있지만, id는 한 페이지에서는 딱 한번만 쓰이게 되는 것입니다.  
  id > class > 태그 
 
7.제어할 태그를 선택할 때 사용할거 querySelector
위에서 배운 내용은 이벤트와 페이지의 스타일일 바꾸는걸 배웠다. 이둘을 조합해서 어떤 이벤트가 발생했을 때 페이지의 스타일을 바꾸는 기능을 구현해야한다. 즉 이벤트가 발생했을 때 어떤 태그에 스타일이 지정될지 선택하는 작업이 필요하다.
documnet.querySelector("body") 이 코드는 페이지 내에서 body라는 이름의 태그를 모두 선택하는 것이다. 만약 js라는 class를 가진 태그를 선택하고 싶다면 따옴표 사이에 .js를 쓰면 되고, first라는 id를 가진 태그를 선택하고 싶다면 #first라고 쓰면 된다.  실제 예시다.
 document.querytSelector("body").style.backgroundColor='black'; => body 태그를 모두 고른 뒤, 여기에 스타일 을 적용하기 위해서
  style이라고 써 주고, 여러 스타일 중에서도 배경색을 지정하기 위해서 backgroundColor라고 써 준것 입니다.
이렇게 완성한 Javascript 코드를 이벤트가 일어날 때마다 실행하면 되는 것 이다. 예를 들어서 버튼을 클릭할 때 이러한 스타일 변화가 일어나도록 만드러면
 다음과 같다. 
<input type="button" value="night" onclick="document.querySelector('body').style.backgroundColor='black';">
  
  





    

#  21/06/05/넥사크로 보충
 
 이클립스 프로젝트 생성

이클립스 프로젝트 생성

1. spring4_1_1을 복사후 이름 지정후 생성
2. import후 톰캣 서버 환경설정(Web Modules ==> / )
3. jar파일 넣기 

---------------------------------jar파일 확인
![jar](https://user-images.githubusercontent.com/78460496/120917445-5378ba80-c6ea-11eb-8ebd-2677dc2b0cd1.JPG)




-----------------------------넥사크로 이클립스 연동 환경설정
1 넥사크로 프로젝트 생성   file --> new --> project

2. Project 이름 밑에 있는 TypeDefinition --> service --> User Service에서 + 버튼 누른후 
PrefixID에 SvcURL , Type은 JSP, URL은 http://localhost:자기톰캣PORT번호/     

3. TOOLS -- > OPTIONS -> Project밑에 Generate에서 Generate Path  경로는 
연결하고자 하는 이클립스 프로젝트 WebContent로 지정한다. 

3-1. Select the browser 체크 박스에서 크롬을 제외하고 다 비활성화 

 

 



강사님 설명==>
http://docs.tobesoft.com/nexacro_17_ko  ==> 넥사크로 api  (help)
PPT 4.화면 개발 실습 부분에서 디비 연동에 대한 설명이 들어가있다.
4.4.5에 JSP 관련 
PPT 6.메인 화면 구성은 전체 페이지를 어떻게 구성해야 하는가 설명
SDI어플리케이션 -> 싱글
6번은 메인에 대한 디자인 5번은 팝업창 4번은 페이지 처리 순서라고 보면 된다.
empManager 에서 grid -> dataset으로 row column을 넣고 정할수 있다. source에서도 넣는게 가능하다.

C:\Users\user\Documents\nexacro\17.1\projects\nexacro17_Education_Materials\Sample\EduProject ==> 소스 모음
Form_EmpMLM, Form_Organization 좋은 예시소스  html에는 없는 bind component를 ui툴에서는 사용이 가능
항상 service에서 port맞춰주는것을 잊지 않아아 한다. 

nexa source 설명 정리
  talbe tag에 해당 되는것은 ==> grid
  
  html에 json에 해당하는것은 ==> dataset 
  
  그 두개를 바인딩 처리하는것이 binddataset="ds_emp"
  
  자바 쪽 코드로 작성할 떄는 DataSet ds_emp = new DataSet();왜냐하면 dataset을 자바코드에서 넣어야 하기에.. 분명 자바쪽에서는List<Map>에 형태로 가져올 것이고 그것을 
 dataset에 바인딩을 시켜야 조회 버튼을 눌렀을 때 화면이 보일테니 자바 클래스를 제공을 해줘야 한다. 
 ==================================
 http://localhost:8000/quickview.html?screenid=Desktop_screen&formname=Base::empManager.xfdl 404에러 해결 필요 06/05 11:20




 

#  21/06/04
 
 (1) start된 Tomcat console에 대해 정리해보았다.(서버 흐름) 


  - Loading XML bean definitions from ServletContext resource [/WEB-INF/spring-service.xml]
  - Loading XML bean definitions from ServletContext resource [/WEB-INF/spring-data.xml] 
  - Loaded JDBC driver: oracle.jdbc.driver.OracleDriver
===> Web.xml에 <contextparam-index>에 있는 spring-service.xml , spring-data.xml 를 초기화하고 
     jdbc드라이버를 올린다.
   
정보: Initializing Spring FrameworkServlet 'appServlet' ==> 초기화?한다 스프링 프레임워크 서블릿 appServlet을 근데 여기서 appServlet은 DispatcherServlet을 의미한다.
   
 - Loading XML bean definitions from ServletContext resource [/WEB-INF/spring-servlet.xml] ==> WEB-INF/spring-servlet.xml 정보를 가져온다.
    Mapped URL path [/di/empUpdate.sp4] onto handler 'emp-controller' 
   
 (2) resultMap, result type
   
 (3) 넥사크로 
 환경설정 port번호 설정 

#  21/06/03

Spring4_1_1/WebContent/WEB-INF/Web.xml

