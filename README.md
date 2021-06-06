# Study

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

