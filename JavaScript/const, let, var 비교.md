## ๐งฒ const, let, var ๋น๊ต

> #### ์์ฝ
>
> - var ๋ณด๋ค๋ let ๊ณผ const ๋ฅผ ์ฌ์ฉ
> - ๋ณ๊ฒฝํ์ง ์๋ ๊ฐ(์์)์ด๋ผ๋ฉด let ๋ณด๋ค๋ const ๋ฅผ ์ฌ์ฉํ๋ ๊ฒ์ด ์์ 

> #### ์ฐธ๊ณ ) ์ฝ๋๋ธ๋ก & ๋ธ๋ก ๋ ๋ฒจ ์ค์ฝํ
>
> ํจ์, if, for, while, try/catch ๋ฑ

### var

- ๋ฌธ์ ์ : ํจ์ ์ฝ๋ ๋ธ๋ก๋ง ์ง์ญ ์ค์ฝํ๋ก ์ธ์ ํจ
  - ๋ฐ๋ผ์ ์ค๋ก์ง ํจ์ ์ฝ๋ ๋ธ๋ก๋ง์ ์ง์ญ ์ค์ฝํ๋ก ์ธ์ ํ๋ `var` ๋์ , ๋ธ๋ก ๋ ๋ฒจ ์ค์ฝํ๋ฅผ ์ง์ํ๋ `const`์ `let`์ ์ฌ์ฉํ๋ ๊ฒ์ ๊ถ์ฅ

### let

- ๋ณ์ ์ฌํ ๋น ๊ฐ๋ฅ (์ค๋ณต ์ ์ธ์ let, const ๋ชจ๋ ๋ถ๊ฐ)

```javascript
let name = 'kmj'
console.log(name) // output: kmj

let name = 'howdy' // ์ฌํ ๋น ๋ถ๊ฐ output: Uncaught SyntaxError: Identifier 'name' has already been declared

name = 'howdy'
console.log(name) // output: howdy
```



### const

- ๋ฐ๋์ ์ ์ธ๊ณผ ์ด๊ธฐํ๋ฅผ ๋์์ ํด์ผํ๋ค.
- let๊ณผ ๋ฌ๋ฆฌ ๋ณ์ ์ฌํ ๋น ๋ถ๊ฐ๋ฅ

```javascript
// ์์๊ฐ์ ์ฌํ ๋น
const name = 'kmj'
name = 'howdy' // output: Uncaught TypeError: Assignment to constant variable.

// ๊ฐ์ฒด์ ์ฌํ ๋น
const name = {
  eng: 'kmj',
}
name.eng = 'howdy'

console.log(name) // output: { eng: "howdy" }
```





