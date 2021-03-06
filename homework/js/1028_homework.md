# 10.28 js_02

# JavaScript 기초

## 1. T/F

- let & const 키워드로 선언한 변수와 var 키워드로 선언한 변수의 유일한 차이점은 변수의 유효범위이다. **(F)** : + var 변수는 호이스팅이 된다.

-  “값이 없음”을 표현하는 값으로 null과 undefined 두 종류가 있으며, 둘 다 typeof 연산 자에서 undefined가 반환된다. **(F)** : null은 object 반환

-  for ... in 문은 배열의 요소를 직접 순회하므로 배열의 각 요소를 활용하는 경우에 주로 활용한다. **(F)**: for of 에 대한 설명이다.

- ‘==’ 연산자는 두 변수의 값과 타입이 같은지 비교하고 같다면 true 아니면 false를 반환한다 **(F)** : JS에선 같은지 비교하는 연산자가 '===' 이다.

- JavaScript에서 함수는 변수에 할당, 인자로 전달할 수 있으나 함수의 결괏값으로 반환할 수는 없다. **(T)**

  

## 2. 다음의 Array Helper Method의 동작을 간략히 서술하시오.

- map - 배열의 요소 하나하나에 함수를 적용시킨 결과를 반환한다.

- filter - 배열의 요소 중 조건에 맞는 요소들을 반환한다.

- every - 배열의 모든 요소의 함수 결과값이 true인지

- some - 배열의 요소 중 함수 결과값이 true인 것이 있는지

- reduce - 배열의 요소들에 함수를 적용하여 쌓아나간다..?

  

## 3. 아래의 숫자 배열에 map 함수를 사용하여, 모든 아이템에 3제곱을 한 새로운 배열을 만드는 코드를 작성하시오

```python
const nums = [1, 2, 3, 4]

const newNums = nums.map(function(x) {
  return x**3
})

// 화살표 함수
nums.map(x => x**3)
```

