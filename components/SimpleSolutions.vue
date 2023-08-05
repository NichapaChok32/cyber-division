<template>
  <div id="SimpleSolutions">
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
  padding: 150px 0 250px;
  .bg-simple {
    position: absolute;
    left: auto;
    right: 3%;
    top: 25%;
    z-index: 999;
  }
  .simple-header {
    padding: 0 110px 56px 24px;
    color: #ecf9e8;
    font-family: "Aeonik Regular";
    font-size: 68.095px;
    font-style: normal;
    font-weight: 400;
    line-height: 74.905px;
  }
  .divider {
    height: 1px;
    margin: 0 100px;
    background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
    opacity: 0.3;
  }
  .solution-green {
    background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
  }
  .simple-row {
    padding: 35px 100px;
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
  }
}
</style>
