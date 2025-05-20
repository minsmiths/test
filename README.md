# HTML 정리
기본 - ~ .html로 파일 생성후 !입력해 기본 틀 생성 <br>
<h2>태그 정리</h2>
&lt;p&gt;: 본문 작성할때 사용 <br>
&lt;hr&gt;: 가로줄 생성 <br>
& nbsp: 스&nbsp페&nbsp이&nbsp스&nbsp를 인위적으로 만든다. <br>
&lt;!-- --!&gt;: 주석 처리 ctrl+/로 한꺼번에 처리 가능 <br>
<h3>[강조태그]</h3>
&lt;b&gt;: 글자를 굵게 해줌, <b>단순 굵게 표시</b> <br>
&lt;strong&gt;: 글자를 굵게 해줌, <strong>중요한 내용임을 명시</strong> +strong{강조내용} 그리고  TAB을 누르면 작성됨됨 <br>
&lt;i&gt;: 글자를 기울임, <i>단순 기울임+ css 같이 사용</i>
&lt;em&gt;: 글자를 기울임, <em>강조할 내용임을 명시</em> <br>
<h3>[첨자태그]</h3>
&lt;sup&gt;: 위첨자 표시, ex) 5<sup>2</sup> <br>
&lt;sub&gt;: 아래첨자 표시, ex) H<sub>2</sub>O <br>
<h3>[밑줄태그]</h3>
&lt;u&gt;: 과거에는 단순히 밑줄을 긋는 용도 but <u>현재는 css와 함께 사용</u> <br>
&lt;s&gt;: 더이상 <s>유효하지 않은</s> 내용을 나타낼때 <br>
<h3>[인용태그]</h3>
&lt;blockquote&gt;: 긴인용을 할때 사용이 된다. <blockquote cite="https://www.yalco.kr/@html-css/1-3/"> <p>보통 들여쓰기가 되어서 나타난다.</p> </blockquote>
&lt;cite&gt;: <cite> &lt;blockquote&gt;- 인용블록요소</cite> fromMDN <br>
&lt;q&gt;: 짧은 인용문 <q cite="https://developer.mozilla.org/ko/docs/Web/HTML/Element/q">이렇게 인용된 부분이 표시가 된다 </q> <br>
&lt;mark&gt;: 인용문에서 주시해야할 부분 표시, ex) 본 페이지는 <mark>"인용문"</mark>이란 키워드로 검색한 결과임 <br>
&lt;abbr&gt;: <strong>abbr</strong>태그를 사용하여 <abbr title="HyperText Markup Language">HTML</abbr>의 풀네임을을 표기한 문단이다. <br>
<h3>[목록태그]</h3>
&lt;li&gt;: 목록 아이템<br>
&lt;ul&gt;: 순서없는 목록 <br>
<ul>
  <li>난 순서가 없다.
  <li>진짜 없음
  </ul>
&lt;ol&gt;: 순서있는 목록 <br>
<ol>
  <li>난 순서가 있다.
  <li>진짜 있음
  </ol>
<ol type="A" start="2">
  <li>심지어 속성도 바꿀수 있지 </ol>
<h3>[용어,정의 나열 태그] </h3>
&lt;dl&gt;: 용어와 정의가 들어있는 리스트 <br>
&lt;dt&gt;: 용어 <br>
&lt;dd&gt;: 정의 <br>
<dl>
  <dt> 프로그래밍</dt>
  <dd>컴퓨터 프로그램을 작성하는 일</dd>
  </dl>
<h3>[이미지태그]</h3>
<ul>
  <li><h4>이미지가 직접적인 경로를 이동해 보여지는 경우</h4></li> </ul>
&lt;img src="이미지 경로" alt="대체 텍스트" title="툴팁">(alt와 title은 설명이 같으면 안된다.) <br>
<ul>
  <li><h4>이미지를 같은 폴더에 저장하여 경로를 내 컴퓨터로 이동해 보여지는 경우</h4></li></ul>
  &lt;img
    src="./coding.png" ( './'는 현재 폴더라는뜻)<br> 
    alt="코딩중인노트북"
    title="프로그래밍"
  &gt;
<ul>
  <li><h4>다른 파일에 있는 이미지를 불러오는 경우</h4></li></ul>
  &lt;img
    src="./images/coding.png" (images파일에 있는 사진 불러오기)<br>
    alt="코딩중인노트북"
    title="프로그래밍밍"
  &gt;
