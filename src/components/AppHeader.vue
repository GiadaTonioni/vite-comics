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
              <li v-for="(option, index) in options" :key="index">
                <a :href="option.option">{{ option.label }}</a>
              </li>
            </ul>
          </div>
        </div>

      </div>

      <div class="jumbotron">
        .
      </div>
      <section>
        <div class="container-comics">
          <div class="row-comics">

            <div class="col">
              <div class="card" v-for="(comic, index) in comics" :key="index">
                <img :src="comic.thumb">
                <h5>{{ comic.series }}</h5>
                <p>{{ comic.type }}</p>
                <p>{{ comic.price }}</p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </header>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as*;

.container-comics {
  height: 500px;
  background-color: black;
  position: relative;
}

.card {
  position: absolute;
}

img {
  width: 50%;
}

.row {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
}

.container {
  margin: 0 auto;
}

.jumbotron {
  background-image: url(../assets/img/jumbotron.jpg);
  height: 260px;
}

li {
  list-style-type: none;
  display: inline;
  padding: 10px;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 14px;

  &:hover {
    border-bottom: 4px solid rgb(0, 132, 255);
    cursor: pointer;
  }
}
</style>
      
      
