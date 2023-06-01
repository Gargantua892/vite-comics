<script>
export default{
  data(){
    return{
      navbar: [
      {
        page: "Characters",
        link: "#",
        state: "off"
      },
      {
        page: "Comics",
        link: "#",
        state: "off"
      },
      {
        page: "Movies",
        link: "#",
        state: "off"
      },
      {
        page: "Tv",
        link: "#",
        state: "off"
      },
      {
        page: "Games",
        link: "#",
        state: "off"
      },
      {
        page: "Collectibles",
        link: "#",
        state: "off"
      },
      {
        page: "Videos",
        link: "#",
        state: "off"
      },
      {
        page: "Fans",
        link: "#",
        state: "off"
      },
      {
        page: "News",
        link: "#",
        state: "off"
      },
      {
        page: "Shop",
        link: "#",
        state: "off"
      },
    ]
    }
  }
}
</script>

<template>
  <div>
      <nav class="navbar navbar-expand-lg bg-body-white p-0">
        <div class="container">
          <a class="navbar-brand" href="#">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
          </a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
            <ul class="navbar-nav">
              <li v-for="item in navbar" class="nav-item  py-4">
                <a class="nav-link active" aria-current="page" href="#">{{item.page}}</a>
              </li>
            </ul>
          </div>
        </div>
    </nav>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;

.nav-item:hover .nav-link {
  color: $primary;
  }

  .navbar-brand{
    img{
      height: 56px;
    }
  }

  .nav-item{
      border-bottom: 4px solid #fff;
      
      &:hover{
        border-bottom: 4px solid $primary;
        cursor: pointer;
      }
    }


</style>