<ul>
  <li><h4>현재있는 폴더에서 나가서 다른 폴더에 있는 사진을 불러오는 경우</h4></li></ul>
  &lt;img
  src="../images/coding.png" ('../'는 일단 부모 폴더로 나가서 다른 폴더로 접근한다.) <br>
  alt="코딩중인노트북"
  title="프로그래밍밍"
  &gt; <br>
  <h3>[표만들기태그]</h3>
  &lt;table&gt;: 테이블 <br>
  &lt;caption&gt;: 테이블 설명 <br>
  &lt;tr&gt;: 행 <br>
  &lt;td&gt;: 데이터셀<br>
  &lt;th&gt;: 행 또는 열
  헤드 <br>
  &lt;thead&gt;: 테이블 헤드 <br>
  &lt;tbody&gt;: 테이블 본문 <br>
  &lt;tfoot&gt;: 테이블 결론...? <br>
  &lt;colgroup&gt;: 표에 열을 묶어서 속성 부여
  <h4> -표 속성-</h4>
  <ul>
    <li>scope="row or col" -> 범위 설정 </li>
    <li>span="숫자"->{열병합(colspan), 행병합(rowspan)} </li>
    </ul>
<table>
    <thead>
      <th scope="col">과목</th>
      <th scope="col">월</th>
      <th scope="col">화</th>
      <th scope="col">수</th>
    </thead>
    <tbody>
      <tr>
        <th scope="row"> HTML </th>
        <td>60분 </td>
        <td>60분</td>
        <td>0분</td>
      </tr>
      <tr>
        <th scope="row"> CSS </th>
        <td>0분</td>
        <td>30분</td>
        <td>60분</td>
      </tr>
      <tr>
        <th scope="row"> JS </th>
        <td>0분</td>
        <td>0분</td>
        <td>60분</td>
      </tr>
    </tbody>
    <tfoot>
    <tr>
    <th> 총시간</th>
    <td> 60분</td>
    <td>90분</td>
    <td>120분</td>
    </tr>
    </tfoot>
</table>
<h3>[다른곳으로 링크태그]</h3> <br>
&lt;a href="(연결할 주소)" target="(링크를 열 곳 옵션)"&gt;: 다른곳으로 이동
<h4>-target 속성-</h4>
<ul>
  <li>_self: 현재창</li>
  <li>_blank: 새 창</li>
  <li>_parent:부모 프레임
  </li>
  <li>_top: 최상위 프레임임</li>
</ul>
  &lt;a href="https://www.google.com" target="_blank" &gt;구글로 가기(새 창에서)</a>
  <a href="https://www.google.com" target="_blank" >구글로 가기(새 창에서)</a> <br>
  <h4>-이미지로 사이트 이동-</h4>
    <a href="https://www.yalco.kr" target="_blank">
    <img src="https://showcases.yalco.kr/html-css/01-07/yalco-logo.png" 
    alt="얄코 사이트로 가기(새 탭에서)" title="얄코 사이트로 이동"></a>
  <br>
<h4>id요소를 이용한 스크롤 이동</h4>
  &lt;a href="#target_4"&gt;타깃으로 이동</a> <br> 
  <a href="#target_4">타깃으로 이동</a>
  <p id="target_1">id: target_1</p>
  <p id="target_2">id: target_2</p>
  <p id="target_3">id: target_3</p>
  <p id="target_4">id: target_4</p>
&lt;address태그&gt;: 주소 및 연락처 정보를 포함 <br><br>
 <address>
    웹사이트 주소: <a href="https://www.yalco.kr">yalco.kr</a> <br>
    오피스: 전산시 개발구 코딩동 123번길 45 <br>
    전화 <a href="tel:010-1234-5678">010-1234-5678</a> (href값 앞부분에 'tel'을 붙이면 전화번호로 연결됨 ) <br>
    이메일: <a href="mailto:yalco@kakao.com">yalco@kakao.com</a> (href값 앞부분에 'mailto'를 붙이면 이메일로 링크됨)
  </address>
<h3>[사용자로 부터 입력받기]</h3>
&lt;form&gt;: 정보를 제출하기 위한 태그들을 포함(&lt;form action="페이지"&gt;) <br>
&lt;input&gt;: 입력을 받는 요소(&lt;input id="name" name="name" type="text") <br>
&lt;label&gt;: 인풋 요소마다 라벨(&lt;label for="name"&gt; 이름) <br>
&lt;button&gt;: 버튼(&lt; button type="submit or rest or button"&gt;) <br>
--label의 for속성과 input의 id속성이 같아야한다. <br>
&lt;fieldset&gt;: 그룹화함 <br>
&lt;legend&gt;: fieldset요소의 제목 설명 <br>
<form action="#"> 
  <fieldset>
    <legend>반장</legend>
    <label for="name">이름</label>
    <input id="name" name="name" type="text"> <br>
    <label for="age">나이</label> 
    <input id="age" name="age" type="number"><br>
    <button type="submit">제출</button>
    <button type="reset">초기화</button>
    <button type="buttom">버튼</button>
  </fieldset>
  </form>
