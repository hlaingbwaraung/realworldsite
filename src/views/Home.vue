<template>
  <div>
    <section id="banner">
      <div class="container mt-3">
        <div class="row">
          <div class="col-md-6 p-5">
            <h2><span class="spancss">APOLLO</span>とは？</h2>
            <p>
              &nbsp;&nbsp;&nbsp;&nbsp;世の中にいる戦争や貧困などの様々な理由で独学に大変な方と子供達を向けて完全<span
                >無料</span
              >
              でメンタリング付きのオンラインスクールです。やる気だけあればゼローから就職までサポート致します。より良い世界へ！
            </p>
            <router-link :to="{ name: 'Chat' }"
              ><button class="button">Create Acoount</button></router-link
            >
          </div>
          <div class="col-md-6 order-first order-md-last text-center">
            <img src="../photo/banimg.png" class="img-fluid" />
          </div>
        </div>
      </div>

      <img src="../photo/wave1.png" class="bottom-img" />
    </section>

    <section id="services">
      <div class="container text-center animate__animated animate__fadeInUp">
        <h1 class="title">サービス</h1>
        <div class="row text-center p-5">
          <div class="col-md-4 services d-1">
            <img src="../photo/service1.png" class="service-img" />
            <h4>日本語コース</h4>
            <div id="box"></div>
            <p>
              漢字、聴解、ビジネス会話、IT用語など様々な知識を日本にいる方、また日本人がメンタリングいたします。
            </p>
          </div>
          <div class="col-md-4 services d-2">
            <img src="../photo/service2.png" class="service-img" />
            <h4>プログラミングコース</h4>
            <p>
              WEB業界のフロントエンドやバックエンドを現場のエンジニアから
              メンタリングいたします。
            </p>
          </div>
          <div class="col-md-4 services d-3">
            <img src="../photo/service3.png" class="service-img" />
            <h4>キャリアサポート</h4>
            <p>
              日本語とITスキルが身につけた後は日本のIT企業に入社するまで精一杯でサポート致します。
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="about-us">
      <div class="container">
        <h1 class="title text-center">学習方法</h1>
        <div class="row align-items-center tex-center p-2">
          <div class="col-md-6 mt-2 font-weight-bold d-1">
            <ul>
              <li>
                <i class="bi bi-book-fill"></i
                >&nbsp;&nbsp;&nbsp;&nbsp;最強のキャリクラム
              </li>
              <li>
                <i class="bi bi-person-video3"></i
                >&nbsp;&nbsp;&nbsp;&nbsp;マンツーマンメンタリング
              </li>
              <li>
                <i class="bi bi-chat-dots"></i
                >&nbsp;&nbsp;&nbsp;&nbsp;質問チャットサポート
              </li>
              <li>
                <i class="bi bi-chat-left-heart-fill"></i
                >&nbsp;&nbsp;&nbsp;&nbsp;生活悩み相談ルーム
              </li>
            </ul>
          </div>
          <div class="col-md-6 order-first order-md-last d-2">
            <img src="../photo/gakushu.png" class="img-fluid mt-2" />
          </div>
        </div>
      </div>
    </section>
    <RelatedBlogs></RelatedBlogs>
    <Patner></Patner>
    
  </div>
</template>

<script>
import RelatedBlogs from "../components/RelatedBlogs";
import Patner from "../components/Patner";
export default {
  components: {
    RelatedBlogs,
    Patner,
  },
};
</script>

<style>
#banner {
  padding-top: 20px;
  background: #c8d8e4;
}
h2 {
  font-size: 30px;
  font-weight: 600;
}
h1 {
  font-size: 40px;
  font-weight: 600;
}
#banner .btn-primary {
  box-shadow: none;
  padding: 8px 25px;
  border: none;
  border-radius: 10px;
  background-color: tomato;
}
.service-img {
  width: 200px;
}
.services h4 {
  padding: 5px;
  margin-top: 20px;
  text-transform: uppercase;
  font-weight: 600;
}
#about-us {
  background: #f8f9fa;
  padding: 30px 0;
}

.about-title {
  font-size: 40px;
  font-weight: 600;
  margin-top: 8%;
}

#about-us ul {
  margin-left: 20px;
  font-size: 20px;
  list-style: none;
}

#about-us ul li {
  margin: 10px 0;
}
.bottom-img {
  width: 100%;
}
</style>
