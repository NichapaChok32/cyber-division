<template>
  <div id="Footers">
    <div class="divider"></div>
    <footer class="footers-main columns-3 grid">
      <div class="footers-img">
        <img
          src="../assets/images/cyber-division-logo-full-2.png"
          class="logo"
        />
      </div>
      <div class="footers-col">
        <div class="footers-section">Information</div>
        <ul>
          <li class="footers-li">About Us</li>
          <li class="footers-li">Origins</li>
          <li class="footers-li">FAQs</li>
          <li class="footers-li">Contact</li>
          <li class="footers-li">Legal</li>
        </ul>
      </div>
      <div class="footers-col">
        <div class="footers-section">Contact Us</div>
        <ul>
          <li class="footers-li">contact@cyberdivisino.tn</li>
          <li class="footers-li">+216 29 065 054</li>
          <li class="footers-li">Susah, Imm Ibrahim, 6th Floor</li>
        </ul>
      </div>
      <div class="footers-col">
        <div class="footers-section">Follow us On Social Media</div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
#Footers {
  .divider {
    width: 100%;
    height: 1px;
    flex-shrink: 0;
    background: linear-gradient(90deg, #e3ffe6 0%, #e5e1d6 100%);
    opacity: 0.3;
  }
  .footers-main {
    display: flex;
    max-width: 2024px;
    margin: 0 auto;
    padding: 54px 0 100px;
    justify-content: space-around;
    .logo {
      width: 159px;
      height: auto;
      object-fit: cover;
    }
    .footers-col {
      display: block;
      .footers-section {
        color: #ecf9e8;
        font-family: "Aeonik Medium";
        font-size: 15px;
        font-style: normal;
        line-height: 22.5px;
        letter-spacing: 0.45px;
      }
      .footers-li {
        margin-top: 13px;
        color: #ecf9e8;
        font-family: "Aeonik Regular";
        font-size: 13px;
        font-style: normal;
        font-weight: 400;
        line-height: 19.5px;
        letter-spacing: 0.39px;
      }
    }
  }
}
</style>