<ul><li>"#"은 현재페이지를 나타낸다</li></ul> <br>
<h4>-텍스트 속성-</h4>
<ul>
  <li>id: 요소를 고유하개 식별한다. </li>
  <li>type: 요소의 종류나 동작 방식을 지정한다.</li>
  <li>placeholder: 빈 칸에 보이는 안내문</li>
  <li>maxlengh: 최대길이</li>
  <li>minlengh: 최소길이</li>
</ul>
<form action="#">
  <fieldset>
  <legend>텍스트 인풋타입</legend>
  <label for="txtIp">text</label> <br>
  <input id="txtIp" type="text" placeholder="5자 이하" maxlengh="5"> <br>
  <label for="pwdIp">비밀번호</label><br>
  <input id="pwdIp" type="password" placeholder="4자 이상"><br>
  <label for="srcIp">search</label><br>
  <input id="srcIp" type="search"> <br>
  <label for="tlIp">tel</label><br>
  <input id="tlIp" type="tel"> <br><br>
  <button type="submit">제출</button>
  </fieldset>
  </form>
<h4>-숫자 속성-</h4>
<ul>
  <li>min: 최솟값</li>
  <li>max: 최댓값</li>
  <li>step: 간격</li> </ul>
<form action="#">
  <fieldset>
  <legend>숫자 인풋타입</legend>
  <label for="numIp">number</label> <br>
  <input id="numIp" type="number" min="0" max="10"><br>
  <label for="rgIp">range</label> <br>
  <input id="rgIp" type="range" min="0" max="100" step="20"> <br>
  <label for="dtIp">date</label>
  <input id="dtIp" type="date" min="2020-01-01" max="2030-12-31"> <br>
  </fieldset>
  </form>
  <h4>-체크 속성-</h4>
  <ul>
  <li>checked:체크박스 & 라디오(체크됨 여부)</li>
  <li>name: 라디오(옵션들의 그룹)</li>
  <li>value: 라디오(옵션에서 실제로 넘겨질 값)</li></ul>
  <form action="#">
  <fieldset>
    <h5>->checkbox</h5>
    <input id="cbIp" type="checkbox" checked>
    <label for="cbIp">유기농</label>
    <h5>->label</h5>
      <input
      type="radio"
      name="fruit"
      id="f_apple"
      value="apple"
      checked
    >
        <label for="f_apple">사과</label>
       <input
      type="radio"
      name="fruit"
      id="f_grape"
      value="grape"
    >
    <label for="f_grape">포도</label> <br>
       <input
      type="radio"
      name="vege"
      id="v_carrot"
      value="carrot"
      checked
    > 
    <label for="v_carrot">당근</label>
    <input
      type="radio"
      name="vege"
      id="v_tomato"
      value="tomato"
    >
    <label for="v_tomato">토마토</label>
    </fieldset>
  </form>
    ---->그룹을 짓고싶을때는 name을 같게해야한다.fruit와 fruits는 다른 그룹이다. <br>
    <h4>-기타 속성-</h4>
    <ul>
      <li>accept: 받아들일수 있는 파일 형식</li>
      <li>multiple: 여러 파일 업로드 가능 여부</li></ul>
    <h4>-인풋 공통 속성-</h4>
    <ul>
      <li>value: 값이 지정됨</li>
      <li>autofocus: 자동 포커스됨</li>
      <li>readonly: 일기만 가능,전송됨</li>
      <li>required: 필수입력!</li>
      <li>disabled: 입력불가, 전송 안됨</li></ul>

  <form action="#">
  <fieldset>
    <label for="valIp">value</label> <br>
    <input 
      id="valIp"
      type="number"
      value="20"
    ><br>
    <label for="afIp">autofocus</label> <br>
    <input 
      id="afIp"
      type="text"
      placeholder="자동 포커스됨"
      autofocus
    ><br>
    <label for="roIp">readonly</label> <br>
    <input 
      id="roIp"
      type="text"
      value="읽기만 가능, 전송됨"
      readonly
    ><br>
    <label for="rqIp">required</label> <br>
    <input 
      id="rqIp"
      type="text"
      placeholder="필수입력!"
      required
    ><br>
    <label for="daIp">disabled</label> <br>
    <input 
      id="daIp"
      type="text"
      placeholder="입력불가, 전송 안됨"
      disabled
    ><br>
    <input
      type="radio"
      name="fruit"
      id="f_apple"
      value="apple"
      checked
    >
    <label for="f_apple">사과</label>
    <input
      type="radio"
      name="fruit"
      id="f_grape"
      value="grape"
    >
    <label for="f_grape">포도</label>
    <input
      type="radio"
      name="fruit"
      id="f_orange"
      value="orange"
      disabled
    >
    <label for="f_orange">오렌지(품절)</label>
    <button type="submit">제출</button>
    <button type="reset">초기화</button>
    </fieldset>
  </form>
