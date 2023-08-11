# MarkDown Study

### *그 외 편리한 기능 정리*
- VScode에서 Preview 띄우기 > shitf + command + v
- Header로 이동 > shitf + command + o
- 공백나타내기 > br 태그 사용 
---
## underline : ___  3번
___
# Header1 
## Header2
### Header3
#### Header4
##### Header5
###### Header6


default
___
## Emphasis 
*이텔릭체* _언더바_

**bold** __언더바__

~~취소선~~
___
## list 
1. 순서가 필요한 목록
2. 순서
3. 순서
    1. 탭으로 구분이 필요하다.
        - 서브1
        - 서브2

- 순서가 필요하지 않은 목록에 사용 가능한 기호
    - 대쉬
    * 별표
    + 더하기
___
## link
[google](https://google.com)

[naver](https://naver.com "링크 설명(title) 작성")

[상대적 참조](/Users/ds)

[Dribbble][Dribbble link]

[GitHub][1]

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

다음과 같이 문서 내 일반 URL이나 꺾쇠 괄호(`< >`, Angle Brackets)안의 URL은 자동으로 링크를 사용합니다.
구글 홈페이지: https://google.com
네이버 홈페이지: <https://naver.com>

[Dribbble link]: https://dribbble.com
[1]: https://github.com
[참조 링크]: https://naver.com "네이버로 이동합니다!"
___
##  Image(이미지)
![대체 텍스트 입력](http://www.gstatic.com/webp/gallery/5.jpg "링크 설명(title) 작성")

![Kayak][logo]

[logo]: http://www.gstatic.com/webp/gallery/2.jpg "To go kayaking."

- **Local 사진 복사해서 붙여넣으면 바로 사진 띄어짐**
- **사진도 깃허브에 같이 올려야 함**
![Alt text](<Screenshot 2023-07-05 at 11.25.29 PM-1.png>)

- 이미지 크기 조정하기 
    - HTML 태그를 사용하여 크기를 조정할 수 있다.
```html
<img src="IMG_3249.PNG" alt="전체그림" width="300">
<img src="work_png/1.png" alt="전체그림" width="500">
```     
___
## 코드 강조 
 - `강조할 단어를` 입력, 주의할 점은 영문일때만 ₩ 가 `로 표시된다.
```
if [ -f ~/Library/KeyBindings/DefaultkeyBinding.dict ]; then
    echo "~/Library/KeyBindings/DefaultkeyBinding.dict already exists"
fi

mkdir -p ~/Library/KeyBindings
cat << EOF > ~/Library/KeyBindings/DefaultkeyBinding.dict 
{
    "₩" = ("insertText:", "\`");
}
EOF

echo "Done."
```

- 터미널에서 아래의 명령어를 입력 후 재부팅하면 grave 문자를 한글일때도 쓸 수 있음.

- `코드 강조 : ``` code block ``` `

```html
<a href="https://www.google.co.kr/" target="_blank">GOOGLE</a>
```

```css
.list > li {
  position: absolute;
  top: 40px;
}
```

```javascript
function func() {
  var a = 'AAA';
  return a;
}
```

```bash
$ vim ./~zshrc
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting. 
But let's throw in a tag.
```

 - 옆에 코드 이름을 쓰면 해당 코드에 맞게 색깔 변환

    - ex) ```java
___
## Table
| ep_no | salary | hire_date|
|:---:|:---:|:---:|
|1|100|~|
|1|200|~|
|2|300|~|
|3|400|~|
|4|100|~|

- `| id | name |` 를 통해 attribute설정
- 그 후 `|:---:|:---|` 를 사용해 튜플과 구분, :를 통해 정렬 가능
- 튜플 : `|eh|ho|`
___
## BlockQuote(인용문)
인용문(blockQuote)

> 남의 말이나 글에서 직접 또는 간접으로 따온 문장.
> _(네이버 국어 사전)_

> 인용문을 작성하세요!
>> 중첩된 인용문(nested blockquote)을 만들 수 있습니다.
>>> 중중첩된 인용문 1
>>> 중중첩된 인용문 2
>>> 중중첩된 인용문 3
___











