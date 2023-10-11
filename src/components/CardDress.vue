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
            <span class="discount">{{ cardObj.discount }}</span>
            <span class="eco">{{ cardObj.sostenibilita}}</span>
        </div>
        <div class="bio">
            <h4>{{ cardObj.marca  }}</h4>
            <h3>{{ cardObj.modello  }}</h3>  
            <div class="price">
                <span class="low-price"><strong>{{ cardObj.fullPrice }}</strong></span>
                <span class="true-price"><s>{{ cardObj.lastPrice }}</s></span>
            </div>
        </div>
    </div>
  
</template>

<style lang="scss">

</style>