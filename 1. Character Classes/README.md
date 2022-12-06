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

(예시 1.) : `space` → `·`으로 표현

**`/./g`**

> `A` `·` `r` `e` `g` `u` `l` `a` `r` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `·` `(` `s` `h` `o` `r` `t` `e` `n` `e` `d` `·` `a` `s` `·` `r` `e` `g` `e` `x` `·` `o` `r` `·` `r` `e` `g` `e` `x` `p` `;` `·` `s` `o` `m` `e` `t` `i` `m` `e` `s` `·` `r` `e` `f` `e` `r` `r` `e` `d` `·` `t` `o` `·` `a` `s` `·` `r` `a` `t` `i` `o` `n` `a` `l` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `)` `·` `i` `s` `·` `a` `·` `s` `e` `q` `u` `e` `n` `c` `e` `·` `o` `f` `·` `c` `h` `a` `r` `a` `c` `t` `e` `r` `s` `·` `t` `h` `a` `t` `·` `s` `p` `e` `c` `i` `f` `i` `e` `s` `·` `a` `·` `s` `e` `a` `r` `c` `h` `·` `p` `a` `t` `t` `e` `r` `n` `·` `i` `n` `·` `t` `e` `x` `t` `.`

---

## 3. 단어, 숫자, 공백

Word Character(영문, 숫자, underscore)에 해당하는 모든 문자를 매칭

**Regex** → `\w`

(예시 1.) : `space` → `_`으로 표현

**`/\w/g`**

> `A` _ `r` `e` `g` `u` `l` `a` `r` _ `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` _ `(` `s` `h` `o` `r` `t` `e` `n` `e` `d` _ `a` `s` _ `r` `e` `g` `e` `x` _ `o` `r` _ `r` `e` `g` `e` `x` `p` `;` _ `s` `o` `m` `e` `t` `i` `m` `e` `s` _ `r` `e` `f` `e` `r` `r` `e` `d` _ `t` `o` _ `a` `s` _ `r` `a` `t` `i` `o` `n` `a` `l` _ `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `)` _ `i` `s` _ `a` _ `s` `e` `q` `u` `e` `n` `c` `e` _ `o` `f` _ `c` `h` `a` `r` `a` `c` `t` `e` `r` `s` _ `t` `h` `a` `t` _ `s` `p` `e` `c` `i` `f` `i` `e` `s` _ `a` _ `s` `e` `a` `r` `c` `h` _ `p` `a` `t` `t` `e` `r` `n` _ `i` `n` _ `t` `e` `x` `t`.
