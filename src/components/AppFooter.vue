<script>

export default{
    name:"AppFooter",
}

</script>

<template>
    <footer>
        <div class="footer-left">
            <h5>Addres</h5>
            <span class="d-block">382 NE 191st St # 87394 Miami, FL 33179-3899</span>
            <span class="d-block">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</span>
            <span class="d-block">support@maxcoach.com</span>
            <div class="socials">
                <i class="fa-brands fa-square-facebook"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin"></i>
            </div>


        </div>
        <div class="footer-right">
            <div class="explore">
                <h5>Explore</h5>
                <ul class="d-flex">
                    <li>Start here</li>
                    <li>Blog</li>
                    <li>About us</li>
                    <li>Success story</li>
                    <li>Courses</li>
                    <li>Contact us</li>
                </ul>

            </div>
            <div class="information">
                <h5>Information</h5>
                <ul>
                    <li>Membership</li>
                    <li>Purchase guide</li>
                    <li>Privacy policy</li>
                    <li>Terms of services</li>
                </ul>

            </div>

        </div>
    </footer>

</template>

<style lang="scss" scoped>
@use "../styles/partials/mixins.scss" as *;

footer{
    @include flex(row,space-between,start);
    width: 80%;
    margin:auto;
    padding-top: 3rem;
    color: grey;
    font-size:0.9rem;
    padding-bottom: 5rem;
    h5{
        color: black;
        font-size: 1.1rem;
        font-weight: bold;
        padding-bottom: 1rem;
    }
}

div.footer-left{
    width: 50%;

    span{
        padding-bottom:1rem;
    }

    i{
        padding-right: 0.5rem;
        font-size: 1.5rem;
    }
}

div.footer-right{
    @include flex(row,space-between,start);
    width: 50%;
    div.explore,div.information{
        width: 50%;
        @include flex(column,start,start);
        li{
            padding-bottom: 1rem;
        }
        
    }

    div.explore{
        margin-right: 2rem;
        ul{
            display: flex;
            flex-wrap: wrap;
        }

        li{
            width: 50%;
        }   
    }
}


</style>