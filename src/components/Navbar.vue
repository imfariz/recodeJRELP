<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light-red">
    <div class="container">
        <a class="navbar-brand fs-1" href="#">
            <img :src="logoJre" alt="JRE Media Testing logo">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
            data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent"
            aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse pt-2 ms-2" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto">
                <li class="nav-item">
                    <a class="nav-link" href="#" :class="{ active: current === 'Beranda' }"
                    @click="current = 'Beranda'">
                        Beranda
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" :class="{ active: current === 'Layanan' }"
                    @click="current = 'Layanan'">
                        Layanan
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" :class="{ active: current === 'Portofolio' }"
                    @click="current = 'Portofolio'">
                        Portofolio
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" :class="{ active: current === 'Blog' }"
                    @click="current = 'Blog'">
                        Blog
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#" :class="{ active: current === 'Kontak' }"
                    @click="current = 'Kontak'">
                        Kontak
                    </a>
                </li>
            </ul>
            <!-- <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Search"
                aria-label="Search">
                <button class="btn btn-outline-success" type="submit">Search</button>
            </form> -->
        </div>
    </div>
</nav>
</template>

<script>
import logoJre from '@/assets/jre.svg';

export default {
  name: 'Navbar',
  props: {
    title: String,
  },
  data() {
    return {
      logoJre,
      current: 'Beranda',
    };
  },
  methods: {
    addClass() {
      this.isActive = true;
    },
  },
};
</script>

<style scoped>
.nav-item {
    font-weight: 500;
    margin-left: 1.5rem;
}

.active {
    font-weight: 700;
}

.bg-light-red {
    background-color: #FFF9F9;
}
</style>
