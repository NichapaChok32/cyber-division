<template>
  <div id="MainBanner">
    <div class="main-banner-row">
      <div class="main-header main-banner-col">
        Closen the technology of the future to help you
        <span class="scroller">
          <div class="scrolling-words-box">
            <ul>
              <li class="main-span" style="color: #c8f4a6">Innovate</li>
              <li class="main-span" style="color: #e9dabd">Connect</li>
              <li class="main-span" style="color: #f3ffa6">Inspire</li>
              <li class="main-span" style="color: #c8f4a6">Innovate</li>
            </ul>
          </div>
        </span>
        <img src="../assets/images/main.svg" class="banner banner-mobile" />
        <p class="main-paragraph">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quam quam
          arcu nunc, orci eu bibendum. Sed morbi pellentesque elit purus quam a
          sollicitudin convallis purus. Sed sed quam risus laoreet viverra id ut
          amet feugiat. Sed nec id id sed ut nulla aliquet neque. Sed est
          malesuada lobortis aliquam dolor eget donec
        </p>
        <div class="get-start">
          <div class="btnStart">Get Started</div>
        </div>
        <div class="our-client">Some of our clients</div>
        <div class="our-client-row">
          <div class="our-client-col">
            <img src="../assets/images/Apple.svg" class="our-client-img" />
          </div>
          <div class="our-client-col">
            <img src="../assets/images/Google.svg" class="our-client-img" />
          </div>
          <div class="our-client-col">
            <img src="../assets/images/Microsoft.svg" class="our-client-img" />
          </div>
        </div>
        <div class="last-divider"></div>
      </div>
      <img
        src="../assets/images/main.svg"
        class="main-banner-col banner banner-desktop"
      />
    </div>
    <div class="green-light">
      <img src="../assets/images/big-green-light.svg" class="big-green" />
      <img src="../assets/images/small-green-light.svg" class="small-green" />
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
$item-count: 4;

