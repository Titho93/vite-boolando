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
            <img class="model" :src="`/assets/${cardObj.primaryImage}`" alt="cardObj.modello">
            <img class="model-2" :src="`/assets/${cardObj.secondaryImage}`" alt="name object..">
            <span class="heart"><i class="fa-solid fa-heart"></i></span>
            <span v-if="cardObj.discount" class="discount">{{ cardObj.discount }}</span>
            <span v-if="cardObj.sostenibilita" class="eco">{{ cardObj.sostenibilita}}</span>
        </div>
        <div class="bio">
            <h4>{{ cardObj.marca  }}</h4>
            <h3>{{ cardObj.modello  }}</h3>  
            <div class="price">
                <span class="low-price"><strong>{{ cardObj.lastPrice }}</strong></span>
                <span class="true-price"><s>{{ cardObj.fullPrice }}</s></span>
            </div>
        </div>
    </div>
  
</template>

<style lang="scss">

</style>