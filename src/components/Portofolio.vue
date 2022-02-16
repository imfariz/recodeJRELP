<template>
    <section class="portofolio">
        <div class="container text-center">
            <h3 class="fw-bold fs-1">Portofolio</h3>
            <p class="fs-5 my-5">
                Silakan masuk ke dalam ruang kreatif kami <br>
                dan lihat apa yang sudah pernah <br>
                kami kerjakan
            </p>
            <div class="catalog my-5 d-flex flex-column flex-md-row p-4">
                <div class="row g-5">
                    <div class="porto col-md-4" v-for="porto in porto" :key="porto">
                        <img :src="porto.imagePath"
                        alt="Portofolio Image">
                        <div class="description text-white text-center">
                            <h5 class="lh-base">{{ porto.client }}</h5>
                            <p class="fs-6">{{ porto.Category }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Portofolio',
  data() {
    return {
      porto: [{
        imagePath: 'https://images.unsplash.com/photo-1618354691373-d851c5c3a990?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=715&q=80',
        client: 'XBRAND',
        Category: 'Desain Ilustrasi TShirt',
      }, {
        imagePath: 'https://images.unsplash.com/photo-1507238691740-187a5b1d37b8?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=755&q=80',
        client: 'PT XASDDAS',
        Category: 'Website Development',
      }, {
        imagePath: 'https://images.unsplash.com/photo-1481487196290-c152efe083f5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1924&q=80',
        client: 'PT XASDDAS',
        Category: 'Website Development',
      }, {
        imagePath: 'https://images.unsplash.com/photo-1467232004584-a241de8bcf5d?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1169&q=80',
        client: 'PT XASDDAS',
        Category: 'Website Development',
      }, {
        imagePath: 'https://images.unsplash.com/photo-1530435460869-d13625c69bbf?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80',
        client: 'PT XASDDAS',
        Category: 'Website Development',
      }, {
        imagePath: 'https://images.unsplash.com/photo-1522199755839-a2bacb67c546?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1172&q=80',
        client: 'PT XASDDAS',
        Category: 'Website Development',
      }],
    };
  },
};
</script>

<style scoped>
.portofolio {
  margin-bottom: 150px;
}

.portofolio .container > p {
    color: #949494;
}

.porto {
    height: 400px;
    min-width: 400px;
    position: relative;
}

.porto:hover img{
    opacity: 0.3;
}

.porto:hover .description{
    opacity: 1;
}

.description {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .5s ease;
    background-color: rgba(0, 0, 0, 0.6);
}

.description p {
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    position: absolute;
    top: 50%;
    left: 50%;
}

.description h5 {
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
    position: absolute;
    top: 45%;
    left: 50%;
}

img {
    display: block;
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: .5s ease;
}

</style>
