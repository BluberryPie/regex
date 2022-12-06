# 1. Character Classes

## 1. 문자열 그대로

특정 문자열을 그대로(exactly) 매칭하고 싶은 경우

**Regex** → (문자열 그대로)

(예시 1.)

**`/reg/g`**

> A `reg`ular expression (shortened as `reg`ex or `reg`exp; sometimes referred to as rational expression) is a sequence of characters that specifies a search pattern in text.

(예시 2.)

**`/텍스트/g`**

> 정규 표현식이라는 문구는 일치하는 `텍스트`가 준수해야 하는 "패턴"을 표현하기 위해 특정한 표준의 `텍스트` 신택스를 의미하기 위해 사용된다.

---

## 2. 아무 Character

개행(Newline)을 제외한 모든 문자를 매칭

**Regex** → `.`

**`/./g`**

> `A` `·` `r` `e` `g` `u` `l` `a` `r` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `·` `(` `s` `h` `o` `r` `t` `e` `n` `e` `d` `·` `a` `s` `·` `r` `e` `g` `e` `x` `·` `o` `r` `·` `r` `e` `g` `e` `x` `p` `;` `·` `s` `o` `m` `e` `t` `i` `m` `e` `s` `·` `r` `e` `f` `e` `r` `r` `e` `d` `·` `t` `o` `·` `a` `s` `·` `r` `a` `t` `i` `o` `n` `a` `l` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `)` `·` `i` `s` `·` `a` `·` `s` `e` `q` `u` `e` `n` `c` `e` `·` `o` `f` `·` `c` `h` `a` `r` `a` `c` `t` `e` `r` `s` `·` `t` `h` `a` `t` `·` `s` `p` `e` `c` `i` `f` `i` `e` `s` `·` `a` `·` `s` `e` `a` `r` `c` `h` `·` `p` `a` `t` `t` `e` `r` `n` `·` `i` `n` `·` `t` `e` `x` `t` `.`

---

## 3. 단어, 숫자, 공백

Word Character(영문, 숫자, underscore)에 해당하는 모든 문자를 매칭

**Regex** → `\w`

**`/\w/g`**

> `A`   `r` `e` `g` `u` `l` `a` `r`·`e` `x` `p` `r` `e` `s` `s` `i` `o` `n`·`(` `s` `h` `o` `r` `t` `e` `n` `e` `d`·`a` `s`·`r` `e` `g` `e` `x`·`o` `r`·`r` `e` `g` `e` `x` `p` `;`·`s` `o` `m` `e` `t` `i` `m` `e` `s`·`r` `e` `f` `e` `r` `r` `e` `d`·`t` `o`·`a` `s`·`r` `a` `t` `i` `o` `n` `a` `l`·`e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `)`·`i` `s`·`a`·`s` `e` `q` `u` `e` `n` `c` `e`·`o` `f`·`c` `h` `a` `r` `a` `c` `t` `e` `r` `s`·`t` `h` `a` `t`·`s` `p` `e` `c` `i` `f` `i` `e` `s`·`a`·`s` `e` `a` `r` `c` `h`·`p` `a` `t` `t` `e` `r` `n`·`i` `n`·`t` `e` `x` `t`.
