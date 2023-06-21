<template>
  <section id="memberSection" class="member__wrap section center">
    <h3>대표인물 소개</h3>
    <p>창립자 및 지브리스튜디오의 대표인물을 소개합니다.</p>
    <div class="member__inner container">
      <div class="member">
        <figure class="member__header">
          <img src="@/assets/images/member/miyazaki.jpg" alt="멤버1" />
        </figure>
        <div class="member__body">
          <h4>미야자키 하야오</h4>
          <a href="#">대표작품</a>
        </div>
      </div>
      <div class="member">
        <figure class="member__header">
          <img src="@/assets/images/member/toshio_suzuki.png" alt="멤버2" />
        </figure>
        <div class="member__body">
          <h4>토시오 스즈키</h4>
          <a href="#">대표작품</a>
        </div>
      </div>
      <div class="member">
        <figure class="member__header">
          <img src="@/assets/images/member/Isao_Takahata.png" alt="멤버3" />
        </figure>
        <div class="member__body">
          <h4>이사오 타카하타</h4>
          <a href="#">대표작품</a>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss">
.member__wrap {
}
.member__inner {
  @include flex-between;

  .member {
    width: 32%;
    border: 2px solid var(--color_body);

    .member__header {
      img {
        width: 100%;
        height: 520px;
      }
    }
    .member__body {
      width: 100%;
      margin-top: -90px;
      padding: 15px 10px;
      background: #000000ab;
      color: #fff;
      z-index: 100;
      position: relative;
      text-align: center;

      h4 {
        font-size: 22px;
      }

      a {
        color: #fff;
        text-decoration: underline;
        text-underline-position: under;
      }
    }
  }
}
</style>
