# 1. Character Classes

## 1. 문자열 그대로

특정 문자열을 그대로(exactly) 매칭하고 싶은 경우

**Regex** → (문자열 그대로)

**(예시 1.)** 정규표현식 = **`/reg/g`**

\[원문\]
> A regular expression (shortened as regex or regexp; sometimes referred to as rational expression) is a sequence of characters that specifies a search pattern in text.

\[매칭 결과\]
> A `reg`ular expression (shortened as `reg`ex or `reg`exp; sometimes referred to as rational expression) is a sequence of characters that specifies a search pattern in text.

**(예시 2.)** 정규표현식 = **`/텍스트/g`**

\[원문\]
> 정규 표현식이라는 문구는 일치하는 텍스트가 준수해야 하는 "패턴"을 표현하기 위해 특정한 표준의 텍스트 신택스를 의미하기 위해 사용된다.

\[매칭 결과\]
> 정규 표현식이라는 문구는 일치하는 `텍스트`가 준수해야 하는 "패턴"을 표현하기 위해 특정한 표준의 `텍스트` 신택스를 의미하기 위해 사용된다.

---

## 2. 아무 Character

개행(Newline)을 제외한 모든 문자를 매칭

**Regex** → `.`

**(예시 1.)** 정규표현식 = **`/./g`** (`space` → `·`으로 표현)

\[원문\]
> A regular expression (shortened as regex or regexp; sometimes referred to as rational expression) is a sequence of characters that specifies a search pattern in text.

\[매칭 결과\]
> `A` `·` `r` `e` `g` `u` `l` `a` `r` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `·` `(` `s` `h` `o` `r` `t` `e` `n` `e` `d` `·` `a` `s` `·` `r` `e` `g` `e` `x` `·` `o` `r` `·` `r` `e` `g` `e` `x` `p` `;` `·` `s` `o` `m` `e` `t` `i` `m` `e` `s` `·` `r` `e` `f` `e` `r` `r` `e` `d` `·` `t` `o` `·` `a` `s` `·` `r` `a` `t` `i` `o` `n` `a` `l` `·` `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` `)` `·` `i` `s` `·` `a` `·` `s` `e` `q` `u` `e` `n` `c` `e` `·` `o` `f` `·` `c` `h` `a` `r` `a` `c` `t` `e` `r` `s` `·` `t` `h` `a` `t` `·` `s` `p` `e` `c` `i` `f` `i` `e` `s` `·` `a` `·` `s` `e` `a` `r` `c` `h` `·` `p` `a` `t` `t` `e` `r` `n` `·` `i` `n` `·` `t` `e` `x` `t` `.`

---

## 3. 단어, 숫자, 공백

**3-1.** Word Character(영문, 숫자, underscore)에 해당하는 모든 문자를 매칭

**Regex** → `\w`

**(예시 1.)** 정규표현식 = **`/\w/g`** (`space` → `_`으로 표현)

\[원문\]
> A regular expression (shortened as regex or regexp; sometimes referred to as rational expression) is a sequence of characters that specifies a search pattern in text.

\[매칭 결과\]
> `A` _ `r` `e` `g` `u` `l` `a` `r` _ `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` _ ( `s` `h` `o` `r` `t` `e` `n` `e` `d` _ `a` `s` _ `r` `e` `g` `e` `x` _ `o` `r` _ `r` `e` `g` `e` `x` `p` ; _ `s` `o` `m` `e` `t` `i` `m` `e` `s` _ `r` `e` `f` `e` `r` `r` `e` `d` _ `t` `o` _ `a` `s` _ `r` `a` `t` `i` `o` `n` `a` `l` _ `e` `x` `p` `r` `e` `s` `s` `i` `o` `n` ) _ `i` `s` _ `a` _ `s` `e` `q` `u` `e` `n` `c` `e` _ `o` `f` _ `c` `h` `a` `r` `a` `c` `t` `e` `r` `s` _ `t` `h` `a` `t` _ `s` `p` `e` `c` `i` `f` `i` `e` `s` _ `a` _ `s` `e` `a` `r` `c` `h` _ `p` `a` `t` `t` `e` `r` `n` _ `i` `n` _ `t` `e` `x` `t`.

**3-2.** 숫자에 해당하는 모든 문자를 매칭

**Regex** → `\d`

**(예시 1.)** 정규표현식 = **`/\d/g`** (`space` → `_`으로 표현)

\[원문\]
> 몬트리올 지하철은 1966년 10월 14일에 장 드라포 시장이 건축 양식과 전동차에 있어서 파리 지하철에 영감을 받아 지어졌으며 첫 개통 당시 3개 노선 26개 역으로 시작하여 2019년 기준 4개 노선 68개 역으로 확장하였으며, 총연장은 71km이다. 세인트로렌스강을 하저터널로 건너 롱괴유에 지하철역이 하나 있고 가장 최근인 2007년에 연장된 라발에는 3개의 역이 있다. 

\[매칭 결과\]
> 몬트리올 지하철은 `1` `9` `6` `6`년 `1` `0`월 `1` `4`일에 장 드라포 시장이 건축 양식과 전동차에 있어서 파리 지하철에 영감을 받아 지어졌으며 첫 개통 당시 `3`개 노선 `2` `6` 개 역으로 시작하여 `2` `0` `1` `9`년 기준 `4`개 노선 `6` `8`개 역으로 확장하였으며, 총연장은 `7` `1`km이다. 세인트로렌스강을 하저터널로 건너 롱괴유에 지하철역이 하나 있고 가장 최근인 `2` `0` `0` `7`년에 연장된 라발에는 `3`개의 역이 있다.

**3-3.** 공백(Whitespace)에 해당하는 모든 문자를 매칭

**Regex** → `\s`

**(예시 1.)** 정규표현식 = **`/\s/g`** (`space` → `_`으로 표현)

\[원문\]
> 예술(藝術)은 학문·종교·도덕 등과 같은 문화의 한 부문으로, 예술 활동(창작, 감상)과 그 성과(예술 작품)의 총칭이다.

\[매칭 결과\]
> 예술(藝術)은 `_` 학문·종교·도덕 `_` 등과 `_` 같은 `_` 문화의 `_` 한 `_` 부문으로, `_` 예술 `_` 활동(창작, `_` 감상)과 `_` 그 `_` 성과(예술 `_` 작품)의 `_` 총칭이다.