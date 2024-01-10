<script>
export default {
    name: 'AppMenu',
    data() {
        return {

        }
    },

}
</script>
<template lang="">
    <header>
        <div class="container-fluid">
            <div class="row d-flex justify-content-between align-items-center">
                <div class="col-12 col-md-3 text-center">
                    <img src="../assets/logo.png" alt="" class="img-fluid">
                </div>
                <div class="col-12 col-md-6 d-flex align-items-center justify-content-center ">
                    <div class="nav">
                        <ul class="list-unstyled text-uppercase gap-5 d-flex">
                            <li>Products</li>
                            <li>Gallery</li>
                            <li>About Us</li>
                        </ul>
                    </div>
                </div>
                <div class="col-12 col-md-3 d-flex align-items-center justify-content-center">
                    <div class="social d-flex gap-3 align-items-center">
                        <i class="fab fa-instagram"></i>
                        <i class="fab fa-facebook"></i>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
@use '../styles/generals.scss';

header img {
    width: 65%;
}

i {
    color: white;
    font-size: 2.00rem;
}

.fa-instagram:hover {
    color: blueviolet;
}

.fa-facebook:hover {
    color: rgb(53, 53, 252);
}
</style>