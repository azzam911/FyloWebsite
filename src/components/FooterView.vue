<template>
    <footer>
        <div class="box">
            <h1>Get early access today</h1>
            <p>it only takes a minutes to sign up and our free starter tier is extremky generous.
                if you have any questions, our support team would be happy to help you.
            </p>
            <div class="ask-form">
                <form @submit.prevent>
                    <input type="text" name="" placeholder="email@example.com">
                    <input type="submit" value="Get Started Free">
                </form>
            </div>
        </div>

        <div class="footer-info">
            
            <div>
                
                <div>
                    <i class="fa-solid fa-location-dot"></i>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure fuga beatae placeat in repudiandae blanditiis laboriosam sapiente accusamus? Magnam, officia maiores a quibusdam suscipit aliquid voluptatibus aperiam ab itaque excepturi.</p>
                </div>
            </div>
            <div class="flex-colmun">
                <div class="phone">
                    <i class="fa-solid fa-phone-volume"></i>
                    +1-543-123-4567
                </div>
                <div class="email">
                    <i class="fa-solid fa-envelope"></i>
                    Email@example.com
                </div>
            </div>
            <div class="flex-colmun">
                <router-link to="about">About Us</router-link>
                <router-link to="jobs">Jobs</router-link>
                <router-link to="press">Press</router-link>
                <router-link to="blog">Blog</router-link>
            </div>
            <div class="flex-colmun">
                <router-link to="contact">Contact Us</router-link>
                <router-link to="terms">Terms</router-link>
                <router-link to="privacy">Privacy</router-link>
            </div>
            <div>
                <div class="social-media">
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-instagram"></i>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name : 'FooterView',
    data() {

    }
}
</script>


<style>
footer {
    padding: 30px;
    background-color: #0c1524;
    position: relative;
    height: 500px;
}
footer .box {
    padding: 20px;
    background-color: #0c1524;
    width: 500px;
    position: absolute;
    box-shadow: 0px 1px 10px #000;
    top: -60px;
    left: 50%;
    transform: translateX(-50%);
    color: #fff;
}
footer .box p {
    margin: 20px 0;
}

footer .ask-form form {
    display: flex;
    justify-content: space-evenly;
    gap: 30px;
}

footer .ask-form form input {
    padding: 10px;
    border-radius: 20px;
}
footer .ask-form form input[type = 'text']{
    color: #000;
}

footer .ask-form form input[type = 'submit'] {
    background-color: #46b6d0;
}
footer .footer-info {
    display: flex;
    justify-content: space-around;
    height: 100%;
    align-items: center;
    gap: 30px;
}
footer .footer-info div {
    display: flex;
    max-width: 250px;
    text-align: left;
}
footer .footer-info i {
    font-size: 15px;
}
footer .flex-colmun {
    flex-direction: column;
}

@media screen and (max-width: 500px) {
    footer .box {
        width: 380px;
    }
}
</style>