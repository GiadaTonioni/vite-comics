<script>
export default {

}
</script>

<template>
  <div>
    <header>
      <div class="container">
        <div class="row">
          <div class="col-header-left">
            <div><img src="../assets/img/dc-logo.png" alt=""></div>
          </div>
          <div class="col-header-right">
            <ul>
              <li>MENU HEADER</li>
            </ul>
          </div>
        </div>

      </div>

      <div class="jumbotron">FASCIA NERA</div>
    </header>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.row {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.container {
  margin: 0 auto;
}

.col-header-left {
  border: 1px solid blue;
  height: 120px;
  width: 20%;
}

.col-header-right {
  border: 1px solid blue;
  height: 120px;
  width: 60%;
}

.jumbotron {
  background-color: black;
  height: 100px;
}
</style>
      
      
