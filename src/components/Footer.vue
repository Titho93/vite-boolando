<script>
export default {
    name: 'Footer',
    data(){
        return{
            menu: [
                {
                    href: '#',
                    text: 'Informazioni legali'   
                },
                {
                    href: '#',
                    text: 'Informativa sulla privacy'   
                },
                {
                    href: '#',
                    text: 'Diritto di recesso'   
                },
            ],
            social: [
                {
                    href: '#',
                    font: 'fa-brands fa-square-twitter'
                },
                {
                    href: '#',
                    font: 'fa-brands fa-square-facebook'
                },
                {
                    href: '#',
                    font: 'fa-brands fa-square-instagram'
                },
                {
                    href: '#',
                    font: 'fa-brands fa-square-pinterest'
                },
                {
                    href: '#',
                    font: 'fa-brands fa-square-youtube'
                },
            ]
        }
    }
}
</script>

<template>

    <footer>
        <div class="container">
            <div class="information">
                <div class="menu">
                    <h2><strong>Boolando s.r.l</strong></h2>
                    <ul class="privacy">
                        <li v-for="(item,index) in menu"
                        :key="index"
                        ><a :href="item.href">{{ item.text }}</a></li>
                    </ul>
                </div>
                <div class="social">
                    <span><strong>Trovaci anche su</strong></span>
                    <ul>
                        <li v-for="(item,index) in social"
                        :key="index"
                        ><a :href="item.href"
                        ><i :class="item.font"></i></a></li>
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
    .privacy{
        li {
            font-size: 13px;
        }
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