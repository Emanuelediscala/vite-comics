<script>
//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
  name: "AppHeader",
  data() {
    return {
      links: ["characters", "comics", "movies", "tv", "games", "collectibles", "videos", "fans", "news", "shop"]
    }
  },
  methods: {

  }
};
</script>

<template>
  <div class="container">
    <div class="d-flex justify-content-between p-2 align-items-center">
      <div>
        <img src="/public/dc-logo.png" alt="">
      </div>
      <div>
        <ul class="nav justify-content-end">
          <div class="h-100">
            <li class="nav-item d-flex">
              <a class="nav-link active" v-for="link in links" aria-current="page" href="#">{{ link.toUpperCase() }}</a>
            </li>
          </div>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
a:hover {
  color: blue;
  border-bottom: 4px solid blue;
  transition: border-color 0.3s;
}

a {
  color: black;



}
</style>