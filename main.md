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

# 画像

<figure class="center caption">
  <img src="./img/sample.png" style="width: 200px; border: 1px solid black;" />
  <figcaption>画像はcssを使用することで柔軟にカスタマイズできます</figcaption>
</figure>

<div style="display: flex; justify-content: space-around; align-items: flex-start; gap: 10px;">
  <figure style="text-align: center;">
    <img src="./img/sample.png" style="width: 200px; border: 1px solid black;" />
    <figcaption>画像1</figcaption>
  </figure>

  <figure style="text-align: center;">
    <img src="./img/sample.png" style="width: 200px; border: 1px solid black;" />
    <figcaption>画像2</figcaption>
  </figure>
  
  <figure style="text-align: center;">
    <img src="./img/sample.png" style="width: 200px; border: 1px solid black;" />
    <figcaption>画像3</figcaption>
  </figure>
</div>

<figure class="center caption">
横並びの画像表示例
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
divなどのhtml表記内の中で数式を書くときは一行改行する
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

<div class="columns">
    <div class="col">

### 左のコンテンツ
- 通常は左寄せ
    </div>
    <div class="col items-center">

### 右のコンテンツ
items-center クラスを使うと<br>中央寄せになる
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
  <div class="box-content">
    <div class="columns">
        <div class="col items-center">
            <ul>
                <li>合わせ技も可能</li>
                <li>中央寄せver</li>
            </ul>
        </div>
        <div class="col items-center">
            <figure class="center caption">
            <img src="./img/sample.png" style="width: 250px; border: 1px solid black;" />
            <figcaption>画像</figcaption>
            </figure>
        </div>
    </div>
  </div>
</div>

