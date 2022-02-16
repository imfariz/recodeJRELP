<template>
    <section class="container hero d-flex flex-column flex-md-row justify-content-between
    align-items-center">
        <div class="description text-md-start text-center">
            <h1 class="fs-1 lh-base fw-bold">Jelajahi setiap <br>
            ruangan yang kami <br>
            sediakan untuk Anda
            </h1>
            <p class="mt-4 fs-6 lh-base">
                Bagaimana Cara Anda Melakukan Promosi <br>
                Menentukan Nasib Bisnis Anda
            </p>
        </div>
        <img :src="heroSvg" alt="Hero Image" class="px-5 px-md-0">
    </section>
</template>
<script>
import heroSvg from '@/assets/hero.svg';

export default {
  name: 'Hero',
  data() {
    return {
      heroSvg,
    };
  },
};
</script>
<style scoped>
.description p {
    color: #949494;
}

.hero {
  height: 80vh;
  margin-bottom: 130px;
  margin-top: 50px;
}

img {
    width: 500px;
    height: 450px;
}
</style>
