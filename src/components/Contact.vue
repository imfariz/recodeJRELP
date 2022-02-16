<template>
    <section class="contact">
        <h3 class="text-center my-5 fw-bold fs-1">Hubungi Kami</h3>
        <div class="d-flex flex-column flex-md-row container align-items-center text-start">
            <img :src="contactSvg" alt="Contact Image" class="px-5 px-md-0">
            <form class="form form-contact w-75 bg-light-red ms-md-5 rounded-3 p-5">
                <div class="row d-flex flex-column flex-md-row">
                    <div class="form-floating mb-3 col-12 col-md-6">
                        <input type="email" class="form-control" id="floatingInput"
                        placeholder="name@example.com">
                        <label for="floatingInput" class="ms-3">Nama</label>
                    </div>
                    <div class="form-floating mb-3 col-12 col-md-6">
                        <input type="email" class="form-control" id="floatingInput"
                        placeholder="name@example.com">
                        <label for="floatingInput" class="ms-3">Telephone</label>
                    </div>
                </div>
                <div class="row d-flex flex-column flex-md-row">
                    <div class="form-floating mb-3 col-12 col-md-6">
                        <input type="email" class="form-control" id="floatingInput"
                        placeholder="name@example.com">
                        <label for="floatingInput" class="ms-3">Email</label>
                    </div>
                    <div class="form-floating mb-3 col-12 col-md-6">
                        <input type="email" class="form-control" id="floatingInput"
                        placeholder="name@example.com">
                        <label for="floatingInput" class="ms-3">Subjek (Optional)</label>
                    </div>
                </div>
                <div class="form-floating">
                    <textarea class="form-control" placeholder="Leave a comment here"
                    id="floatingTextarea"></textarea>
                    <label for="floatingTextarea">Pesan Anda</label>
                </div>
                <button class="btn btn-red p-2 mt-5 mt-md-4 w-50 text-center rounded-3">
                    Kirim Pesan
                </button>
            </form>
        </div>
    </section>
</template>

<script>
import contactSvg from '@/assets/contact.svg';

export default {
  name: 'Contact',
  data() {
    return {
      contactSvg,
    };
  },
};
</script>

<style scoped>
.contact {
    margin-bottom: 150px;
}

img {
    width: 400px;
    height: 400px;
}

.form-contact {
    height: fit-content;
}

.bg-light-red {
    background-color: #FFF9F9;
}

.btn-red {
    color: #FFFFFF;
    background-color: #F50057;
}

.btn-red:hover {
    color: #121212;
}

label {
    color: #8B8B8B;
}
</style>
