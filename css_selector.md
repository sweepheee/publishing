CSS 선택자와 선택자의 우선순위
=================



CSS 속성으로 선택하기
-----

```

<style>


  /* .list 바로 밑의 li 다음의 모든 li. 즉, .list 아래의 첫번째 li를 제외한 다음 모든 li를 선택할 수 있다. */
  .list li + li {
    background-color: black;
  }

  /* 태그[속성명] 선택자로 CSS적용 가능하다. */
  a[href] {
    background-color: red;
  }
  
  /* 태그[속성명=value] 선택자로 value값을 선택할 수 있다. */
  a[href="http://www.naver.com"] {
    background-color: blue;
  }
  
  /* 태그[href ^= "http://"] href속성이 http://로 시작하는 태그를 선택 */
  a[href ^= "http://"] {
    background-color: lime;
  }
  
  /* 태그[href $= ".pdf"] href속성이 .pdf로 끝나는 태그를 선택 */
  a[href $= ".pdf"] {
    background-color: yellow;
  }
  
  /* 태그[속성명 ~= value] 선택자로 해당 속성안에 value값의 문장을 가진 태그의 선택이 가능하다 */
  li[title = "text"] {
    background-color: green;
  }
  
  /* 태그[속성명 *= value] 선택자로 해당 속성안에 value값이 하나라도 포함되어 있을 경우 선택이 가능하다 */
  li[title = "te"] {
    background-color: cyan;
  }
</style>

```

link
