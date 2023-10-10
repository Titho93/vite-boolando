<script>
export default {
    name: 'Header'
}
</script>

<template>

    <header>
        <div class="sticky">   
            <div class="container">
      
                <div class="bar">
                    <div class="menu">
                        <ul>
                            <li><a href="#"><strong>Donna</strong></a></li>
                            <li><a href="#"><strong>Uomo</strong></a></li>
                            <li><a href="#"><strong>Bambini</strong></a></li>
                                        
                        </ul>
                    </div>
               
                    <div class="logo"></div>
                    <div class="action">
                        <ul>
                            <li> <i class="fa-regular fa-user"></i></li>
                            <li><i class="fa-regular fa-heart"></i></li>
                            <li><i class="fa-solid fa-bag-shopping"></i></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </header>
  
</template>

<style lang="scss" scoped>

@use '../scss/partials/variables' as *;

header {
    box-shadow: 0px 1px 2px gray;
    background-color: $primary-color;
    .sticky {
        position: fixed;
        top: 0;
        height: 70px;
        z-index: 5;
        background-color: $primary-color;
        width: 100%
    }    
    .bar {
        display: flex;
        justify-content: space-between;
        height: 40px;
    }
    .menu {
        cursor: pointer;
        left: 0;
        color: $text-primary-color;
    }
    .action {
        cursor: pointer;
        right: 0;
        color: $text-primary-color;
    }
    .logo {
        text-align: center;
        background-image: url(/boolean-logo.png);
        width: 130px;
        height: 30px;
        background-position: center;
        background-size: contain;
        background-repeat: no-repeat;
        margin-left: -130px;
    }
}

</style>