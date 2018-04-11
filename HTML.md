# HTML(Hyper Text Markup Language) 

HTML is skeleton of all web pages. 

마크업  언어 raw text의 구조와 표현을 정의

HTML에서 컴퓨터는 HTML elements로 wrap되어있는 raw text를 해석(interpret)할 수 있음 

HTML Hierachy 중요, 자식 엘리먼트가 부모 엘리먼트의 행동이나 스타일링을 상속 받음 

W3C에서는 HTML 작성시 2 space of indentation을 추천 

<br>

`<!DOCTYPE html>`

- HTML  문서의 첫줄에  선언,  HTML을 사용한 다는 것을 브라우저가 알 수 있도록 
- 선언후 \<html>\</html>태그로 html 코딩 시작



**태그 종류**

- `<body>` : 웹페이지에 실제로 나타남
- `<head>`  :  웹 페이지에 대한 메타데이터를 포함하고 있음, 페이지에 보여지지 않는 정보, 페이지 자체에 대한 정보를 포함 


- `<div>` : 페이지를 구분

- HTML에서  텍스트를 보여주고 싶은 경우 

  - `<p>` : block of plain text
  - `<span>` : 짧은 txt나 다른 HTML을 포함, 똑같은 줄에 있는 컨텐츠를 구분하고 싶은 경우	span은 div와 다르게 줄 구분을 시키지 않음

- `<br>` : line break, 닫는 태그 없음

- `<em>` : 이태릭 체 

- `<strong>` : bold

- `<img src="" alt="" />` : 이미지 태그안에 alt Attr에는 이미지의 description을 기술 , 이미지가 로딩되지 않을 경우 화면에 표시 됨

- `<video src="" width="" height="" controls>Video not supported</video>` : 

  - controls 옵션을 주면 기본적인 비디오 컨트롤 가능, pause, play, skip 
  - 비디오 태그 사이에는 비디오가 로드 되지 않을 경우 보여줄 문장

- `<a href="" target="_blacnk"></a>` : anchor 태그, hyperlink reference 

  - target Attr에 _blank 옵션을 주면 링크를 눌렀을 경우 새 창(새 탭)에서 열리게 됨

- `<a href=""><img src=""/><\a>` : 이미지를 누르면 해당 링크로 이동 가능

- `<li><a href="#introduction">Introduction</a></li>`

  - 태그에 id를 부여해서 동일한 이름의 태그들을 구분할 수 있음, 이를 이용해서 a href 태그에 링크대신 "#id"를 주면 해당 링크를 눌렀을 경우 페이지의 원하는 부분으로 이동 가능

- List

  - `<ul>` : Unordered List
  - `<ol>` : Ordered List 
  - `<li> `: List Item  

- Table

  ````html
  <table>
  	<tr>
  		<th></th> table heading => 행, 렬의 타이틀
  		<th scope="col" || "row" ></th> 
          		어느 부분의 타이틀인지 scope attr이용 해서 정함
  	</tr>
  	<tr>
  		<td></td> table data-> 행안의 정보들
  		<td colspan="2"></td> => 두개의 열을 합칠 수 있음
  		<td rowspan="3"></td> => 두개의 행을 합칠 수 있음
  	</tr> => table row, 행
  </table>
  ````

- 테이블이 커지면 관리하기 힘드므로 테이블을 head, body, foot으로 나눠서 관리

  - `<thead>` : th 태그를 감쌈 
  - `<tbody>` 
  - `<tfoot> ` : row의 합이라던가 결과를 표현하는 행
