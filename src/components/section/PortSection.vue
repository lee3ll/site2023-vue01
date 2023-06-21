<template>
  <section id="portSection" :class="attr">
    <h3>포트폴리오 소개</h3>
    <p>웹디자이너, 웹 퍼블리셔, 프론트앤드 개발자 포트폴리오 입니다.</p>
    <div class="port__inner container">
      <div class="port__btn">
        <ul>
          <li><a href="#">21기</a></li>
          <li><a href="#">22기</a></li>
          <li><a href="#">23기</a></li>
          <li><a href="#">24기</a></li>
        </ul>
      </div>
      <div class="port__cont">
        <div class="port" v-for="(text, index) in texts" :key="index">
          <figure class="port__header">
            <img :src="text.img" alt="text.title" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img :src="text.icon" alt="text.title" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
        <div class="port">
          <figure class="port__header">
            <img src="@/assets/images/portfolio/portfolio02.jpg" alt="포폴1" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img src="@/assets/images/member/member02.svg" alt="멤버1" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
        <div class="port">
          <figure class="port__header">
            <img src="@/assets/images/portfolio/portfolio03.jpg" alt="포폴1" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img src="@/assets/images/member/member05.svg" alt="멤버1" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
        <div class="port">
          <figure class="port__header">
            <img src="@/assets/images/portfolio/portfolio04.jpg" alt="포폴1" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img src="@/assets/images/member/member09.svg" alt="멤버1" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
        <div class="port">
          <figure class="port__header">
            <img src="@/assets/images/portfolio/portfolio05.jpg" alt="포폴1" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img src="@/assets/images/member/member11.svg" alt="멤버1" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
        <div class="port">
          <figure class="port__header">
            <img src="@/assets/images/portfolio/portfolio06.jpg" alt="포폴1" />
          </figure>
          <div class="port__body">
            <div class="pic">
              <img src="@/assets/images/member/member13.svg" alt="멤버1" />
            </div>
            <div>
              <h4>김현정 포트폴리오</h4>
              <span>프론트앤드 개발자 포트폴리오</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    attr: String,
  },
  data: function () {
    return {
      texts: [
        {
          img: "./assets/images/portfolio/portfolio01.jpg",
          title: "김현정 포트폴리오 ",
          desc: "프론트앤드 개발자 포트폴리오",
          icon: "./assets/images/member/member01.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.port__wrap {
}
.port__inner {
  .port__btn {
    ul {
      display: flex;
      justify-content: center;
      margin-bottom: 40px;
      li {
        margin-right: 20px;
        a {
          padding: 10px 40px;
          border-radius: 50px;
          border: 1px solid #ff8585;
          font-weight: 300;
          background-color: #fd6c6c;
          font-size: 18px;
          color: #fff;
        }
      }
    }
  }
  .port__cont {
    @include flex-between;
    flex-wrap: wrap;

    .port {
      width: 32.2222%;
      margin-bottom: 30px;
      .port__header {
      }
      .port__body {
        display: flex;
        align-items: center;
        margin-top: 10px;

        .pic {
          margin-right: 10px;
          border-radius: 50px;

          img {
            width: 50px;
            height: 50px;
          }
        }

        .title {
          h4 {
            font-size: 20px;
            color: var(--color_body);
          }
          span {
            font-size: 16px;
            color: #2c3a4b;
          }
        }
      }
      img {
        border-radius: 10px;
        width: 100%;
      }
      &:nth-child(1) .port__body .pic {
        background-color: #ffb6b6;
      }
      &:nth-child(2) .port__body .pic {
        background-color: #ffe4ab;
      }
      &:nth-child(3) .port__body .pic {
        background-color: #d7f8ac;
      }
      &:nth-child(4) .port__body .pic {
        background-color: #acf3f8;
      }
      &:nth-child(5) .port__body .pic {
        background-color: #acbaf8;
      }
      &:nth-child(6) .port__body .pic {
        background-color: #daacf8;
      }
    }
  }
}
</style>