@keyframes scrollUp {
  @for $i from 1 through ($item-count - 1) {
    #{($i * 33.33) - 10%},
    #{$i * 33.33%} {
      transform: translateY(calc(-100% / $item-count) * $i);
    }
  }
}
@keyframes run {
  0% {
    right: 0;
    bottom: 0;
  }
  25% {
    right: 40%;
    bottom: 20%;
  }
  50% {
    bottom: 40%;
    right: 60%;
  }
  75% {
    right: 60%;
    bottom: 20%;
  }
  100% {
    right: 60%;
    bottom: 0;
  }
}
@keyframes run2 {
  0% {
    top: 0;
    left: 10%;
  }
  25% {
    top: 20%;
    left: 40%;
  }
  50% {
    top: 40%;
    left: 60%;
  }
  75% {
    top: 20%;
    left: 60%;
  }
  100% {
    top: 0;
    left: 60%;
  }
}
#MainBanner {
  position: relative;
  width: 100%;
  padding: 91.5px 100px 48.5px;
  @media screen and (max-width: 990px) {
    margin: 0 auto;
    padding: 30px 0 100px;
    display: flex;
    justify-content: center;
  }
  .green-light {
    display: flex;
    opacity: 0.5;
    @media screen and (max-width: 500px) {
      display: none;
    }
    .big-green {
      min-width: 347px;
      position: absolute;
      right: 0;
      bottom: 0;
      animation: run 10s linear infinite;
      fill: #e5e1d6;
      filter: blur(25px);
    }
    .small-green {
      min-width: 247px;
      position: absolute;
      top: 0;
      left: 10%;
      animation: run2 10s linear infinite;
      fill: #e5e1d6;
      filter: blur(25px);
    }
  }
  .main-banner-row {
    display: flex;
    justify-content: space-between;
    @media screen and (max-width: 990px) {
      display: block;
      margin: 0 auto;
    }
    .main-banner-col {
      width: fit-content;
      &.main-header {
        max-width: 873.205px;
        padding-top: 68.5px;
        color: #ecf9e8;
        font-family: "Aeonik Regular";
        font-size: 64px;
        font-style: normal;
        line-height: 83.2px;
        z-index: 2;
        @media screen and (max-width: 1544px) {
          font-size: 54px;
          line-height: 73px;
        }
        @media screen and (max-width: 1315px) {
          font-size: 44px;
          line-height: 63px;
        }
        @media screen and (max-width: 1185px) {
          font-size: 40px;
          line-height: 60px;
        }
        @media screen and (max-width: 1134px) {
          max-width: 480px;
        }
        @media screen and (max-width: 1040px) {
          max-width: 420px;
        }
        @media screen and (max-width: 990px) {
          max-width: 380px;
          padding: 0;
        }
        .scroller {
          position: relative;
          display: inline-flex;
          .scrolling-words-box {
            position: relative;
            width: fit-content;
            height: 6rem;
            margin: 0;
            padding-bottom: 20px;
            overflow: hidden;
            ul {
              margin: auto 0;
              padding: 0;
              animation: scrollUp 3.5s ease-in-out infinite normal;
              animation-delay: 2s;
              li.main-span {
                display: flex;
                align-items: center;
                justify-content: flex-start;
                height: 5rem;
                list-style: none;
                font-family: "Aeonik Regular";
                font-size: 64px;
                font-style: normal;
                line-height: normal;
                @media screen and (max-width: 1544px) {
                  font-size: 54px;
                }
                @media screen and (max-width: 1315px) {
                  font-size: 44px;
                }
                @media screen and (max-width: 1185px) {
                  font-size: 40px;
                }
              }
            }
          }
        }
        .banner-mobile {
          display: none;
          @media screen and (max-width: 990px) {
            display: block;
            margin-bottom: 38px;
          }
        }
        .main-paragraph {
          max-width: 687px;
          margin-top: 114px;
          color: #ecf9e8;
          font-family: "Aeonik Light";
          font-size: 16px;
          font-style: normal;
          line-height: 24px;
          letter-spacing: 0.25px;
          @media screen and (max-width: 1134px) {
            max-width: 480px;
          }
          @media screen and (max-width: 1040px) {
            max-width: 420px;
          }
          @media screen and (max-width: 990px) {
            max-width: 380px;
            margin-top: 0;
          }
          @media screen and (max-width: 500px) {
            display: none;
          }
        }
        .get-start {
          width: 152px;
          height: 52px;
          margin-top: 30px;
          border-radius: 6px;
          border: 5px solid rgba(227, 255, 230, 0.21);
          overflow: hidden;
          .btnStart {
            width: 142px;
            height: 42px;
            border-radius: 5px;
            background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
            color: #1e3f04;
            font-family: "Aeonik Medium";
            font-size: 16px;
            font-style: normal;
            line-height: 18px;
            letter-spacing: 0.48px;
            text-align: center;
            padding: 12px 0;
          }
          @media screen and (max-width: 500px) {
            display: none;
          }
        }
        .our-client {
          margin-top: 156px;
          color: #636d5b;
          font-family: "Aeonik Medium";
          font-size: 15px;
          font-style: normal;
          line-height: 22.5px;
          text-decoration-line: underline;
          @media screen and (max-width: 990px) {
            margin-top: 38px;
          }
        }
        .our-client-row {
          display: flex;
          flex-flow: row nowrap;
          column-gap: 24px;
          align-items: center;
        }
        .last-divider {
          max-width: 991px;
          height: 1px;
          margin-top: 48.5px;
          background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
          opacity: 0.3;
          @media screen and (max-width: 500px) {
            margin-top: 10px;
          }
        }
      }
      &.banner {
        max-width: 557px;
        max-height: 719.234px;
        @media screen and (max-width: 1600px) {
          max-width: 500px;
          max-height: 700px;
        }
        @media screen and (max-width: 1544px) {
          max-width: 450px;
          max-height: 690px;
        }
        @media screen and (max-width: 1494px) {
          max-width: 400px;
          max-height: 610px;
        }
        @media screen and (max-width: 1134px) {
          max-width: 350px;
          max-height: 590px;
        }
        &.banner-desktop {
          display: block;
          @media screen and (max-width: 990px) {
            display: none;
          }
        }
        &.banner-mobile {
          display: none;
        }
      }
    }
  }
}
</style>
<style scoped>
.scroller::after {
  left: 0;
  bottom: 0;
  z-index: 1;
  width: 100%;
  content: "";
  height: 20px;
  position: absolute;
  background: url("../assets/images/underline.svg") no-repeat bottom;
}
@media screen and (max-width: 1544px) {
  .scroller::after {
    bottom: 10px;
  }
}
@media screen and (max-width: 1315px) {
  .scroller::after {
    bottom: 15px;
  }
}
.scroller > .scrolling-words-box::before {
  top: 0;
  left: 0;
  z-index: 1;
  width: 100%;
  content: "";
  height: 10px;
  position: absolute;
}
.scroller > .scrolling-words-box::after {
  left: 0;
  bottom: 0;
  z-index: 1;
  width: 100%;
  content: "";
  height: 30px;
  position: absolute;
}
</style>
