---
title: '2장 - Python의 기본'
description:
  '2장에서는 Python의 기본 개념을 다룹니다.'
prev: null
next: /chapter3
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

<exercise id="6" title="숫자 자료형" type="choice">
  <h2>자료형의 파악</h2> <br/>

  <p>
    숫자는 정수(<code>integer</code>)와 부동소수(<code>floating point number</code>)로 표현될 수 있습니다. 쉽게는 소수점이 있고 없고 정도의 차이가 있다고 생각해볼 수 있습니다. 파이썬에서는 이 둘의 자료형을 <code>int</code>, <code>float</code> 라는 키워드로 규정하고 있습니다.
  </p>

  <p>
    <code>type</code> 함수를 이용하면, 값 또는 변수(에 포함된 값)의 자료형이 어떤것인지 손쉽게 알아내는것이 가능합니다. 아래의 연습문제를 통해서, <code>type</code> 함수의 사용법을 익혀보겠습니다.
  </p>

  <codeblock id="02_05">
    힌트 없음
  </codeblock>

  <p>
    아래의 것들 중 부동소수가 아닌 것은 어떤것일까요?
  </p>

<choice>
<opt text="34.1"></opt>
<opt text="0.0"></opt>
<opt text="8" correct="true"></opt>
<opt text="99.99"></opt>
</choice>

  <h2>숫자 자료형에 사용 가능한 연산자</h2> <br/>
  <p>
    숫자 값들 끼리는 여러가지 연산자를 통해서, 여러가지 계산을 할 수 있습니다. 우리가 흔히 알고 있는 <code>+</code>(덧셈), <code>-</code>(뺄셈), <code>*</code>(곱셈), <code>/</code>(나눗셈)과 더불어 아래와 같이 보다 편리한 연산자를 제공합니다. 
  </p>

  <table>
    <tr>
      <th>연산자의 종류</th>
      <th>연산자의 의미</th>
    </tr>
    <tr>
      <th>A ** B</th>
      <th>A 값을 B 값만큼 거듭제곱된 값을 반환합니다</th>
    </tr>
    <tr>
      <th>A // B</th>
      <th>A 값을 B 값으로 나누고, 소수점 이하는 버려진 값을 반환합니다</th>
    </tr>
    <tr>
      <th>A % B</th>
      <th>A 값을 B 값으로 나누고, 나머지만을 취하여 반환합니다</th>
    </tr>
    <tr>
      <th>A ?= B</th>
      <th>? 에는 모든 연산자가 사용가능합니다. <br/> A와 B에대한 계산을 한 뒤 그 결과를 A에 담습니다. <br/>예를들어 A += B는 A+B 값을 A에 할당합니다</th>
    </tr>
  </table>

  <p>
    아래의 연습문제에서 <code>+=</code> 연산자를 이용하여 두 변수의 값을 서로 더한다음 화면에 출력해 보세요.
  </p>

  <codeblock id="02_06">
    힌트 없음
  </codeblock>

  <h2>숫자 자료형을 위해 제공되는 내장 함수/메서드</h2> <br/>
  <p>
    모든 숫자의 연산은 기본적인 연산자의 조합으로 충분히 가능하지만, 이미 널리 알려져서 많이 사용되는 연산 (로그, 반올림, 팩토리얼, 코사인, 등)을 위한 코드를 직접 작성하는것은 꽤 시간이 낭비되는 작업일 것입니다. Python는 이렇게 자주 사용되는 연산을 위한 내장된 방법을 함수와 같은 장치로서 제공합니다 (물론 제 3의 패키지를 활용할 수도 있습니다).
  </p>

  <table>
    <tr>
      <th>함수 종류</th>
      <th>함수의 의미</th>
    </tr>
    <tr>
      <th>abs(X)</th>
      <th>X의 절대값을 반환합니다</th>
    </tr>
    <tr>
      <th>round(X)</th>
      <th>X에 소수점 이하의 값을 반올림하여 반환합니다</th>
    </tr>
    <tr>
      <th>math.log(X)</th>
      <th>밑을 10으로 하는 로그를 X에 적용한 값을 반환합니다</th>
    </tr>
    <tr>
      <th>math.sin(X) | math.cos(X) | math.tan(X)</th>
      <th>각각 X에 대한 삼각함수를 적용한 값을 반환합니다</th>
    </tr>
    <tr>
      <th>math.fatorial(X)</th>
      <th>X의 계승 값을 계산하여 반환합니다</th>
    </tr>
    <tr>
      <th>math.exp(X)</th>
      <th>상수 e를 X만큼 거듭제곱한 값을 반환합니다</th>
    </tr>
    <tr>
      <th>math.sqrt(X)</th>
      <th>X의 제곱근 값을 계산하여 반환합니다</th>
    </tr>
  </table>  

  <p>
    아래의 연습문제에서 주어진 숫자에 대한 <code>절대값</code>, <code>로그</code>, <code>계승</code>, <code>제곱근</code> 값이 계산된 결과를 화면에 출력해 보세요.
  </p>

  <codeblock id="02_07">
    abs, math.log, math.factorial, math.sqrt
  </codeblock>
</exercise>

<exercise id="7" title="리스트 자료형">
  <h2>리스트 자료형의 단일 요소 접근</h2> <br/>

  <p>
    앞서 잠시 다뤄진 리스트(<code>list</code>)는 여러 데이터 뭉치를 논리적으로 모아서 관리하기 위한 자료형입니다. 이 때의 데이터 뭉치는 단일 자료형을 따를 수도 있지만, 서로 다른 자료형의 데이터를 섞어서 보관하는것도 가능합니다. 가령 <code>[1, "문자열", 1.1, ...]</code>과 같은 것이 가능하죠. 또한, 나중에 배우게될 <code>사용자 정의 자료형</code> 및 다양한 객체 또한 보관하는것이 가능합니다.
  </p>

  <p>
    리스트 자료형의 각 요소를 접근하는 방법은 <code>[ ]</code> 대괄호 연산자를 사용하는 것입니다. 가령 <code>리스트[0]<code> 과 같은 코드는 리스트의 첫 번째 요소를 접근할 수 있게 해줍니다. 0부터 시작됨에 주의하세요.
  </p>  

  <p>
    아래의 연습문제에서 주어진 리스트의 다섯번째 요소의 내용을 화면에 출력해보세요.
  </p>

  <codeblock id="02_08">
    대괄호 연산자를 사용해 보세요
  </codeblock>

  <h2>리스트 자료형을 위해 제공되는 메서드</h2> <br/>

  <p>
  d
  </p>
</exercise>