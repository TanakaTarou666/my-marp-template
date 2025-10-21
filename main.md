---
marp: true
size: 16:9
paginate: true
math: katex
theme: custom-theme
---

# タイトルページ
作者：たなかたろう

---

<figure class="center caption">
  <img src="./img/sample.png" style="width: 500px; border: 1px solid black;" />
  <figcaption>画像はcssを使用することで柔軟にカスタマイズできます</figcaption>
</figure>

---

# 数式

インライン数式: $E=mc^2$

ブロック数式:
$$
\begin{align*}
\int_0^\infty e^{-x^2} dx &= \frac{\sqrt{\pi}}{2} (\text{tex表記で書ける})
\end{align*}
$$

<div>

$$
\begin{align*}
\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2} \\
\end{align*}
$$
divなどのhtml表記内の中で，書くときは一行改行して書く
</div>

---

# 表

<table>
<caption>表もCSSで書くと柔軟にカスタマイズできます</caption>
  <thead>
    <tr>
      <th></th>
      <th>データA</th>
      <th>データB</th>
      <th>データC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>手法A</td>
      <td>0.650</td>
      <td>0.640</td>
      <td>0.380</td>
    </tr>
    <tr>
      <td>手法B</td>
      <td>0.682<br><span style="color:red;">(一番高い！)</span></td>
      <td>0.667</td>
      <td>0.455</td>
    </tr>
    <tr>
      <td>手法C</td>
      <td>0.612</td>
      <td>0.598</td>
      <td>0.410</td>
    </tr>
  </tbody>
</table>

---

# 追加の機能1 横並びのレイアウト

<div class="flex sa items-center">
    <div>
        横並びで表示できる
    </div>
    <div>
       <figure class="center caption">
            <img src="./img/sample.png" style="width: 300px; border: 1px solid black;" />
            <figcaption>画像</figcaption>
        </figure>
    </div>
</div>

---

# 追加の機能2 ブロック

<div class="box">
  <div class="box-title">ブロック表示</div>
  <div class="box-content">
    texのブロックを真似して作った
  </div>
</div>

<div class="box">
  <div class="box-title">横並びレイアウト＋ブロック表示</div>
  <div class="box-content flex sa items-center">
    <p>合わせ技も可能</p>
    <figure class="center caption">
      <img src="./img/sample.png" style="width: 250px; border: 1px solid black;" />
      <figcaption>画像</figcaption>
    </figure>
  </div>
</div>