<script>
export default {
    name: 'CardDress',

    props : {
        cardObj : Object
    },
    data(){
        return{

        }
    },
}
</script>

<template>

    <div class="card">
        <div class="img">
            <img class="model" :src="`/assets/${cardObj.primaryImage}`" alt="1.webp">
            <img class="model-2" :src="`/assets/${cardObj.secondaryImage}`" alt="1b.webp">
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
  
</template>

<style lang="scss">

</style>