<script>
export default {
    data() {
        return {
            slider: [
                {
                    image: "public/slider5.jpeg"
                },
                {
                    image: "public/slider4.jpg"
                },
                {
                    image: "public/slider3.jpg"
                },
                {
                    image: "public/slider2.jpg"
                },
                {
                    image: "public/slider1.jpg"
                },
            ],
            activeImg: 0
        }
    },
    created() {
        this.nextImg()
    },
    methods: {
        nextImg() {
            setInterval(() => {
                this.activeImg++
                if (this.activeImg == this.slider.length) {
                    this.activeImg = 0
                }
            }, 2000);
        }
    },
}
</script>
<template lang="">
    <section id="jumbo" class="d-none d-md-block text-center">
        <div class="container-fluid">
            <div class="row">
                <div class="col-12">
                    <div class="slider">
                        <img :src="slider[activeImg].image" alt="ecig" class="img-fluid">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>
@use '../styles/generals.scss';

#jumbo {
    margin-top: 70px;
}

img {
    max-height: 720px;
    width: 80vw;
}
</style>