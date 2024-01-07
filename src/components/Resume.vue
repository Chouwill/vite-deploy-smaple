<template>
  <div class="wrap">
      <header>
        <p>CHARLIE CASH | BLOGGER</p>
        <a href="#">HOME</a>
        <a href="#" class="phone_menu"><i class="fa-solid fa-bars"></i></a>
      </header>

      <main>
        <div class="profile">
          <img src="https://picsum.photos/414/544/?random=10">
          <h2>
            Hi, My Name is<br />
            Charlie Cash.
          </h2>
          <!-- <p>
            SF based. NY raised.<br />
            British born. Speak fluent social.
          </p> -->
        </div>
        <div class="introduction">
          <ul class="education">
            <h2>EDUCATION</h2>
            <li><h3>台北市立龍門國中</h3></li>
            <li><h3>台北市立大理高中</h3></li>
            <li><h3>高雄義守大學</h3></li>
            <li><h3>休閒事業管理學系</h3></li>
          </ul>

          <ul class="link">
            <li><a href="#">履歷</a></li>
            <li><a href="#">作品一</a></li>
            <li><a href="#">作品二</a></li>
            <!-- <li><a href="#">WORK WITH ME</a></li> -->
          </ul>

          <div class="community">
            <!-- <a href="#"><i class="fa-brands fa-twitter"></i></a>
            <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
            <a href="#"><i class="fa-brands fa-instagram"></i></a>
            <a href="#"><i class="fa-brands fa-youtube"></i></a>
            <a href="#"><i class="fa-brands fa-tiktok"></i></a> -->
          </div>

          <div class="copyright">
            Copyright &copy; 2035 by Charlie Cash. Powered and secured
          </div>
        </div>
      </main>
    </div>
</template>

<script setup></script>

<style scoped>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    list-style: none;
    text-decoration: none;
    font-family: "微軟正黑體", sans-serif;
  }
  .wrap {
    max-width: 100%;
    height: 100vh;
  }
  header {
    width: 100%;
    padding: 20px;
    display: flex;
    align-items: center;
    background: palegoldenrod;

    height: 58px;
  }
  header p {
    flex: 1;
    margin-left: 50px;
  }
  header a {
    flex-basis: 20%;
    /* background-color: aqua; */
    text-align: right;
    margin-right: 50px;
    text-decoration: none;
    color: #000;
  }
  .phone_menu {
    display: none;
  }
  @media screen and (max-width: 768px) {
    .wrap {
      height: auto;
    }
    header {
      width: 100%;
      z-index: 1000;
    }
    header a {
      display: none;
    }
    .phone_menu {
      display: block;
    }
  }
  /* --------------------------------------------------主內容 */
  main {
    display: flex;
    height: calc(100% - 58px);
  }
  @media screen and (max-width: 768px) {
    main {
      flex-direction: column;
      height: auto;
      position: relative;
    }
  }
  /* --------------------------------------------------  左區域 */
  .profile {
    display: flex;
    align-items: center;
    flex: 1;
    flex-direction: column;

    background: linear-gradient(135deg, #ff9a9e, #86e3ce);
  }
  .profile img {
    display: block;
    border-radius: 20%;
    max-width: 100%;
    height: auto;
    margin: 0 auto;
    padding: 50px 0;
  }
  .profile h2 {
    font-size: 40px;
  }
  .profile p {
    font-size: 20px;
    margin: 20px 0;
  }
  @media screen and (max-width: 768px) {
    .profile {
      width: 100%;
      position: relative;
      order: 1;
      height: auto;
    }
    .profile img {
      width: 40%;
      height: auto;
      margin: 0 auto;
      position: relative;
      bottom: -3rem;
    }
  }
  /* ---------------------------------------左end ------------*/
  /*-----------------------------------------------------右education*/
  .introduction {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 1;
    background-color: rgb(199, 165, 102);
    min-height: 500px;
  }
  .link{
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 100%;  /*詢問是否要寫寬度，或要寫死寬度，可否用100%，用父層introduction*/
    /* border: 5px solid yellow; */
  }
  .link li {
    border: 2px solid #000;
    background-color: aliceblue;
    padding: 5px 40px;
    text-align: center;
    margin: 15px;
  }
  .education {
    width: 500px;
    /* border: 1px solid red; */
  }
  .education h2 {
    font-size: 40px;
    text-align: center;
  }
  .education li {
    padding: 0 133px;
  }
  .education li h3 {
    border-left: 3px solid #ff7168;
    padding: 5px 15px;
    text-align: left;
  }
  .community {
    margin-top: 10px;
  }
  .community a {
    margin-right: 15px;
    color: #000;
    font-size: 20px;
  }
  .copyright {
    margin-top: 100px;
  }

  @media screen and (max-width: 768px) {
    .introduction {
      width: 100%;
      padding-top: 100px;
      order: 2;
    }
    .introduction h2 {
      font-size: 30px;
    }
    .introduction p {
      font-size: 15px;
    }
    .introduction_link li {
      padding: 10px;
    }

    .copyright {
      margin-top: 100px;
      padding: 2rem;
      text-align: center;
    }
  }
</style>
