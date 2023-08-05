<template>
  <div id="Empowered">
    <img src="../assets/images/women.png" class="empowered-img" />
    <div class="empowered-content">
      <div class="empowered-header">
        Empowered by Innovation, Commited by <br />
        Intellect and Driven by Values
      </div>
      <div class="columns-3 empowered-values">
        <div v-for="emp in empowered" :key="emp.name" class="empowered-lists">
          <div class="empower-day">{{ emp.day }}</div>
          <div class="empower-desc">
            <div class="header">{{ emp.name }}</div>
            <div class="description">{{ emp.description }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const empowered = [
  {
    day: "07",
    name: "Projects",
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quam quam arcu nunc, orci eu bibendum. Sed morbi pellentesque elit purus quam a sollicitudin convallis purus. Sed sed quam risus laoreet viverra id ut amet feugiat. Sed nec id id sed ut nulla aliquet neque. Sed est malesuada lobortis aliquam dolor eget donec ",
  },
  {
    day: "23",
    name: "Clients",
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quam quam arcu nunc, orci eu bibendum. Sed morbi pellentesque elit purus quam a sollicitudin convallis purus. Sed sed quam risus laoreet viverra id ut amet feugiat. Sed nec id id sed ut nulla aliquet neque. Sed est malesuada lobortis aliquam dolor eget donec ",
  },
  {
    day: "04",
    name: "Tech & Creative teams",
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quam quam arcu nunc, orci eu bibendum. Sed morbi pellentesque elit purus quam a sollicitudin convallis purus. Sed sed quam risus laoreet viverra id ut amet feugiat. Sed nec id id sed ut nulla aliquet neque. Sed est malesuada lobortis aliquam dolor eget donec ",
  },
];
</script>

<style lang="scss" scoped>
#Empowered {
  padding-bottom: 250px;
  display: flex;
  .empowered-content {
    padding: 75px 95px;
    .empowered-header {
      color: #ecf9e8;
      font-family: "Aeonik Regular";
      font-size: 68.095px;
      font-style: normal;
      line-height: 74.905px;
    }
    .empowered-values {
      margin-top: 63px;
      column-gap: 75px;
      .empowered-lists {
        display: flex;
        border-left: 1px solid #e5e1d6;
        border-color: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
        .empower-day {
          max-width: 60px;
          max-height: 60px;
          padding: 5px 7px 7px;
          background: linear-gradient(135deg, #e3ffe6 0%, #e5e1d6 100%);
          color: #1e3f04;
          font-family: "Aeonik Regular";
          font-size: 40px;
          font-style: normal;
          line-height: normal;
        }
        .empower-desc {
          margin-top: 89px;
          margin-left: -60px;
          padding-left: 27px;
          .header {
            margin-bottom: 19px;
            color: #ecf9e8;
            font-family: "Aeonik Medium";
            font-size: 24px;
            font-style: normal;
            line-height: normal;
          }
          .description {
            color: #f9fff8;
            font-family: "Aeonik Light";
            font-size: 15px;
            font-style: italic;
            line-height: 22.5px;
            letter-spacing: 0.5px;
          }
        }
      }
    }
  }
}
</style>
