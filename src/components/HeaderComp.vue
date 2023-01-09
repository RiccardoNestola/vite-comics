<script>

export default{
    data(){
        return{
            menuList: [
                {
                    text: "Characters",
                    url: "#",
                    active: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    active: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    active: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    active: false,
                },
                {
                    text: "Games",
                    url: "#",
                    active: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    active: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    active: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    active: false,
                },
                {
                    text: "News",
                    url: "#",
                    active: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    active: false,
                },
            ]
        }
    }
}

</script>

<template>

    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="" class="logo">
            <nav>
                <ul>
                    <li v-for="navItem in menuList" :class="(navItem.active) ? `active` : ``">
                    {{ navItem.text }}
                </li>
                </ul>
            </nav>
        </div>
    </header>

</template>

<style lang="scss" scoped>
    @use "../styles/general.scss" as *;
    @use "../styles/partials/variables" as *;   

    .container{
        height: 100px;
        display: flex;
        justify-content: space-around;
        align-items: center;

        img{
            width: 60px;
        }
        ul{
            list-style-type: none;
            display: flex;
            padding: 1rem;
        }
        li{
            padding: .8rem;
            text-transform: uppercase;
            font-weight: bold;
            font-size: .8rem;

            &:hover{
                color: $Main-Color;
            }
            &.active{
                border-bottom: 2px solid $Main-Color;
                width: 50%;
            }
        }
    }
        

</style>
