<template>
  <div>
    <header>
      <img src="../assets/images/cyber-division-logo-full-2.png" class="logo" />
      <img src="../assets/images/hamburger.svg" class="menu" />
    </header>
    <div class="divider"></div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  height: 65px;
  padding: 0 100px;
  @media screen and (max-width: 990px) {
    width: 100%;
    height: 100px;
    margin: 0 auto;
    padding: 60px 0 20px;
    justify-content: center;
  }
  .logo {
    max-width: 143px;
    height: auto;
    padding: 26px 0 21.5px;
    @media screen and (max-width: 990px) {
      display: none;
    }
  }
  .menu {
    max-width: 44px;
    height: auto;
    padding: 30px 0 27.5px;
    @media screen and (max-width: 990px) {
      padding: 0;
    }
  }
}
.divider {
  width: 100%;
  height: 1px;
  flex-shrink: 0;
  background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
  opacity: 0.3;
}
</style>
