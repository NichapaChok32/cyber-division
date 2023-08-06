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
  @media screen and (max-width: 990px) {
    padding-bottom: 100px;
    margin: 0 auto;
    justify-content: center;
  }
  .empowered-img {
    @media screen and (max-width: 1430px) {
      max-width: 322px;
      object-fit: cover;
    }
    @media screen and (max-width: 1210px) {
      max-width: 222px;
      object-fit: cover;
    }
    @media screen and (max-width: 990px) {
      display: none;
    }
  }
  .empowered-content {
    padding: 75px 95px;
    @media screen and (max-width: 1210px) {
      padding: 75px 65px;
    }
    @media screen and (max-width: 990px) {
      display: block;
      max-width: 380px;
      padding: 0px;
    }
    .empowered-header {
      color: #ecf9e8;
      font-family: "Aeonik Regular";
      font-size: 68.095px;
      font-style: normal;
      line-height: 74.905px;
      @media screen and (max-width: 1855px) {
        font-size: 60px;
        line-height: 70px;
        br {
          display: none;
        }
      }
      @media screen and (max-width: 1710px) {
        font-size: 58px;
        line-height: 64px;
      }
      @media screen and (max-width: 1597px) {
        font-size: 50px;
        line-height: 60px;
      }
      @media screen and (max-width: 1463px) {
        font-size: 48px;
        line-height: 54px;
      }
      @media screen and (max-width: 1430px) {
        font-size: 40px;
        line-height: 50px;
      }
      @media screen and (max-width: 990px) {
        font-size: 30px;
        line-height: 33px;
      }
    }
    .empowered-values {
      margin-top: 63px;
      column-gap: 75px;
      @media screen and (max-width: 1180px) {
        column-gap: 35px;
      }
      @media screen and (max-width: 990px) {
        margin-top: 40px;
        &.columns-3 {
          columns: 1;
        }
      }
      .empowered-lists {
        display: flex;
        border-left: 1px solid;
        border-image-slice: 1;
        border-image-source: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
        @media screen and (max-width: 1610px) {
          min-height: 387px;
          max-height: 400px;
        }
        @media screen and (max-width: 1445px) {
          min-height: 400px;
          max-height: 480px;
        }
        @media screen and (max-width: 1161px) {
          min-height: 440px;
          max-height: 480px;
        }
        @media screen and (max-width: 1081px) {
          min-height: 500px;
          max-height: 580px;
        }
        @media screen and (max-width: 990px) {
          min-height: 148px;
          max-height: 200px;
          margin-bottom: 30px;
        }
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
          @media screen and (max-width: 990px) {
            max-width: 45px;
            max-height: 45px;
            padding: 4px;
            font-size: 32px;
          }
        }
        .empower-desc {
          margin-top: 89px;
          margin-left: -60px;
          padding-left: 27px;
          @media screen and (max-width: 990px) {
            margin-top: 58px;
            padding-left: 38px;
          }
          .header {
            margin-bottom: 19px;
            color: #ecf9e8;
            font-family: "Aeonik Medium";
            font-size: 24px;
            font-style: normal;
            line-height: normal;
            @media screen and (max-width: 1605px) {
              font-size: 20px;
            }
            @media screen and (max-width: 1483px) {
              font-size: 18px;
            }
            @media screen and (max-width: 990px) {
              font-size: 20px;
              margin-bottom: 13px;
            }
          }
          .description {
            color: #f9fff8;
            font-family: "Aeonik Light";
            font-size: 15px;
            font-style: italic;
            line-height: 22.5px;
            letter-spacing: 0.5px;
            @media screen and (max-width: 990px) {
              font-size: 13px;
              line-height: 15.6px;
              letter-spacing: 0.75px;
            }
          }
        }
      }
    }
  }
}
</style>
