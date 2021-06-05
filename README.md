# Study

#  21/06/05/넥사크로 보충
 
  spring4_1_1을 nexa_test로 복사후 workspace80에 따로 만든후 넥사크로 프로젝트 생성
  화면을 top/left로 생성 후 finsh
  Form-top, Form-left에서 라벨에 텍스트를 넣은후 테스트
 (이후 목적 : 이클립스에 배포하는 과정)
 base -> file -> new -> form -> name 정하고 default로 설정후 완성 -> id : btn_sal로 정함 조회 버튼
 버튼을 더블클릭하면 이벤트 처리로 간다. 	alert("조회 설정 성공");
tool -> 제너레이트 -> 크롬만 설정후 nexa_test/webcontent로 경로 지정
그 후 이클립스에서 실행 
http://docs.tobesoft.com/nexacro_17_ko  ==> 넥사크로 api  (help)
PPT 4.화면 개발 실습 부분에서 디비 연동에 대한 설명이 들어가있다.
4.4.5에 JSP 관련 
PPT 6.메인 화면 구성은 전체 페이지를 어떻게 구성해야 하는가 설명
SDI어플리케이션 -> 싱글
6번은 메인에 대한 디자인 5번은 팝업창 4번은 페이지 처리 순서라고 보면 된다.
empManager 에서 grid -> dataset으로 row column을 넣고 정할수 있다. source에서도 넣는게 가능하다.

C:\Users\user\Documents\nexacro\17.1\projects\nexacro17_Education_Materials\Sample\EduProject ==> 소스 모음
Form_EmpMLM, Form_Organization 좋은 예시소스  html에는 없는 bind component를 ui툴에서는 사용이 가능




 

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

