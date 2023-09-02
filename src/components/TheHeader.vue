<!-- IMPORTA VARIABILI SASS
NON VA PIU DROP SHADOW
COLORE SFONDO SEARCH BAR NON CAMBIA -->

<script>
export default {
  data() {
    return {
      links: [
        { name: "Link 1" },
        { name: "Link 2" },
        { name: "Link 3" },
        { name: "Link 4" },
        { name: "Link 5" },
        { name: "Link 6" },
      ],
    };
  },
};
</script>

<template>
  <header class="header">
    <div class="container">
      <div class="row align-items-center">
        <div class="col">
          <div class="logo">
            <img src="../assets/img/dark-logo.png" alt="Logo" />
          </div>
        </div>
        <div class="col">
          <!-- NAV START -->
          <nav class="navbar navbar-expand-lg">
            <ul class="navbar-nav justify-content-center">
              <!-- con v-for genero link da array oggetti (differenti nomi ai link) -->
              <li
                v-for="(link, index) in links"
                :key="index"
                class="nav-item dropdown"
              >
                <a
                  class="nav-link dropdown-toggle"
                  href="#"
                  :id="'navbarDropdown' + index"
                  role="button"
                  data-toggle="dropdown"
                  aria-haspopup="true"
                  aria-expanded="false"
                >
                  {{ link.name }}
                </a>
                <div
                  :id="'dropdown-menu-' + index"
                  class="dropdown-menu"
                  :aria-labelledby="'navbarDropdown' + index"
                >
                  <a class="dropdown-item" href="#">Action</a>
                  <a class="dropdown-item" href="#">Another action</a>
                  <div class="dropdown-divider"></div>
                  <a class="dropdown-item" href="#">Something else here</a>
                </div>
              </li>
            </ul>
          </nav>
          <!-- NAV END -->
        </div>
        <div class="col">
          <!-- ____________________________________ -->
          <div class="search-bar">
            <!--bg-myclass non cambia colore allo sfondo della search bar -->
            <input type="text" placeholder="Search..." />
            <i class="fas fa-search"></i>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  background-color: #ffffff;
  color: #fff;
  padding: 10px 0;
  // non vedo più box shadow
  box-shadow: 2px 2px 10px rgb(10, 0, 0);
  z-index: 10;
}

.logo img {
  max-width: 100px;
}

ul {
  list-style: none;
  padding: 0;
  display: flex;
  margin: 0;
}

li {
  margin-right: 20px;
  a {
    color: black;
    &:hover {
      color: black;
    }
  }
}

.header .search-bar {
  display: flex;
  align-items: center;

  input {
    flex: 1;
    padding: 5px;
    border: none;
    border-radius: 4px;
  }

  .fa-search {
    font-size: 20px;
    margin-left: 10px;
  }

  i {
    color: rgb(32, 173, 150);
  }
}
</style>
