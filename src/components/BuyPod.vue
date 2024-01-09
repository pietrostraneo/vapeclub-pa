<script>
export default {
    data() {
        return {

        }
    },
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
                        <p class="fs-5">La nostra gamma comprende sigarette elettroniche di alta qualità, mod, vaporizzatori, liquidi e molto altro ancora. Selezioniamo con cura i migliori marchi e prodotti per garantirvi il meglio del meglio. Troverete sia marchi famosi che produttori emergenti che offrono prodotti innovativi ed entusiasmanti.</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="argus">
            <div class="container">
                <div class="row d-flex justify-content-center">
                    <div class="col-12 col-md-6 d-flex align-items-center order-md-0 order-1">
                        <p class="fs-5">Entra nel nostro mondo di liquidi per svapo e scopri il paradiso dei sapori. Sii pronto a liberare la tua fantasia, esplorare nuove frontiere gustative e lasciarti trasportare in un mondo di piacere aromatico senza limiti!</p>
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
                        <button>
                            SHOP NOW
                        </button>
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
        width: 70%;
    }

    p {
        color: white;
    }
}

button {
    @include btn_pod;
    font-family: 'Montserrat', sans-serif;
}
</style>