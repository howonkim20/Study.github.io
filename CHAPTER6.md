# 컴퓨터 과학 교양 강좌 : cs 50

---

(https://howonkim20.github.io/Study.github.io/CHAPTER1)

(https://howonkim20.github.io/Study.github.io/CHAPTER2)

(https://howonkim20.github.io/Study.github.io/CHAPTER3)

(https://howonkim20.github.io/Study.github.io/CHAPTER4)

(https://howonkim20.github.io/Study.github.io/CHAPTER5)

(https://howonkim20.github.io/Study.github.io/CHAPTER6)

# chapter 6 : 웹 프로그래밍

<br> <br>

# 소단원

## <b> 1. HTML

- HTML 이란? <br>
  HTML(Hyper Text Markup Language)은 웹 페이지의 내용을 나타내는 언어입니다. 반복문이나 조건문 등을 포함하는 프로그래밍 언어가 아니지만, 웹 페이지의 내용을 어떻게 구성할지 결정할 수 있습니다. 사용자가 웹 페이지를 요청하면 웹 서버는 페이지의 내용을 HTML로 보내고, 웹 브라우저는 HTML을 해석해 페이지를 사용자에게 보여줍니다.

        1. 일반적으로 사용되는 태그들
        HTML에는 웹 페이지의 형식을 만들 수 있는 많은 태그들이 있습니다.
        이미 소개된 기본적인 태그들인 html, head, title, body는 여러분이 작성하는 거의 모든 웹 페이지에 쓰일 것입니다.
        다른 태그들은 특정 상황에서만 쓰게 될 것입니다.
        예를 들어, 웹 페이지의 제목들은 <h1>에서 <h6>까지의 태그들로 나타낼 수 있습니다.
        <h1>이 가장 크며, 주 표제이고, 숫자가 올라갈수록 더 작아집니다. <p> 태그는 문단을 나타냅니다.

        2. 요소의 속성
        HTML 요소들은 이름뿐만 아니라 속성도 가지고 있습니다. 속성은 HTML 요소에 대한 추가 정보를 제공합니다.
        예를 들어, <img>라는 이미지 태그에는 src라는 속성이 있는데 사진 파일이 어디에 있는지를 명시합니다.
        <img src=”cat.jpg”> 같은 태그를 사용했을 때 cat.jpg가 HTML 문서와 동일한 디렉토리(저장위치)에 있으면, 웹 페이지에 사진을 보여줄 것입니다.

        HTML에서 다른 페이지로 링크를 만들기 위해서 <a> 태그를 씁니다. <a> 태그에서 href라는 속성을 씁니다.
        href는 웹 페이지를 어디로 링크시킬지 명시합니다.
        결과적으로, <a href=http://google.com>Click Here</a>와 같은 HTML은 “Click Here”라고 표기된 링크를 생성하고, 클릭했을 때 사용자는 구글 웹 사이트로 가게 됩니다.

        모든 HTML 요소들은 id 속성을 가질 수 있습니다.
        고유한 값이어야 하는 id 속성은 웹 페이지에서 특정 요소를 분간하고 확인할 수 있게 도와줍니다.
        HTML 요소는 class 속성도 가질 수 있는데, 고유한 값이 아니어도 되며, 이것 또한 HTML 요소를 확인하는 데에 쓰입니다. CSS와 JavaScript에 대하여 공부하다 보면 id와 class 속성이 어떻게 유용하게 쓰이는지 알게 될 것입니다.

## <b> 2. CSS

- CSS란? <br>
  HTML이 웹 페이지의 구조를 표현하기 위한 언어인 반면, CSS(Cascading Style Sheets)는 웹 페이지를 디자인하기 위해 인터넷에서 사용되는 언어입니다. 웹 사이트를 디자인한다는 것은 텍스트의 정렬, 다양한 요소의 크기나 색, 창의 크기가 조정될 때 HTML 요소가 어떻게 나타날 지 등을 결정하는 것입니다. CSS를 웹 페이지에 포함시키는 몇 가지 다른 방법이 있습니다.

        1. Style속성
        CSS는 HTML의 요소 태그 안에 style 속성으로 사용할 수 있습니다.
        CSS는 속성과 값이 한 쌍을 이루어 사용되며, 각각의 CSS 속성 뒤에는 콜론(:)과 그 값이 옵니다.
        또한 여러 속성-값 쌍의 경우 세미콜론(;)으로 분리됩니다.

        1 : <p style="font-size:28px;">
      2 : This is a paratraph.
        3 : </p>
        <코드 1>

        <코드 1>을 보면, <P> 태그 안에 CSS를 직접 포함시켰습니다. CSS 속성으로 font-size를 추가했고 그 값을 28px로 설정했습니다.
        CSS를 적용시킨 결과로 HTML이 웹 브라우저에 표시될 때 이 문단은 28px의 글꼴로 나타날 것입니다.

        HTML 속성과 CSS 속성에 차이가 있는지 살펴봅시다.
        style은 HTML 속성의 이름이고, font-size는 CSS 속성의 예입니다.
        CSS속성은 굉장히 다양합니다.
        color는 텍스트의 색을 설정하고, text-align은 텍스트를 왼쪽, 가운데 등으로 정렬합니다.
        font는 텍스트의 글꼴을 설정합니다.

        2. Style 태그

        <!DOCTYPE html>
        <html>
          <head>
              <title>Page</title>
              <style>
      	    p
      	    {
      		    font-size:28px;
      	    }
              </style>
          </head>
      <body>
      <p>This is a paragraph.</p>
      </body>
        </html>
        <코드 2>

        CSS는 style 태그의 내부에 위치할 수 있습니다.
        <코드 2>의 5-10행과 같이 대개 HTML 문서의 head 부분에 위치합니다.
        style 태그 안에서 가장 먼저 무엇에 스타일을 적용할 것인지 명시해야 합니다.
        요소의 이름 (예를 들어 p), ID, class 등이 될 수 있습니다. ID에 스타일을 적용한다면, #과 그 뒤에 ID의 이름을 적어서 ID를 참조합니다.
        클래스에 적용한다면, .과 그 뒤에 클래스의 이름을 적어서 참조합니다.

        스타일을 어디에 적용할 지 결정한 후, CSS 속성-값 쌍은 괄호 {}안에서 세미콜론(;)으로 분리해 포함시킬 수 있습니다.
        6-9행에서 모든 p 요소가 글꼴의 크기로 28을 가져야 한다고 명시하고 있습니다.

        이런 방식을 사용하면 같은 HTML 요소를 여러 번 사용하였을 때, 동일한 CSS를 반복할 필요가 없습니다.

        3. 분리된 CSS
        CSS로 스타일을 지정하는 3번째 방법은 완전히 분리된 파일에 CSS를 저장하는 것입니다.
        <style> 태그 안의 내용을 문서로 저장하면, d일반적으로 .css 형태의 파일이 생성됩니다.
        그리고 이러한 CSS 파일을 HTML 문서 안으로 불러와 HTML 문서의 head 요소에 <link> 태그를 포함하면 CSS가 적용됩니다.
        <link href=”style.css” rel=”stylesheet” />과 같은 줄을 포함하면, 외부의 CSS 문서가 HTML 문서에 추가되어 적절한 스타일이 나타날 것입니다.

        CSS를 분리된 문서로 만드는 것은 서로 다른 HTML 문서들이 같은 스타일을 사용할 때 유용합니다. 그 HTML 문서들의 스타일을 바꿔야 할 때, CSS 문서 하나만 바꿔주면 나머지 HTML 문서들의 스타일은 자동적으로 적절하게 바뀌게 됩니다.

## <b> 3. SQL

- SQL이란? <br>
  SQL(Structured Query Language)은 데이터베이스에서 사용하는 언어입니다. 데이터를 추가하거나 삭제하고 필요에 따라 조회할 수도 있습니다. 데이터를 저장하는 방법으로 지금까지는 C의 파일입출력을 알아보았지만 좀 더 많은 양의 데이터를 체계적이고 빠르게 찾아보기 위해서는 SQL을 어떻게 사용하는지 배워보는 것이 좋습니다. 데이터베이스는 사용자 데이터를 영구히 저장했다가 필요할 때 가져옴으로써 웹에서 더 좋은 사용자 경험을 제공할 때 사용합니다.

## <b> 3. JavaScript

- JavaScript란? <br>
  PHP를 이용하면 역동적인 웹사이트를 만들 수 있습니다. PHP는 웹 서버 측의 프로그램을 만드는 데 사용되는데, 웹 브라우저와 같은 클라이언트에서 사용되는 자바스크립트(JavaScript)를 알면 더 많은 것들을 할 수 있습니다. JavaScript는 사용자가 입력한 데이터를 다루거나 웹 서버에 요청하거나 웹 페이지를 변경하는 역할을 함으로써 사용자가 웹 서비스를 더 잘 사용할 수 있도록 해줍니다.

        1. 자바스크립트의 문법
        PHP의 문법이 C와 매우 유사하듯이 JavaScript 역시 C 또는 PHP와 매우 비슷합니다.
        그리고 JavaScript PHP와 같이 main 함수가 없습니다. JavaScript의 조건문, 반복문은 C언어의 문법 구조와 동일합니다.

        var s = "hello, world!";
        var num = 3;
        var number = [4, 8, 15, 16, 23, 42];
        var quaot = {symbol: "FB", price: 79.53};
        <코드 1>

        <코드 1>을 통하여 JavaScript의 변수, 배열, 객체 사용법을 살펴볼 수 있습니다.
        JavaScript는 PHP와 마찬가지로 자료형을 따로 명시하지 않습니다.
        그러나 $를 쓰지 않고 var 뒤에 변수명을 작성합니다.
        배열은 3행과 같이 [ ]괄호 안에 데이터를 나열합니다.

        객체는 4행과 같이 선언하여 사용할 수 있는데, JavaScript에서는 객체를 자주 사용합니다.
        { }괄호 내부에 키와 값의 조합이 작성되는데, 각각의 조합은 쉼표로 나누어집니다.
        :기호 왼쪽이 키, 오른쪽이 값입니다.
