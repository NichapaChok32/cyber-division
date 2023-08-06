<template>
  <div id="SimpleSolutions">
    <div class="solutions">
      <img src="../assets/images/rectangle-40.png" class="bg-simple" />
      <div class="simple-header">
        Simple Solutions for Complex Connections. <br />
        We are Pushing Limits.
      </div>
      <div class="divider"></div>
      <div
        v-for="sol in solutions"
        :key="sol.name"
        :class="{ 'solution-green': sol.name === 'Voxxt' }"
      >
        <div class="columns-2 simple-row">
          <div class="solution-name" :class="{ green: sol.name === 'Voxxt' }">
            {{ sol.name }}
            <div v-if="sol.name !== 'Voxxt'" class="links">
              <img src="../assets/images/link.svg" />
            </div>
            <div v-else class="links">
              <img src="../assets/images/activeLinks.svg" />
            </div>
          </div>
          <div
            class="solution-description"
            :class="{ green: sol.name === 'Voxxt' }"
          >
            {{ sol.description }}
          </div>
        </div>
        <div v-if="sol.name !== 'Voxxt'" class="solution-divider"></div>
      </div>
    </div>
  </div>
</template>

<script setup>
const solutions = [
  {
    name: "Elita.app",
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quam quam arcu nunc, orci eu bibendum.",
  },
  {
    name: "Voxxt",
    description:
      "The Primal Voxxt are a collection of human designed and computer generated NFT’s, with a maximum supply of 5,000.",
  },
  {
    name: "Hype Dudes",
    description:
      "HYPEDUDES is a utility-driven project featuring a collection of 1444 unique, 3D designed, fashionable NFT dudes ready to take over the Metaverse.",
  },
  {
    name: "CryptoKings",
    description:
      "At CryptoKings we focus on educating everyday people about the world of cryptocurrency. Learn to trade safely and profitably with a large community of aspiring traders and investors",
  },
  {
    name: "Helix",
    description:
      "A helix, plural helixes or helices, is a shape like a corkscrew or spiral staircase. It is a type of smooth space curve with tangent lines at a constant angle to a fixed axis",
  },
];
</script>

<style lang="scss" scoped>
#SimpleSolutions {
  position: relative;
  width: 100%;
  padding: 150px 0 250px;
  @media screen and (max-width: 990px) {
    margin: 0 auto;
    padding: 0 0 100px;
    display: flex;
    justify-content: center;
  }
  @media screen and (max-width: 610px) {
    padding: 0 15px 100px;
  }
  .solutions {
    @media screen and (max-width: 990px) {
      width: 100%;
      display: block;
      max-width: 380px;
    }
    .bg-simple {
      position: absolute;
      left: auto;
      right: 3%;
      top: 25%;
      min-width: 359px;
      z-index: 999;
      @media screen and (max-width: 1845px) {
        right: 2%;
      }
      @media screen and (max-width: 1600px) {
        right: 1.5%;
      }
      @media screen and (max-width: 1300px) {
        right: 3%;
        max-width: 300px;
      }
      @media screen and (max-width: 1170px) {
        right: 2%;
      }
      @media screen and (max-width: 1105px) {
        min-width: 250px;
      }
      @media screen and (max-width: 990px) {
        display: none;
      }
    }
    .simple-header {
      padding: 0 110px 56px 24px;
      color: #ecf9e8;
      font-family: "Aeonik Regular";
      font-size: 68.095px;
      font-style: normal;
      font-weight: 400;
      line-height: 74.905px;
      @media screen and (max-width: 1460px) {
        font-size: 60px;
        line-height: 70px;
      }
      @media screen and (max-width: 1304px) {
        font-size: 54px;
        line-height: 68px;
      }
      @media screen and (max-width: 1189px) {
        font-size: 50px;
        line-height: 60px;
      }
      @media screen and (max-width: 1112px) {
        font-size: 44px;
        line-height: 58px;
      }
      @media screen and (max-width: 990px) {
        font-size: 30px;
        line-height: 40px;
        padding: 0 0 26px;
      }
      @media screen and (max-width: 610px) {
        br {
          display: none;
        }
      }
    }
    .divider {
      height: 1px;
      margin: 0 100px;
      background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
      opacity: 0.3;
      @media screen and (max-width: 990px) {
        margin: 0 auto;
      }
    }
    .solution-green {
      background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
      @media screen and (max-width: 990px) {
        margin: 0 -19rem;
      }
      .simple-row {
        @media screen and (max-width: 990px) {
          padding: 30px 19rem;
        }
      }
    }
    .simple-row {
      padding: 35px 100px;
      @media screen and (max-width: 990px) {
        padding: 30px 0;
        &.columns-2 {
          columns: 1;
        }
      }
      .solution-name {
        max-width: 65%;
        min-height: 45px;
        color: #ecf9e8;
        font-family: "Aeonik Light";
        font-size: 24px;
        font-style: normal;
        line-height: normal;
        letter-spacing: 0.5px;
        vertical-align: middle;
        align-items: center;
        display: flex;
        @media screen and (max-width: 1845px) {
          min-height: 50px;
        }
        @media screen and (max-width: 1760px) {
          min-height: 55px;
        }
        @media screen and (max-width: 1600px) {
          min-height: 60px;
        }
        @media screen and (max-width: 1500px) {
          min-height: 65px;
        }
        @media screen and (max-width: 1410px) {
          min-height: 70px;
        }
        @media screen and (max-width: 1150px) {
          min-height: 75px;
        }
        @media screen and (max-width: 990px) {
          margin-bottom: 23px;
        }
        &.green {
          color: #1e3f04;
          font-family: "Aeonik Regular";
        }
        .links {
          min-height: 30px;
          vertical-align: middle;
          align-items: center;
          display: flex;
          margin-left: 10px;
          img {
            max-height: 13px;
            margin: auto 0;
          }
        }
      }
      .solution-description {
        max-width: 700px;
        margin-left: -37%;
        color: #ecf9e8;
        font-family: "Aeonik Light";
        font-size: 15px;
        font-style: normal;
        line-height: 22.5px;
        letter-spacing: 0.65px;
        @media screen and (max-width: 1845px) {
          max-width: 650px;
        }
        @media screen and (max-width: 1760px) {
          max-width: 600px;
          margin-left: -47%;
        }
        @media screen and (max-width: 1600px) {
          max-width: 550px;
        }
        @media screen and (max-width: 1500px) {
          max-width: 500px;
        }
        @media screen and (max-width: 1410px) {
          max-width: 450px;
        }
        @media screen and (max-width: 1365px) {
          margin-left: -57%;
        }
        @media screen and (max-width: 1150px) {
          max-width: 400px;
        }
        @media screen and (max-width: 990px) {
          margin-left: 0;
          display: block;
        }
        &.green {
          color: #1e3f04;
          font-family: "Aeonik Regular";
        }
      }
    }
    .solution-divider {
      display: block;
      height: 1px;
      margin: 0 100px;
      background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
      opacity: 0.3;
      @media screen and (max-width: 990px) {
        margin: 0 auto;
      }
    }
  }
}
</style>
