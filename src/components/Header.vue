<template>
  <header id="header">
    <div class="header__inner">
      <div class="header__inner__port">
        <router-link to="/portfolio">Portfolio</router-link>
      </div>
      <div class="header__inner__logo">
        <router-link to="/">Inyoung</router-link>
      </div>
      <div class="header__inner__menu">
        <router-link to="#">
          <span class="sr-only">menu</span>
        </router-link>
      </div>
    </div>
    <div class="header__nav demo">
      <ul>
        <li>
          <router-link to="/about">About</router-link>
        </li>
        <li>
          <router-link to="/reference">Reference</router-link>
        </li>
        <li>
          <router-link to="/youtube">Youtube</router-link>
        </li>
        <li>
          <router-link to="/script">Script</router-link>
        </li>
        <li>
          <router-link to="/contact">Contact</router-link>
        </li>
      </ul>
      <ul>
        <li>
          <router-link to="/">회원가입</router-link>
        </li>
        <li>
          <router-link to="/">로그인</router-link>
        </li>
        <li>
          <router-link to="/">게시판</router-link>
        </li>
      </ul>
    </div>
    <div class="header__info" id="{info}">
      <div>
        <h4>email</h4>
        <p>
          <a href="mailto:webstoryboy@naver.com">webstoryboy@naver.com</a>
        </p>
      </div>
      <div>
        <h4>kakao</h4>
        <p>
          <a href="/">webstupids</a>
        </p>
      </div>
      <div>
        <h4>social</h4>
        <ul>
          <li>
            <a href="/">Youtube</a>
          </li>
          <li>
            <a href="/">Instargram</a>
          </li>
          <li>
            <a href="/">Github</a>
          </li>
          <li>
            <a href="/">Cafe</a>
          </li>
          <li>
            <a href="/">Referecne</a>
          </li>
          <li>
            <a href="/">Tutorials</a>
          </li>
          <li>
            <a href="/">CSS</a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
#header {
  overflow: hidden;
}
.header__inner {
  z-index: 1200;
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  color: #fff;
  border-bottom: 1px solid #2e2e30;
  display: flex;
  align-items: center;
  font-family: "Rajdhani", "Chosunilbo_myungjo";
  font-weight: 500;
  background: #000;
}
.header__inner__port {
  flex: 1 1 35%;
  padding-left: 1rem;
}
.header__inner__port a {
  position: relative;
  padding-left: 10px;
}
.header__inner__port a::before {
  content: "";
  width: 5px;
  height: 5px;
  background: #fff;
  position: absolute;
  left: 0;
  top: 3px;
  border-radius: 50%;
}
.header__inner__port a::after {
  content: "";
  width: 5px;
  height: 5px;
  background: #fff;
  position: absolute;
  left: 0;
  top: 11px;
  border-radius: 50%;
}
.header__inner__logo {
  flex: 1 1 30%;
  text-align: center;
  margin: 1.5rem;
}
.header__inner__logo a {
  font-family: "Playfair Display";
  font-size: 1.8rem;
  line-height: 1;
}
.header__inner__menu {
  flex: 1 1 35%;
  text-align: right;
  padding-right: 1rem;
}
.header__inner__menu a {
  display: inline-block;
  width: 40px;
  height: 40px;
  position: relative;
  margin-top: 5px;
}
.header__inner__menu a::before {
  content: "";
  position: absolute;
  left: 10px;
  top: 10px;
  width: 8px;
  height: 8px;
  background: #fff;
  box-shadow: 0 12px 0 #fff;
}
.header__inner__menu a::after {
  content: "";
  position: absolute;
  right: 10px;
  top: 10px;
  width: 8px;
  height: 8px;
  background: #fff;
  box-shadow: 0 12px 0 #fff;
}
.header__bg {
  z-index: 1100;
  position: fixed;
  left: 0;
  top: 0;
  width: 100vw;
  height: 100vh;
}
.header__bg > div {
  position: absolute;
  left: 0;
  top: 0;
  width: 10vw;
  height: 100vh;
  background: rgba(0, 0, 0, 0.83);
}
.header__bg > div:nth-child(1) {
  left: 0vw;
}
.header__bg > div:nth-child(2) {
  left: 10vw;
}
.header__bg > div:nth-child(3) {
  left: 20vw;
}
.header__bg > div:nth-child(4) {
  left: 30vw;
}
.header__bg > div:nth-child(5) {
  left: 40vw;
}
.header__bg > div:nth-child(6) {
  left: 50vw;
}
.header__bg > div:nth-child(7) {
  left: 60vw;
}
.header__bg > div:nth-child(8) {
  left: 70vw;
}
.header__bg > div:nth-child(9) {
  left: 80vw;
}
.header__bg > div:nth-child(10) {
  left: 90vw;
}
.header__nav {
  z-index: 1200;
  position: fixed;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: #fff;
  text-align: center;
}
.header__nav li a {
  font-family: "Saol Display Regular", "Chosunilbo_myungjo";
  font-size: 5vw;
  line-height: 1.2;
  font-weight: 100;
}
.header__nav ul:last-child li {
  display: inline-block;
  margin-top: 20px;
}
.header__nav ul:last-child li a {
  font-family: "Chosunilbo_myungjo";
  font-size: 16px;
  line-height: 1;
  padding: 10px;
}
.header__nav.demo {
  position: fixed;
  right: 60px;
  top: 16px;
  z-index: 1300;
  left: auto;
  transform: none;
  visibility: visible;
  text-align: right;
  display: flex;
  flex-direction: column-reverse;
}
.header__nav.demo li {
  display: inline;
  margin-top: 0;
}
.header__nav.demo li a {
  transform: translateY(0);
  font-family: "Rajdhani", "Chosunilbo_myungjo";
  font-size: 16px;
  font-weight: 400;
  padding: 2px 5px;
}
.header__nav.demo ul:last-child li {
  margin-top: 0;
}
.header__nav.demo ul:last-child li a {
  padding: 2px 5px;
}
.header__info {
  z-index: 1200;
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  color: #fff;
  border-top: 1px solid #2e2e30;
  display: flex;
  align-items: center;
  font-family: "Rajdhani", "Chosunilbo_myungjo";
  font-weight: 500;
  background: #000;
}
#none.header__info {
  display: none;
}
.header__info > div {
  text-align: center;
  padding: 30px;
}
.header__info > div h4,
.header__info > div p,
.header__info > div ul {
  display: inline-block;
}
.header__info > div h4 {
  font-family: "Rajdhani", "Chosunilbo_myungjo";
  font-weight: 500;
  opacity: 0.6;
  padding: 0 10px;
}
.header__info > div:nth-child(1) {
  flex: 1 1 25%;
  border-right: 1px solid #2e2e30;
}
.header__info > div:nth-child(2) {
  flex: 1 1 20%;
  border-right: 1px solid #2e2e30;
}
.header__info > div:nth-child(3) {
  flex: 1 1 55%;
}
.header__info > div:nth-child(3) li {
  display: inline-block;
  padding: 0 10px;
}

/* header light */
.light .header__inner {
  background: #f0eeeb;
  border-bottom: 1px solid #dad8d1;
}
.light .header__inner__port a {
  color: #000;
}
.light .header__inner__logo a {
  color: #000;
}
.light .header__nav.demo li a {
  color: #000;
}
.light .header__inner__menu a::before {
  background: #000;
  box-shadow: 0 12px 0 #000;
}
.light .header__inner__menu a::after {
  background: #000;
  box-shadow: 0 12px 0 #000;
}
.light .header__inner__port a::before {
  background: #000;
}
.light .header__inner__port a::after {
  background: #000;
}
</style>
