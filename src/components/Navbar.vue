<template>
  <nav class="navbar">
    <div class="mx-auto navbar-body" style="width:80%">
      <div class="col-sm">
        <img src="../assets/image/logo.png" alt="">
      </div>
      <div class="col-sm">
        <ul class="">
          <li>關於我們</li>
          <li>聯絡方式</li>
          <li>消費方式</li>
          <li>店內景觀</li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.navbar {
  background-color: #9F353A;
}
.navbar-body {
  display: flex !important;
  justify-content: space-around;
  text-align: left;
  img {
    cursor: pointer;
  }
  ul {
    height: 100%;
    margin: auto;
    display: flex !important;
    justify-content: space-around;

    li {
      font-size: 1.5rem;
      color: #fff;
      list-style: none;
      margin: auto 10px;
      cursor: pointer;
    }
  }
}

</style>
