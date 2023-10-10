<script>
export default {
    name: 'Footer'
}
</script>

<template>

    <footer>
        <div class="container">
            <div class="information">
                <div class="menu">
                    <h2><strong>Boolando s.r.l</strong></h2>
                    <ul class="privacy">
                        <li><a href="#">Informazioni legali</a></li>
                        <li><a href="#">Informativa sulla privacy</a></li>
                        <li><a href="#">Diritto di recesso</a></li>            
                    </ul>
                </div>
                <div class="social">
                    <span><strong>Trovaci anche su</strong></span>
                    <ul>
                        <li><a href="#"><i class="fa-brands fa-square-twitter"></i></a></li>
                        <li><a href="#"><i class="fa-brands fa-square-facebook"></i></a></li>
                        <li><a href="#"><i class="fa-brands fa-square-instagram"></i></a></li>
                        <li><a href="#"><i class="fa-brands fa-square-pinterest"></i></a></li>
                        <li><a href="#"><i class="fa-brands fa-square-youtube"></i></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
  
</template>

<style lang="scss" scoped>

@use '../scss/partials/variables' as *;

footer {
    background-color: $text-secondary-color;
    height: 90px;
    .information {
        display: flex;
        justify-content: space-between;
    }
    .privacy li {
        font-size: 13px;
    }
    .social {
        margin-right: 50px;
        color: $text-primary-color;

        span {
            font-size: 12px;
            color: $text-primary-color;
        }
        a {
            padding: 0px;
        }
    }
}

</style>