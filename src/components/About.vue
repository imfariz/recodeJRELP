<template>
    <section class="about container d-flex flex-column">
        <h3 class="text-center fw-bold fs-1 my-5">Tentang Kami</h3>
        <div class="phase1 d-flex flex-column flex-md-row my-5">
            <img :src="aboutSvg" alt="About Image" class="px-4 px-md-0 me-md-5">
            <p class="text-center text-md-start lh-lg fs-5 align-self-center">
                Creative House JRE Media, rumah bagi setiap bisnis
                untuk melakukan komunikasi kepada khalayaknya,
                Kami bekerja sebagai tim yang membantu bisnis anda
                untuk membuat konten kreatif, strategi pemasaran dan website.
            </p>
        </div>
        <div class="phase2 d-flex flex-column flex-md-row my-5 justify-content-evenly">
            <p class="text-center text-md-end lh-lg fs-5 order-1 order-md-0 align-self-center">
                Awali dengan perkenalan hangat antara kami dan bisnis Anda.
                Kami akan memulainya dengan menganalisis bisnis Anda.
                Riset sangat diperlukan untuk mengumpulkan data yang diperlukan.
                Tim kami akan melakukan proses brainstorming untuk mendapatkan
                hasil yang maskimal bagi kebutuhan bisnis Anda
            </p>
            <div class="image my-5 my-md-0 mx-auto mx-md-0 order-0 order-md-1"></div>
        </div>
    </section>
</template>
<script>
import aboutSvg from '@/assets/about.svg';

export default {
  name: 'About',
  data() {
    return {
      aboutSvg,
    };
  },
};
</script>

<style scoped>
.about {
    margin-bottom: 100px;
}

img {
    width: 450px;
    height: 300px;
}

p {
    font-weight: 500;
    width: 450px;
}

.image {
    background-image: url('https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80');
    background-size: cover;
    width: 300px;
    height: 300px;
    position: relative;
}

.image::after {
    content: "";
    display: block;
    width: 100%;
    height: 100%;
    position: absolute;
    z-index: 2;
    background-color: rgba(0, 0, 0, 0.3);
}

.image::before {
    content: "";
    display: block;
    background-color: antiquewhite;
    width: 100%;
    height: 100%;
    position: absolute;
    left: 30px;
    top: 30px;
    z-index: -1;
}
</style>
