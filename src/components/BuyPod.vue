<script>
import AppJumbo from './AppJumbo.vue';
export default {
    components: {
        AppJumbo
    },
    data() {
        return {

        }
    },
    methods: {
        ageControl() {
            let age = confirm('Hai più di 18 anni?')
            if (age) {
                alert('ok')
            }
            else {
                alert('no')
            }
        }
    }
}
</script>
<template lang="">
    <main>

        <section class="argus">
            <div class="container">
                <div class="row d-md-flex justify-content-center">
                    <div class="col-12 col-md-4 d-flex justify-content-center">
                        <img src="../assets/8648_7.png" alt="argus" class="img-fluid">
                    </div>
                    <div class="col-12 col-md-6 d-flex align-items-center">
                        <p class="fs-4 text-center text-md-start">La nostra gamma comprende sigarette elettroniche di alta qualità, mod, vaporizzatori, liquidi e molto altro ancora. Selezioniamo con cura i migliori marchi e prodotti per garantirvi il meglio del meglio. Troverete sia marchi famosi che produttori emergenti che offrono prodotti innovativi ed entusiasmanti.</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="argus">
            <div class="container">
                <div class="row d-flex justify-content-center">
                    <div class="col-12 col-md-6 d-flex align-items-center order-md-0 order-1">
                        <p class="fs-4 text-center text-md-end">Entra nel nostro mondo di liquidi per svapo e scopri il paradiso dei sapori. Sii pronto a liberare la tua fantasia, esplorare nuove frontiere gustative e lasciarti trasportare in un mondo di piacere aromatico senza limiti!</p>
                    </div>
                    <div class="col-12 col-md-4 order-md-1 order-0 d-flex justify-content-center">
                        <img src="../assets/watson-20-ml.jpg.png" alt="watson" class="img-fluid ">
                    </div>
                </div>
            </div>
        </section>

        <section class="buttons my-3">
            <div class="container">
                <div class="row">
                    <div class="col-12 text-center">
                        <button @click="ageControl()">
                            SHOP NOW
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <AppJumbo />

        <section id="maps">
            <div class="container">
                <div class="row d-flex justify-content-center gap-1">
                    <div class="col-12 col-md-6">
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3137.3306372131406!2d13.328342375986203!3d38.1557546901227!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1319e8c6bd89a123%3A0xe55b53b11820a056!2sVape%20Club%20Palermo!5e0!3m2!1sit!2sch!4v1704829250391!5m2!1sit!2sch" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                    </div>
                    <div class="col-12 col-md-4 text-center">
                        <i class="fas fa-map-pin mb-4"></i>
                        <p class="fs-5">Siamo localizzati nel cuore della città, il punto di riferimento per gli amanti delle sigarette elettroniche. La nostra sede accogliente è il luogo ideale per trovare le ultime novità nel mondo delle e-cig, offrendo un'ampia gamma di prodotti e accessori di alta qualità. Il nostro staff esperto è pronto ad assistervi e guidarvi nella scelta migliore per le vostre esigenze di svapo. Venite a trovarci per un'esperienza di shopping dedicata al vostro piacere di vapori!</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>
<style lang="scss" scoped>
@use '../styles/generals.scss';
@use '../styles/partials/mixins' as *;

main {
    margin-top: 35px;
}

.argus {
    padding: 20px;
    margin: 0 45px;

    img {
        width: 80%;
    }

    p {
        @include text_pod;
    }
}

button {
    @include btn_pod;
    font-family: 'Montserrat', sans-serif;
}

#maps {
    margin-top: 120px;

    p {
        @include text_pod;
    }

    i {
        color: red;
        font-size: 8rem;
    }
}
</style>