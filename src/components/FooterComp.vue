<script>
export default{
    data(){
        return{
            DcMenu: [
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
                    text: "Videos",
                    url: "#",
                    active: false,
                },
                {
                    text: "News",
                    url: "#",
                    active: false,
                },
            ],

            ShopMenu: [
                {
                    text: "Shop DC",
                    url: "#",
                    active: false,
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                    active: true,
                },
            ],

            DcMenu: [
                {
                    text: "Terms Of Use",
                    url: "#",
                    active: false,
                },
                {
                    text: "Privacy policy (New)",
                    url: "#",
                    active: true,
                },
                {
                    text: "Ad Choices",
                    url: "#",
                    active: false,
                },
                {
                    text: "Advertising",
                    url: "#",
                    active: false,
                },
                {
                    text: "Jobs",
                    url: "#",
                    active: false,
                },
                {
                    text: "Subscriptions",
                    url: "#",
                    active: false,
                },
                {
                    text: "Talent Workshops",
                    url: "#",
                    active: false,
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                    active: false,
                },
                {
                    text: "Ratings",
                    url: "#",
                    active: false,
                },
                {
                    text: "Shop Help",
                    url: "#",
                    active: false,
                },
                {
                    text: "Contact Us",
                    url: "#",
                    active: false,
                },
            ],

            SitesMenu: [
                {
                    text: "DC",
                    url: "#",
                    active: false,
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                    active: false,
                },
                {
                    text: "DC Kids",
                    url: "#",
                    active: false,
                },
                {
                    text: "DC Universe",
                    url: "#",
                    active: false,
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                    active: false,
                },
            ],
        }
    }
}
</script>

<template>
    <footer>
        <div class="menu_container">
            <div class="nav">
                <div>
                    <ul>
                        <li><h4>Dc Comics</h4></li>
                        <li v-for="Item in DcMenu">
                            {{Item.text }}
                        </li>
                    </ul>
                    <ul>
                        <li><h4>Shop</h4></li>
                        <li v-for="Item in ShopMenu">
                            {{ Item.text }}
                        </li>
                    </ul>
                </div>
    
                <ul>
                    <li><h4>Dc</h4></li>
                    <li v-for="Item in DcMenu">
                        {{ Item.text }}
                    </li>
                </ul>
    
                <ul>
                    <li><h4>Sites</h4></li>
                    <li v-for="Item in SitesMenu">
                        {{ Item.text }}
                    </li>
                </ul>
            </div>
    
            <div class="logo">
                <img src="../assets/img/dc-logo-bg.png" alt="Logo Dc">
            </div>
        </div>
    </footer>

    <div class="sub_footer">
        <div class="social_container">
            <div class="call_to_action">
                <h4>Sign-up Now!</h4>
            </div>
            <div class="icons">
                <h3>Follow Us</h3>
                <ul class="icons">
                    <li>
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;
@use "../styles/partials/variables" as *;   

footer{
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    .menu_container{
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        overflow: hidden;
        .nav{
            display: flex;
            padding: 3rem 0;
        }
        .logo{
            position: relative;

            img{
                position: absolute;
                top: -20%;
                right: 0;
            }
        }
    }

    ul{
        list-style-type: none;
        margin-right: 2rem;
        margin-bottom: 2rem;
        

        li{
            font-size: 0.9rem;
            line-height: 1.4rem;
            color: $Secondary-Color;
        }
    }

}

h4{
    text-transform: uppercase;
    font-size: 1rem;
    color: white;
}
    .sub_footer{
    background-color: #303030;


    .social_container{
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        padding: 1.5rem;

        .call_to_action{
            border: 2px solid $Main-Color;
            padding: 1rem;
        }
        .icons{
            display: flex;
            align-items: center;

            h3{
                color: $Main-Color;
                text-transform: uppercase;
            }

            ul{
                list-style-type: none;
                margin-left: 1.5rem;

                li{
                    display: inline-block;
                    padding-right: 1.5rem;
                }
            }
        }
    }
}

</style>