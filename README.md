## 'card-ui-02'

<br>

### • 배포 주소: [https://card-ui-02.netlify.app/](https://card-ui-02.netlify.app/)

<br>

#### - 작업 기간: 2021.08

#### - 리팩토링: 2024.01

<br>

### 기술 스택

Development

<p>
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
</p>

Config

<p>
<img src="https://img.shields.io/badge/npm-CB3837?style=flat&logo=npm&logoColor=white"/></a>
</p>

Environment

<p>
<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat&logo=Visual Studio Code&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/></a>
<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/></a>
</p>
<br>

### 전체 페이지

<img src="https://github.com/azure0929/card-ui-02/assets/128226527/f48da2b4-3bb9-4147-8d9c-62f110ec8051" />

<br><br>

### 💻 주요 기능

---

- flex, counter-increment, content: counter

```html
<div class="item">
  <div class="photo">
    <a href="#none">
      <img src="images/item-01.jpg" alt="item1" />
      <img src="images/item-01-hover.jpg" alt="item1 hover" />
    </a>
  </div>
  <div class="detail">
    <span class="price"
      ><b>77<small>%</small></b> 159,000원</span
    >
    <span class="name">폭스 퍼 구스다운 후드 롱패딩</span>
    <span class="count">상품평 110</span>
  </div>
</div>
```

```css
.items {
  display: flex;
  gap: 20px;
  counter-reset: item;
}
.item {
  height: 400px;
  position: relative;
  flex: 1;
}
.item:before {
  counter-increment: item;
  content: counter(item);
  position: absolute;
  background-color: rgb(91, 69, 192);
  width: 45px;
  height: 45px;
  top: 0;
  left: 0;
  z-index: 10;
  font-size: 18px;
  color: #fff;
  text-align: center;
  line-height: 45px;
  transition: 0.35s;
}
.item:hover:before {
  background-color: crimson;
}
```
