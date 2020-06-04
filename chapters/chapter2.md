---
title: '2장 - Python의 기본'
description:
  '2장에서는 Python의 기본 개념을 다룹니다.'
prev: /chapter2
next: /chapter2
type: chapter
id: 1
---

<exercise id="1" title="화면에 글자 출력">
  <p>
    <code>print</code>는 화면에 글자를 출력하는 능력을 가진 함수입니다. 출력하고 싶은 글자를 따옴표 또는 쌍따옴표로 감싼 다음, ( ) 소괄호 속에 넣어주면 됩니다. 참고로 프로그래밍 언어에서, 글자 하나는 <code>문자</code>, 여러 글자의 집합은 <code>문자열</code> 이라고 부르는것이 일반적입니다.
  </p>

  <p>
    다음은 간단한 연습문제 입니다. <code>Hello</code>라는 문자열을 화면에 출력하기 위해서 사용해야 할 함수명을 _____ 에 입력한 다음, 『Run Code』 버튼을 클릭해서 결과를 확인해 보세요. 힌트를 보고 싶으면, 『힌트 보기』를, 정답을 보고 싶다면 『솔루션 보기』을, 코드 내용을 리셋시키고 싶다면 『코드 초기화』 를 클릭해 보세요.
  </p>

  <codeblock id="02_01">
    p로 시작합니다
  </codeblock>
</exercise>

<exercise id="2" title="변수">
  <p>
    문자열을 직접적으로 <code>print</code> 함수에 넣어줘도 되지만, 문자열을 담은 변수를 print 함수에 넣어줄 수도 있습니다. 변수가 글자 정보를 담아내고 있는것입니다. 변수를 사용해서 얻을 수 있는 장점은 변수명 만으로, 같은 값을 어디서든지 참조가 가능하다는 것입니다. 코드가 훨씬 간결해지고, 변수에 정보를 할당해주는 부분만 수정하면 코드 전역에 걸친 모든 값이 손댈 필요없이 수정됩니다. 
  </p>
  
  <p>
    다음 연습문제에서 <code>greeting</code> 이라는 변수에 <code>Hello Python from String!</code> 이라는 문자열을 담고, 해당 변수를 이용하여 화면 출력해 보세요.
  </p>

  <codeblock id="02_02">
    ddd
  </codeblock>  
</exercise>

<exercise id="3" title="for 반복문 (feat. range)">
  <p>
    <code>range</code>는 지정된 범위의 숫자들의 범위를 만들어줍니다. 예를 들어서, <code>range(0, 10)</code>과 같은 코드는 <code>0 ~ 9</code>까지의 범위를 표현합니다. 마지막 10이 포함되지 않는다는 사실에 주의하세요. <code>range</code>는 함수처럼 생겼지만, 사실은 <code>객체</code>라고 불리는 것입니다. 이 내용은 나중에 좀 더 자세히 살펴보겠습니다.
  </p>

  <p>
    <code>for</code> 반복문은 무언가를 순차적으로, 반복적으로 접근할 때 사용되는 문법입니다. 이 때 <code>range</code>를 함께 사용할 수 있는데요, 그러면 <code>range</code>가 표현하는 범위에 포함된 숫자들을 순차적으로 하나씩 접근하게 됩니다. 가령 <code>for number in range(0, 10)</code>과 같은 코드는 처음에는 0, 두 번째에는 1, ..., 마지막에는 9라는 숫자를 순차적으로 접근하여 <code>number</code> 라는 변수에 담아두게 됩니다. 
  </p>

  <p>
    <code>for</code> 반복문의 기본적인 형태는 <code>for 순차적_내용을_담을_변수 in 순차적으로_접근할_무언가</code> 입니다. 
  </p>

  <p>
    다음 연습문제에서 <code>range</code> 객체를 사용하여, 0부터 10까지의 숫자를 차례대로 화면에 출력하는 코드를 완성해 보세요.
  </p>

  <codeblock id="02_03">
    9까지가 아니라, 10까지 포함한다는 사실에 주의하세요.
  </codeblock> 
</exercise>

<exercise id="4" title="for 반복문 (feat. list)">
  <p>
    <code>list</code>는 <code>range</code>와 유사한 개념입니다 (내부적으로는 약간 다릅니다). <code>range</code>가 숫자 범위를 표현하는과는 달리, <code>list</code>는 모든 종류의 데이터를 표현하는것이 가능한 객체입니다. 가령 <code>[0, 1, 2]</code>와 같은 코드는 <code>0, 1, 2</code> 숫자 세개를 포함하는 <code>list</code>를 만들어줍니다. 또 다른 예로, <code>["아빠", "엄마", "딸"]</code>와 같은 코드는 세 개의 문자열을 포함하는 <code>list</code>를 만들어줍니다.
  </p>

  <p>
    <code>list</code>는 <code>range</code>와 마찬가지로, <code>for</code> 반복문에서 사용이 가능합니다. 가령 <code>for number in [0, 1, 2]</code>와 같은 코드는 <code>list</code>에 담긴 내용을 순차적으로 접근하여 <code>number</code>에 반복적으로 담아줍니다.
  </p>

  <p>
    다음 연습문제에서 <code>list</code> 객체를 이용하여, ["아빠", "엄마", "딸"]의 내용을 차례대로 화면에 출력하는 코드를 완성해 보세요.
  </p>

  <codeblock id="02_04">
    힌트 없음
  </codeblock>
</exercise>

<!-- <exercise id="1" title="Introduction" type="slides">

<slides source="chapter1_01_introduction">
</slides>

</exercise>

<exercise id="2" title="Getting Started">

Let's ask some questions about the slides. Whats the correct answer?

<choice>
<opt text="Answer one">

This is not the correct answer.

</opt>

<opt text="Answer two" correct="true">

Good job!

</opt>

<opt text="Answer three">

This is not correct either.

</opt>
</choice>

</exercise>

<exercise id="3" title="First steps">

This is a code exercise. The content can be formatted in simple Markdown – so
you can have **bold text**, `code` or [links](https://spacy.io) or lists, like
the one for the instructions below.

- These are instructions and they can have bullet points.
- The code block below will look for the files `exc_01_03`, `solution_01_03` and
  `test_01_03` in `/exercises`.

<codeblock id="01_03">

This is a hint.

</codeblock>

</exercise> -->
