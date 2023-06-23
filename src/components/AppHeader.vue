<script>
export default {
  data() {
    return {
      options: [
        {
          label: 'CARACHTERS',
          active: false
        },
        {
          label: 'COMICS',
          active: true
        },
        {
          label: 'MOVIES',
          active: false
        },
        {
          label: 'TV',
          active: false
        },
        {
          label: 'GAMES',
          active: false
        },
        {
          label: 'COLLECTIBLES',
          active: false
        },
        {
          label: 'VIDEOS',
          active: false
        },
        {
          label: 'FANS',
          active: false
        },
        {
          label: 'NEWS',
          active: false
        },
        {
          label: 'SHOP',
          active: false
        },
      ]
    }
  }

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
              <li v-for="(option, index) in options">
                <a :href="option.option">{{ option.label }}</a>
              </li>
            </ul>
          </div>
        </div>

      </div>

      <div class="jumbotron">Conent goes here</div>
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

.jumbotron {
  background-color: black;
  height: 100px;
  color: white;
}

li {
  list-style-type: none;
  display: inline;
  padding: 10px;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 15px;
}
</style>
      
      
