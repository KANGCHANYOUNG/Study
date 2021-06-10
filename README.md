# Study

#  21/06/10

1교시
부트스트랩에 대한 설명 
게시판 getBoardList 수정

2교시
![1](https://user-images.githubusercontent.com/78460496/121451714-068e3000-c9d9-11eb-8cf6-b8dc373ad0d3.JPG)


브라우저에 출력 방법 2가지
 
 크롬 -> 인터프리터 ->Tag를안씀

 브라우저 document.write("Tag")                  
 자바문법으론    out.print("")
 개행 처리 시 ln은 의미가 없다 <br>쓴다   
 처리할때 out.print("<br>") 
 ((<%=%> )))쓴다(내장객체이기에) ;을 쓰지 않는다


html은정적만 올수있다    fetch하고 그대로 처리  쿠키 -> local   
 
  (jsp) java +        타임라인순서

컴파일 일어나서(타입) -->클라이언트에 fetch 주체는 크롬이다.

"유지 -->세션, 쿠키        캐쉬메모리를 쓴다. 문제는 비싸기에 용량에 제약이 있다.

 
 

  
![2](https://user-images.githubusercontent.com/78460496/121451740-10179800-c9d9-11eb-98b7-d94a70971e01.JPG)

let a = "<%= %>";                                                                
 정적(상수이다)->처리 주체가 서버이다. 
 이미 패치가 일어나서 변하면 안된다 우리가 쓰는 프로토콜은 stateless인데
 쿠키와 세션이 있고(유지 문제) 고정값이다. 자바스크립트와 익스프레션이 만났을때!
  
  자바스크립트   = 익스프레션(아빠가 java)
  client       치환     server 

  3교시
  
![3](https://user-images.githubusercontent.com/78460496/121459322-fdf02680-c9e5-11eb-9e0b-e3ab639999dc.JPG)



(#dg_board)(#)이 오면 유니크 자바에선 protected  erd에선 PK 
DOM - hoisting 순서(위치)
$('#dg_board').datagrid --> object --> () 생성자 --> 구현( {}을 의미 이 영역은 실행문이 오는 자리이다.  ) --> 메소드, event  

1. function - () {}
2. 이름 = function(){}

부적잡한 식별자 뜨면 xml 확인 ->board.xml
부적절한 열 유형 -->sql

table id="dg_board" class="easyui-datagrid" data-options="title:'게시판', toolbar:'#tb_board'" style="width: 1000px; height: 350px">

구분자는 콜론
열거형 연산자
바깥쪽에는 더블 ""
안쪽은 싱글 ''

4교시
https://www.jeasyui.com/documentation/index.php#

url:'datagrid_data.json' 
http://localhost:8000/board/jsonGetBoardList.sp4

----------------
![4](https://user-images.githubusercontent.com/78460496/121470355-0e5dcc80-c9f9-11eb-8561-1e00c8d076dc.JPG)
조회 버튼을 누르면 id ="btn_sel"을 타게된다.

![5](https://user-images.githubusercontent.com/78460496/121470497-4533e280-c9f9-11eb-9f94-734903c27998.JPG)

여기서 메소드를 부른다.

![6](https://user-images.githubusercontent.com/78460496/121470555-5b41a300-c9f9-11eb-9d25-248fbfccdea8.JPG)

출력하게 된다.

--------------
5교시

넥사크로,안드로이드 -> xml기반

+ 파이어베이스 연계 

1.ready( )  --> xxx.sp4

2.버튼   -->  xxx.jsp
       Event xxx.sp4 -> js    Tag로는 안된다!
     
  조건 검색 -> 파라미터를 넘겨야 한다. 2번과 가깝다. Tag로 처리할건지 js로 처리할건지..고민하지말고 js
  
  
  
  ![7](https://user-images.githubusercontent.com/78460496/121473158-318a7b00-c9fd-11eb-8c4c-7d955fd2cd8c.JPG)

  
  datagrid를 부른다.  
  <table class = "클래스이름"  easyui-datagrid
  비동기로 처리하면 ajax
         
  <script type"textjavascript
  $(document).ready()는 문서가 준비되면 매개변수로 넣은 콜백 함수를 실행하라는 의미입니다.
  
  <bean id class
          <property name= " " ref = "id"
            
          xml이라 문법이 다르다 tag와tag사이에 문법이 다르다.


        
          
          
          
      
  




#  21/06/09
1교시 
객체 초기자
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Object_initializer


![2](https://user-images.githubusercontent.com/78460496/121275872-88faef00-c908-11eb-9906-4486ead47be4.JPG)

키값과 value과 일치하면 생략할 수 있다. 
const object2 = {a: a, b:b, c : c,}; const object3 = {a, b, c};

<Books book ={book}/>  

![1](https://user-images.githubusercontent.com/78460496/121275610-1722a580-c908-11eb-8bff-c1342f51e952.JPG)
불변 유무


var를 쓰게되면 전역변수와 지역변수 경계가 없고 좌우중괄호 경계가 없어진다. 
![3](https://user-images.githubusercontent.com/78460496/121276630-f3605f00-c909-11eb-98a8-70917e09837e.JPG)


이렇듯 key값 value 값이 일치하면 생략할 수 있다.


구조 분해 할당
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment
자바스크립트는 0이면 false다. java와 다르게 에러 조심! 

2교시

![4](https://user-images.githubusercontent.com/78460496/121279562-b72ffd00-c90f-11eb-8a25-ec28e38ac3c6.JPG)
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array api 참고

전개구문 api
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Spread_syntax


![5](https://user-images.githubusercontent.com/78460496/121280915-0414d300-c912-11eb-852c-9f35c1b7988d.JPG)

3교시

![7](https://user-images.githubusercontent.com/78460496/121284438-d03cac00-c917-11eb-8a35-1e3540a420ae.JPG)

![8](https://user-images.githubusercontent.com/78460496/121284918-80aab000-c918-11eb-851b-600f24923584.JPG)

spread syntax 배열을 만들거나 복사해온다. ...을 붙힌다. 


app.jsx에서 이벤트 처리를 담당하게 하자.
book -app 밑에 node-moduels  그 밑에  
public -> index.html -> index.jsp 이미지에 대한 정보가 여기로 배치된다. -> div id='root'면 렌더링이 여기서부터 시작한다고 보면된다.
                             components --> book, books                  
src
package.json -> json형태로 file이 관리 되어가고 있다.
yarn.lock ->yarn 관리


books 상태 바뀔떄 마다 render()라는 함수 호출


주소번지를 넣으려면 {}   

기본값 매개변수

Optional chaining

https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Optional_chaining


5교시

![11](https://user-images.githubusercontent.com/78460496/121309908-b57d2e00-c93d-11eb-9d36-6c021638092c.JPG)
![12](https://user-images.githubusercontent.com/78460496/121309897-b3b36a80-c93d-11eb-9e75-d3a701345243.JPG)
![13](https://user-images.githubusercontent.com/78460496/121309902-b44c0100-c93d-11eb-99f9-4381d7e1eafa.JPG)
![14](https://user-images.githubusercontent.com/78460496/121309903-b4e49780-c93d-11eb-8aa0-d20ea2d90dc4.JPG)
![15](https://user-images.githubusercontent.com/78460496/121309906-b4e49780-c93d-11eb-99d6-38c86398e272.JPG)





#  21/06/08

(1교시) typescript로 넘어가는 과정!

![1](https://user-images.githubusercontent.com/78460496/121476733-fcccf280-ca01-11eb-87e9-065484a651a0.JPG)
객체는 크게보면 3가지 1. 내장객체 -> 사용자 객체포함 --> String, Array, Date(Ajax에서) --> 중첩 사용가능 
window.loaction.href = " ";
      (내장 객체)(이동)
2. 브라우저 객체(BOM), 3. 문서 객체(DOM) 
      
{local} switch문이나 for문안에서 int i로 정의했을 경우 {}밖에서는 정의가 안되는거랑 비슷한 메커니즘  
브라우저 문제는 크롬을 무조건 사용해야 한다.
참조변수(인스턴스변수) = function(){} 레퍼런스 타입은 react같은 경우 적극적으로 사용됨 구조체(체인닝) 
var tv = new Object -->tv.channel = 10 tv.power = true or false 이런식으로 사용 가능

![2](https://user-images.githubusercontent.com/78460496/121476752-00f91000-ca02-11eb-876a-b63a5f0c24e2.JPG)

tv.info = function(){      --> 패턴1
 this.color // 이러한 경우this는 tv라는 객체를 바라본다.
 this.channel
} 
var car = {  --> 패턴2
         color : "black", price : 50000000, info : function(){  } --> 보통 이러한 패턴이다.
          };
---------------실습
spring 4_1_1  code.으로 열고 ch03 만듬 -> pattern1.js파일 만듬 -> 
![3](https://user-images.githubusercontent.com/78460496/121476761-048c9700-ca02-11eb-91b0-f1e184888d9a.JPG)cmd에서도 사용은 가능하지만 비효율적

스튜디오코드 내에서는 node 파일이름.js로 터미널로 실행이 가능하다! 

2교시

호이스팅(hoisting) : 함수 안에 있는 선언들을 모두 끌어올려서 해당 함수 유효 범위의 최상단에 선언하는 것을 말한다.
window <- 최상위 객체 
document라는 내장 객체 -> 그아래 html -->  그 아래 첫째 아들 head 둘째 아들 body --> body는 화면에 출력, head ->meta (view 포트, 인코딩, 호이스팅 등등..)를 처리한다.
body쪽에 script가 있다 하더라도 head쪽으로 끌어올려서 --> 호이스팅(hoisting)
절차지향적은 철저하게 순서 중심이다. document is not defined -->Dom tree가 없어! window 바로 직계 자녀임

호이스팅(hoisting) : 함수 안에 있는 선언들을 모두 끌어올려서 해당 함수 유효 범위의 최상단에 선언하는 것을 말한다.
일반 함수 정의방식과 익명 함수 선언 방식의 차이점
일반 함수 정의는 함수 호출 시 호이스팅(hoisting) 기술을 지원 합니다.
그러나 익명 함수 선언 참조 방식은 호이스팅을 지원하지 않습니다.
호이스팅을 적용하면 함수 정의문 보다 호출문이 먼저 나와도 함수 정의문을 
끌어 올려서 함수를 호출 합니다.

Template literals : 템플릿 리터럴은 내장된 표현식을 허용하는 문자열 리터럴입니다. 여러 줄로 이뤄진 문자열과 문자 보관기능을 사용할 수 있습니다
https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Template_literals

![6](https://user-images.githubusercontent.com/78460496/121476810-12421c80-ca02-11eb-8d70-50a033e6e2c5.JPG)


![5](https://user-images.githubusercontent.com/78460496/121476834-1837fd80-ca02-11eb-9bba-0fd5203174ca.JPG)
Expression interpolation(표현식 삽입법) 

3교시

let color = ["orange", "red", "green", "aqua"]; //배열형태는 [] Object 형태는{}

getElementById  : 메서드는 주어진 문자열과 일치하는 id 속성을 가진 요소를 찾고, 이를 나타내는 Element 객체를 반환합니다.


![6](https://user-images.githubusercontent.com/78460496/121116015-dae03e00-c850-11eb-9ba9-59bfcd3f9370.JPG)
-------------------------
5교시 게시판 만들기
![8](https://user-images.githubusercontent.com/78460496/121476852-1bcb8480-ca02-11eb-905a-564076654751.JPG)

UI/UX  O|X --> UI/UX없이 테스트 할 수 있냐? 없냐? 애매한데? 애매한사람이 제일 나쁜 사람
HOW ? -> 쿼리 스트링 (?) &연산자  
 PostMan         get(제약조건) -> 
 -->단위 테스트  post 
 parameter , , ,   ...Arrry
파라미터로 처리(상수_ --> const final prototupe

WHERE?

데이터 JDBC 기준, 경우의수  , 문제해결능력
개발하는데 다른일 하는 것 비동기 처리 
AJAX -> REACT 

ORM 솔루션-> JDO HIBERRATE MYBATIS
Insert(id , p)
insert into  M()  Values ()    배달사고 주의 
insert       S()  Values ()
응답에 중요한건 리턴타입 --> 유지 -->forward -->request, (sendRedirect쓰면 맞아야한다.) 
http://blog.naver.com/PostView.nhn?blogId=seotaji&logNo=80165579691
forward와, Redirect 차이를 모르면 공부안한사람 

![9](https://user-images.githubusercontent.com/78460496/121476873-1f5f0b80-ca02-11eb-8465-444bafb97510.JPG)

![10](https://user-images.githubusercontent.com/78460496/121476884-22f29280-ca02-11eb-85be-7744436cc45a.JPG)
6교시

![11](https://user-images.githubusercontent.com/78460496/121476890-2554ec80-ca02-11eb-96cc-1a588ff1b814.JPG)

outer조인을 생각하면 보는 세상이 다른 사람 

desc board_master2019

desc board_sub2019

![12](https://user-images.githubusercontent.com/78460496/121476911-2c7bfa80-ca02-11eb-8e86-f220e05cadbb.JPG)
조회수 그룹번호는 0 Default값 

------- --> 컬럼수 만큼 있어야지 뭘 물어? 이렇게 안하려면 로직에서 map에다 다 박던지; dao에서 하지말고
xxxx.sp4?bm_no=101
            &bm_title= 게시판 연습  --> 컬럼수 만큼 있어야지 뭘 물어? 이렇게 안하려면 로직에서 map에다 다 박던지; dao에서 하지말고
             &bm_writer= 이순신
                &bm_content= 내용
                    &bm_date= 20121-06-08
                  &bm_hit= 0
                     &bm_group= 0  bm_no처럼 채번해야 된다.
                     &bm_pos = 0 원글이면 0 1차 댓글이면 1, 1차 댓글에 대한 공격글이면 2가됨
                     &bm_step = 0
                     &bm_pw= 123
                     &bm_email= 이메일 연습

/board/boardInsert.sp4?bm_no=101
            &bm_title= 게시판 연습  
             &bm_writer= 이순신
                &bm_content= 내용
                    &bm_date= 20121-06-08
                  &bm_hit= 0
                     &bm_group= 0  bm_no처럼 채번해야 된다.
                     &bm_pos = 0 원글이면 0 1차 댓글이면 1, 1차 댓글에 대한 공격글이면 2가됨
                     &bm_step = 0
                     &bm_pw= 123
                     &bm_email= 이메일 연습


INSERT INTO board_maseter(bm_no, bm_title, bm_writer, bm_content
                          ,bm_date ,bm_hit, bm_group, bm_pos, bm_step
                          ,bm_email, bm_pw)
 
 VALUES(#{bm_no},#{bm_title}, #{bm_writer}
 
VALUES(SELECT 문.....) 


                    
                    





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

이제 이 while문 안에 각각의 스타일을 지정하는 코드를 넣어주도록 합시다. 먼저 alist의 i번째 원소를 가져오면 되겠죠. 그리고 이렇게 가져온 태그의 스타일을 지정해주면 됩니다. 마지막에 i에 1을 더해주는 것도 잊으면 안된다.

var i = 0;
while (i < alist.length) {
  alist[i].style.color = 'powderblue';
  i = i + 1;
}
querySelectorAll --> 다수의 태그를 사용하고 싶다면
querySelector -> 하나의 태그만 알려준다.


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

![2](https://user-images.githubusercontent.com/78460496/121476668-eaeb4f80-ca01-11eb-8154-ebe09e777fea.JPG)
![3](https://user-images.githubusercontent.com/78460496/121476641-e4f56e80-ca01-11eb-8220-25938099b9c9.JPG)

Dom에 대한 생성, 시점이 우리가 얘기하는  Lifecycle이 연관이 있다. 
함수는 괄호로 생성하고 세미콜론은 생략하면 된다. 이런것들이 이제 내부에 올 수도 있고 외부에 있는 함수를 호출 할 수 있다.
아까 test2 undefined 같은 오류들을 조심해야 한다. easy ui를 쓸 때는 jQuery기반이고 직접접근이 아니라 $표시를 이용해 접근한다.
$(document).ready(function({ --> 익명 함수이다. 
});     
$("# dg_emp").datagrid(); -> 생성자
js기반은 기본적으로 오브젝트가 들어가 있다.

![4](https://user-images.githubusercontent.com/78460496/121476624-de66f700-ca01-11eb-80c2-f22ac4094db1.JPG)


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
![jar](https://user-images.githubusercontent.com/78460496/121476506-baa3b100-ca01-11eb-84b7-6cccbb29eb9d.JPG)




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

