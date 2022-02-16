<template>
    <section class="service container d-flex flex-column">
        <h3 class="text-center fw-bolder fs-1 my-5">Layanan</h3>
        <div class="web-development d-flex flex-column flex-md-row align-items-center">
            <div class="illustrasi" >
                <h5 class="text-center fs-1 mb-5 fw-bold">Web Development</h5>
                <img :src="service1Svg" alt="Service Image 1">
            </div>
            <div class="services ms-5">
                <div class="row">
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Desain Web
                        </h5>
                        <p class="description fs-6">
                            <b>Website</b> yang menarik akan membuat pengunjungnya
                            tertarik melihat halaman Anda. Kami dapat membuat
                            tampilan website menarik dan juga interaktif.
                        </p>
                    </div>
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Sistem Admin
                        </h5>
                        <p class="description fs-6">
                            Membuat sistem pada website sesuai kebutuhan Anda secara dinamis
                            dan otomatis.
                        </p>
                    </div>
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Hosting Domain
                        </h5>
                        <p class="description fs-6">
                            Layanan untuk membuat website Anda dapat dikunjungi dan terlihat oleh
                            khalayak.Dengan kata lain, hosting merupakan rumah dan domain merupakan
                            alamatnya.
                        </p>
                    </div>
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Konten
                        </h5>
                        <p class="description fs-6">
                            Membuat konten artikel, blog dan juga konten pendukung
                            di dalam website Anda agar dapat menarik pengunjung untuk
                            membacanya.
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <div class="creative-media d-flex flex-column flex-md-row align-items-center">
            <div class="services ms-5 order-1 order-md-0">
                <div class="row">
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Marketing Tools
                        </h5>
                        <p class="description fs-6">
                            Perlengkapi bisnis Anda dengan
                            alat promosi atau marketing,
                            seperti company profile, booklet,
                            presentasi, brosur, kartu nama,
                            map, product knowledge
                            dan sebagainya
                        </p>
                    </div>
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Creative Content
                        </h5>
                        <p class="description fs-6">
                            Mempertahankan sebuah bisnis
                            didukung oleh konten bisnis yang kreatif.
                            Berikan warna bagi bisnis Anda dengan konten
                            seperti komik,infografis, video komik, artikel
                            SEO Friendly dan sebagainya.
                        </p>
                    </div>
                    <div class="card p-4 text-center text-md-start">
                        <div class="head-logo mb-4 fs-1">
                            <i class="bi bi-tv-fill"></i>
                        </div>
                        <h5 class="card-title mb-4 fs- fw-bold">
                            Hosting Domain
                        </h5>
                        <p class="description fs-6">
                            Era digital menuntut semua bisnis untuk bersaing di dalamnya.
                            Salah satu cara yaitu kami membantu Anda untuk membuat langkah
                            strategi media sosial, konten media sosial dan juga pengelolaannya.
                        </p>
                    </div>
                </div>
            </div>
            <div class="illustrasi order-0 order-md-1" >
                <h5 class="text-center fw-bold fs-1 mb-5">Media Creative</h5>
                <img :src="service2Svg" alt="Service Image 2">
            </div>
        </div>
    </section>
</template>

<script>
import service1Svg from '@/assets/service1.svg';
import service2Svg from '@/assets/service2.svg';

export default {
  name: 'Service',
  data() {
    return {
      service1Svg,
      service2Svg,
    };
  },
};
</script>

<style scoped>
.service {
    margin-bottom: 150px;
}

.card {
    width: 385px;
    height: 330px;
    margin: 0.5em;
}

.card:hover {
    box-shadow: 2px 2px 5px 1px rgba(0, 0, 0, 0.15);

}

.card p {
    color: #949494;
    font-weight: 400;
}

.creative-media {
    margin-top: 15em;
}

.creative-media .card {
    width: 380px;
    height: 350px;
}

img {
    width: 450px;
    height: 450px;
}
</style>
