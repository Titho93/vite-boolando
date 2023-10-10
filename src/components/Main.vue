<script>
export default {
    name: 'Main'
}
</script>

<template>

    <main>
        <div class="container">

            <div class="cards">

                <!-- 1 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/1.webp" alt="1.webp">
                    <img class="model-2" src="../assets/1b.webp" alt="1b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    <span class="discount">-50%</span>
                    <span class="eco">Sostenibilità</span>
                    </div>
                    <div class="bio">
                    <h4>Levi's</h4>
                    <h3>Relaxed fit tee unisex</h3>  
                    <div class="price">
                        <span class="low-price"><strong>14,99 €</strong></span>
                        <span class="true-price"><s>29,99</s></span>
                    </div>
                    </div>
                </div>

                <!-- 2 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/2.webp" alt="2.webp">
                    <img class="model-2" src="../assets/2b.webp" alt="2b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    <span class="discount">-30%</span>
                    </div>
                    <div class="bio">
                    <h4>Guess</h4>
                    <h3>Roses tee</h3>  
                    <div class="price">
                        <span class="low-price"><strong>20,99 €</strong></span>
                        <span class="true-price"><s>29,99</s></span>
                    </div>
                    </div> 
                </div>

                <!-- 3 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/3.webp" alt="3.webp">
                    <img class="model-2" src="../assets/3b.webp" alt="3b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    <span class="discount">-30%</span>
                    </div>
                    <div class="bio">
                    <h4>Come Zucchero Filato</h4>
                    <h3>Voglia di colori pastello</h3>  
                    <div class="price">
                        <span class="low-price"><strong>129,99 €</strong></span>
                        <span class="true-price"><s>184,99</s></span>
                    </div>
                    </div>
                </div>

                <!-- 4 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/4.webp" alt="4.webp">
                    <img class="model-2" src="../assets/4b.webp" alt="4b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    <span class="discount">-50%</span>
                    <span class="eco">Sostenibilità</span>
                    </div>
                    <div class="bio">
                    <h4>Levi's</h4>
                    <h3>Tee unisex</h3>  
                    <div class="price">
                        <span class="low-price"><strong>14,99 €</strong></span>
                        <span class="true-price"><s>29,99</s></span>
                    </div>
                    </div>
                </div>

                <!-- 5 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/5.webp" alt="5.webp">
                    <img class="model-2" src="../assets/5b.webp" alt="5b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    </div>
                    <div class="bio">
                    <h4>Maya Deluxe</h4>
                    <h3>Stripe bodice</h3>  
                    <div class="price">
                        <span class="low-price"><strong>99,99 €</strong></span>
                    </div>
                    </div>  
                </div>

                <!-- 6 card  -->
                <div class="card">
                    <div class="img">
                    <img class="model" src="../assets/6.webp" alt="6.webp">
                    <img class="model-2" src="../assets/6b.webp" alt="6b.webp">
                    <span class="heart"><i class="fa-solid fa-heart"></i></span>
                    <span class="eco single">Sostenibilità</span>
                    </div>
                    <div class="bio">
                    <h4>Esprit</h4>
                    <h3>Maglione - black</h3>  
                    <div class="price">
                        <span class="low-price"><strong>29,99 €</strong></span>
                    </div>
                    </div>
                </div>

            </div>
        </div>
    </main>
  
</template>

<style lang="scss" scoped>

@use '../scss/partials/variables' as *;

main {
    .cards {
        padding-top: 100px;
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    .card {
        width: calc(100% / 3 - 20px );
        height: 650px;
        position: relative;
        min-width: 250px;
    }
    .model {
        position: relative;
        z-index: 2;
        width: 100%;
        cursor: pointer;
    }
    .price {
        font-size: 12px;
    }
    .low-price {
        color: $color-discount;
    }

}

</style>