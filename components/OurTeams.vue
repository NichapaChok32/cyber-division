<template>
  <div id="OurTeam">
    <div class="team-header">
      Our teams are continuously developing innovative strategies, building new
      technologies, and conducting ongoing research.
    </div>
    <div class="team-function">
      <div
        v-for="t in teams"
        :key="t.name"
        class="team-image"
        :class="{ computer: t.name === 'Development' }"
      >
        <img
          :src="imageSrc(t.team_img)"
          class="function-img"
          :class="{ computer: t.name === 'Development' }"
        />
        <div
          class="function-name"
          :class="{ computer: t.name === 'Development' }"
        >
          {{ t.name }}
        </div>
      </div>
    </div>
    <div class="team-header-2">
      You’ve got questions, we’ve got answers... Let’s Chat!
    </div>
    <div class="btnTeam">Contact the Team</div>
  </div>
</template>

<script setup>
const teams = [
  {
    name: "Administration",
    team_img: "administration.png",
  },
  {
    name: "Design",
    team_img: "design.png",
  },
  {
    name: "Development",
    team_img: "development.jpg",
  },
  {
    name: "AI",
    team_img: "ai.png",
  },
];

const imageSrc = (path) => {
  return new URL(`../assets/images/${path}`, import.meta.url).href;
};
</script>

<style lang="scss" scoped>
#OurTeam {
  padding-bottom: 250px;
  .team-header {
    margin-bottom: 40px;
    padding-left: 24px;
    color: #ecf9e8;
    font-family: "Aeonik Regular";
    font-size: 68.095px;
    font-style: normal;
    font-weight: 400;
    line-height: 74.905px;
  }
  .team-function {
    display: flex;
    width: 100%;
    padding-bottom: 250px;
    margin: 0 auto;
    column-gap: 5px;
    .team-image {
      position: relative;
      max-width: 20%;
      max-height: 624px;
      &.computer {
        max-width: 40%;
      }
      .function-name {
        position: absolute;
        bottom: 21px;
        left: 19px;
        color: #ecf9e8;
        font-family: "Aeonik Bold";
        font-size: 24px;
        font-style: normal;
        line-height: 36px;
        &.computer {
          left: 22px;
        }
      }
      .function-img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        &.computer {
          transform: scaleX(-1);
        }
      }
    }
  }
  .team-header-2 {
    margin: 0 auto 62px;
    text-align: center;
    color: #ecf9e8;
    font-family: "Aeonik Regular";
    font-size: 68.095px;
    font-style: normal;
    font-weight: 400;
    line-height: 74.905px;
  }
  .btnTeam {
    width: 180px;
    height: 50px;
    margin: 0 auto;
    padding: 12px 0;
    border-radius: 5px;
    background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
    color: #1e3f04;
    font-family: "Aeonik Medium";
    font-size: 16px;
    font-style: normal;
    line-height: 24px;
    letter-spacing: 0.48px;
    text-align: center;
  }
}
</style>
