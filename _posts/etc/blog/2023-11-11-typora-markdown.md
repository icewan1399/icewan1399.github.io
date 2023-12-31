---
title:  "[Blog] Typora Markown 정리" 
excerpt: "Typora의 Markdown Reference내용을 정리하였습니다."

categories:
  - ETC
  - Blog

tags:
  - [ETC, Blog, Typora, Markdown, Markdown Reference]

date: 2023-11-11
last_modified_at: 2023-11-17
---

타이포라를 사용하여 블로그를 작성할 계획이기 때문에 타이포라 관련 마크다운 문법을 정리합니다.  
Typora 문서의 [Markdown-Reference](https://support.typora.io/Markdown-Reference/) 내용을 바탕으로 정리하였습니다.
{: .notice--info}

## 들어가기에 앞서

* 타이포라 에디터 기준으로 작성한 마크 다운 언어이므로 다른 에디터에서는 안될수도 있습니다.
* 문서에서 보이는 Return은 Enter를 의미하므로 Enter로 표기합니다.
* 블로그 작성에 사용할 문법만 정리했습니다.

## 단락

* Enter키로 단락을 구분할 수 있으며 소스 코드로는 두 개 이상의 빈 줄(Enter)로 구분됩니다.

```html
이렇게

단락이 나누어집니다.
```
이렇게

단락이 나누어집니다.

## 줄 바꿈

* Shift + Enter로 한 줄 바꿈 가능
* 다른 마크다운에서 파서에서 무시할 수 있으므로 줄 끝에 공백(space) 2칸을 남겨두거나 \<br/>을 삽입하는걸 추천

```html
뒤에 2칸 공백 있어요  
\<br/>로도 줄 바꾸기 가능<br/>
```

뒤에 2칸 공백 있어요  
\<br/>로도 줄 바꾸기 가능<br/>

## 제목

* 줄 시작부분에 # 를 1 ~ 6개를 사용합니다.
* #가 많을수록 제목이 작아집니다.

```html
### 이건 3개

#### 이건 4개

##### 이건 5개
```

### 이건 3개

#### 이건 4개

##### 이건 5개

## 인용부호

* \>  뒤에 인용 문구를 넣습니다.
* 제목과는 다르게 목록에서도 사용 가능합니다.

```html
> 제목처럼 하시면 됩니다.
> 여러줄을 연속적으로 사용하면 이렇게 되요

* > 목록에서도<br/>
   > 이렇게
   >
   > 됩니다.
```

> 제목처럼 하시면 됩니다.
> 여러줄을 연속적으로 사용하면 이렇게 되요

* > 목록에서도<br/>
   > 이렇게
   >
   > 됩니다.

## 목록

* *를 사용하면 순서가 지정되지 않는 목록이 생성되고 + 혹은 -도 가능해요
* +나 -를 사용하면 *와 다른 모양의 순서가 지정되지 않는 목록이 생성됩니다.
* 숫자 + .를입력하면 해당 숫자부터 목록이 생성됩니다.
* 단축키로 tab을 누르면 하위 목차가 생기고 shift + tab을 누르면 상위 목차로 다시 돌아갑니다.

```html
* 이건 *
* 이건 *
+ 이건 + 
- 이건 - 



1. 처음만 번호를 입력하면 에디터에서



2. 자동으로
3. 숫자를 매겨줍니다.



12. 1이 아닌 숫자로도
13. 시작할 수 있어요



* 이렇게 
  * tab을 사용해서
    * 하위 목차를
      * 만들 수 있구요 



1. 이렇게
   1. 하위 목차에서
      1. 상위 목차로 다시
      2. 돌아가고 싶다면
   2. shift + tab 

```

* 이건 *
* 이건 *
+ 이건 +
- 이건 -



1. 처음만 번호를 입력하면 에디터에서



2. 자동으로
3. 숫자를 매겨줍니다.



12. 1이 아닌 숫자로도
13. 시작할 수 있어요



* 이렇게 
  * tab을 사용해서
    * 하위 목차를
      * 만들 수 있구요 



1. 이렇게
   1. 하위 목차에서
      1. 상위 목차로
      2.  돌아가고 싶다면
   2. shift + tab 

## 작업 목록

- \* \[ ]또는\* \[x]로 작업 목록을 표시할 수 있고 *는 +나 -로도 대체됩니다.

```
* [ ] 식사
  * [x] 아침
  * [ ] 점심
  * [x] 저녁
* [x] 공부
  * [x] C++
  * [x] 언리얼
```

* [ ] 식사
  * [x] 아침
  * [ ] 점심
  * [x] 저녁
* [x] 공부
  * [x] C++
  * [x] 언리얼

## 코드 블록

- \`\`\` + 언어 형식을 입력하면 언어에 맞게 구문을 강조해줍니다.
- 언어 형식을 생략해도 블록 자체는 만들 수 있습니다.

\`\`\`html <br/>
이게 \<br/\><br/>
html형식으로 생성된\<br/\><br/>
코드 블록입니다.\<br/\><br/>
\`\`\`

```html
이게 <br/>
html형식으로 생성된<br/>
코드 블록입니다.<br/>
```

## 테이블

- 코드로도 가능하지만 타이포라에서 지원하는 GUI(ctrl + t)를 사용하여 생성하는걸 권장합니다.
- 테이블안에 링크, 기울임, 취소선과 같은 인라인 마크다운을 사용할 수 있습니다.
- 머리글에 있는 행에 :을 포함하여 열의 텍스트를 원하는 방향으로 정렬할 수 있습니다.

```html
| 왼쪽 정렬 | 가운데 정렬 | 오른쪽 정렬 |
| :-------- | :---------: | ----------: |
| 1, 1      |    1, 2     |        1, 3 |
| 2, 1      |    2, 2     |        2, 3 |
```



| 왼쪽 정렬 | 가운데 정렬 | 오른쪽 정렬 |
| :-------- | :---------: | ----------: |
| 1, 1      |    1, 2     |        1, 3 |
| 2, 1      |    2, 2     |        2, 3 |

## 각주

- 각주를 등록하고 고유 식별 기호를 사용하여 표시할 수 있습니다.
- 양식은 \[\^고유기호(한글x)\]: 각주에 표시되는 텍스트
- 등록한 각주는 포스트 맨 아래에 표시되며 등록하는 위치는 상관없습니다.

```html
각주를 등록했다면 고유식별 번호를 사용해  이렇게 각1[^fn1] , 각2[^fn2] 표현할 수 있습니다.

[^fn1]: 이건 각주1 입니다.
[^fn2]: 이건 각주2 입니다.
```
각주를 등록했다면 고유식별 번호를 사용해  이렇게 각1[^fn1] , 각2[^fn2] 표현할 수 있습니다.

[^fn1]: 이건 각주1 입니다.
[^fn2]: 이건 각주2 입니다.

## 수평선

- 빈 줄에 --- 또는 ***를 입력하고 엔터를 누르면 수평선이 그려집니다.

```html
***
---
```

***
---

## 링크

- 링크는 3가지 종류(인라인, 내부, 참조)가 있습니다.
- 참조 링크는 다른 링크의 기능으로도 대체되기 때문에 제외하였습니다.
- 제가 정리한 두 형태의 링크는 공통적으로 \[제목\]\(주소\) 형태를 가집니다.

### 인라인 링크

- (주소) 부분에 url을 입력하여 특정 페이지로 연결합니다.
- 추가적으로 (주소) 부분에 "제목"으로 문자열을 넣어 링크에 제목을 포함할 수 있습니다

```html
이건 마우스를 올리면 [블로그](https://icewan1399.github.io/ "블로그 홈") 링크의 제목이 나와요 

이건 [블로그](https://icewan1399.github.io/) 제목을 제거한 형태입니다.
```

이건 마우스를 올리면 [블로그](https://icewan1399.github.io/ "블로그 홈") 링크의 제목이 나와요 

이건 [블로그](https://icewan1399.github.io/) 제목을 제거한 형태입니다.

### 내부 링크

- (주소)부분에 \(\# + 포스트의 제목중 하나\)를 넣어 포스트에 다른 영역으로 이동합니다.
- 제목 사이에 공백이 있다면 그 자리에 -를 넣어줍니다.

```html
[처음으로 돌아가기](#들어가기에-앞서)
```

[처음으로 돌아가기](#들어가기에-앞서)

## 기울이기

- *나 _을 사용하여 텍스트를 기울입니다.
- 타이포라에서는 * 사용을 권장합니다.

```html
*기울이기* 비교 : 기울이기
```

*기울이기*  비교 : 기울이기

## 굵게

- **나 __을 사용하여 텍스트를 굵게 표시합니다.
- 타이포라에서는 * *사용을 권장합니다.

```html
**굵게** 비교 : 굵게
```

**굵게** 비교 : 굵게

## 코드

- 코드 블럭과 다르게 단락 내의 코드를 표현할 때 사용합니다.
- ``를 사용해 표시합니다.

```html
`printf()` 함수
```

`printf()` 함수

## 취소선

- \~\~텍스트\~\~를 사용해 취소선을 표현합니다.

```html
~~텍스트~~
```

~~텍스트~~

## 이모티콘

- \: 이후 이모티콘 이름을 입력하여 표시할 수 있습니다.
- 타이포라의 편집 -> 이모지 및 기호(win + .)을 통해서도 입력 가능합니다.

```html
:heavy_check_mark:

✔
```

:heavy_check_mark:

✔

## 밑줄

- html 태그를 사용하여 밑줄을 생성할 수 있습니다.
-  \<u>텍스트\</u>로 표시합니다.

```html
<u>텍스트</u>
```

<u>텍스트</u>

---
