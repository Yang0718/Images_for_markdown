
# <center>Markdown
希臘字母、其他運算符號見此網頁：
http://jzqt.github.io/2015/06/30/Markdown中写数学公式/

## 方程式
左右放錢字號：<br>
$\int_0^3 \int_2^4 (xy+2x-y)\,dx\,dy$<br>
如果用兩個錢字號表示該方程式獨立一行且置中：<br>
$$\int_0^3 \int_2^4 (xy+2x-y)\,dx\,dy$$<br>
***
## 上下標
若上下標的內容超過一個字，就用{}包起來
$$x=a^n_{5y+2n}$$
<br>
兩邊都要上下標的話，用\sideset
$$\sideset{^1_2}{^3_4}A$$

## 大括號
因為{}本身有其他功能，所以在使用大括號{}時為了避免搞混，通常會寫成\lbrace \rbrace來替代<br>
$$f(x, y) = 100 * \lbrace[(x + y) * 3] - 5\rbrace$$

## 分數
\frac{分母}{分子}：$\frac{1}{3}$ <br>
改用\cfrac會讓數字不那麼擠：$\cfrac{1}{3}$<br>
***
## 開根號
\sqrt[根號次數]{被開方數}
$$\sqrt[3]{X}$$<br>
$$\sqrt{5 - x}$$

## 引用
>這裡放要引用的內容<br>
後面相鄰的行可以不用加>，一樣會變引用

## 列表&排序
這三種符號都可以：*,+,-
1. 第一層
    * 111
    + 222
    
2. 第二層
    - asdasd
    * oijiji3

## 刪除線
用~~把字包住<br>

~~這就是刪除線~~

## 超連結
打[要顯示的名字] (網址)<br>
[Google](http://www.google.com/)

## 程式碼
在句子裡添加程式碼，例如`print`，用反引號來包住
若要放多行程式碼，且讓程式碼變色，就要用三個反引號，並在第一行後面寫使用的語言：<br>
```python
x = symbols('x')
y = symbols('y')
```
## 粗體＆斜體
*HAHA*<br>
**HAHA**

## 表格
用---來分隔表頭與下方內容<br>
:--- 代表靠左<br>
:--: 代表置中<br>
---: 代表靠右<br>
此處在打最右邊的錢字號時，要先加個\，否則會變成方程式

| Tables | Are | Cool |
| ------- | :------: | -----:|
| col 3 is | right-aligned | \$1600 |
| col 2 is | centered | \$12 |
| zebra stripes | are neat | \$1 |

# 插入圖片的方法
先上傳到github，再引用該圖片連結(如果是網路上的就直接複製連結即可)
### 法一：markdown之引用<br>
後面放的title要滑鼠移過去才會顯示<br>
`![微積分](https://github.com/Yang0718/Images_for_markdown/raw/master/微積分符號.png "calculus for markdown")`<br>

### 法二：html之語法，可以改圖片大小<br>
指定圖片的大小百分比：width="40%"<br>
`<img src='https://github.com/Yang0718/markdown_notes/blob/master/微積分符號.png',width=200,height=200>`<br>
<img src='https://github.com/Yang0718/Images_for_markdown/raw/master/微積分符號.png'>
