<template>
    <div class="container">
        <div class="home">
            <img src="../assets/images/pananr.jpg" alt="">
            <div class="home-text">
                <h1>All your files in one secure location, accessible anywhere.</h1>
                <p>Fylo stores all your most important files in one secure location.</p>
                <p>Access them wherever you need, share and collaborate with friends family, and co-workers.</p>
                <button>Get Started</button>
            </div>
        </div>

        <!---------- Start About -------------->

        <div class="about">
            <div class="about-cont row">
                    <div class="col-5 cards">
                        <i class="fa-solid fa-computer"></i>
                        <h3>Access your files, anywhere</h3>
                        <p>The ability to use a smartphone, tablet, or computer
                            to access your account means your files follow you everywhere
                        </p>
                    </div>
                    <div class="col-5 cards">
                        <i class="fa-solid fa-user-shield"></i>
                        <h3>Security you can trust</h3>
                        <p>2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files</p>
                    </div>
                    <div class="col-5 cards">
                        <i class="fa-solid fa-user-check"></i>
                        <h3>Real-time collaboration</h3>
                        <p>Secure share files and folders with friends, family and colleagues for live collaboration.
                            No email attachments required.
                        </p>
                    </div>
                    <div class="col-5 cards">
                        <i class="fa-solid fa-database"></i>
                        <h3>Store any type of file</h3>
                        <p>Weather you'r sharing holidays photos or work documents, Fylo has you covered allowing for all file types to be securely stored and shared.</p>
                    </div>
            </div>
        </div>
        <!---------- End About -------------->


        <!---------- Start Services  -------------->
        <div class="services">
            <div class="service-con">
                <div>
                    <img src="../assets/images/services.jpg" alt="">
                </div>
                <div>
                    <h1>Stay Productive,
                        wherever you are
                    </h1>
                    <p>never let location be an issue when accessing your files. Fylo has you coverd for all of your file storage needs.</p>
                    <p>Securely share files and folders with friends, family and colleagues for live collaboration. No email attachments required.</p>
                    <router-link to="about" class="fylo-link">See how Fylo works</router-link>
                </div>
            </div>
        </div>
        <!---------- End Services  -------------->



        <!---------- Start Users  -------------->

        <div class="users">
            <div class="comments">
                <div>
                    <p>
                        Fylo has improved our team productivity by an order of magnitude. 
                        Since making the switch our team has become a well-oiled collaboration machine
                    </p>
                    <div class="user-info">
                        
                        <i class="fa-solid fa-user"></i>
                        <div>
                            <h2>Satish Patel</h2>
                            <p>Files and Folders</p>
                        </div>
                    </div>
                </div>
                <div>
                    <p>
                        Fylo has improved our team productivity by an order of magnitude. 
                        Since making the switch our team has become a well-oiled collaboration machine
                    </p>
                    <div class="user-info">
                        
                        <i class="fa-solid fa-user"></i>
                        <div>
                            <h2>Satish Patel</h2>
                            <p>Files and Folders</p>
                        </div>
                    </div>
                </div>
                <div>
                    <p>
                        Fylo has improved our team productivity by an order of magnitude. 
                        Since making the switch our team has become a well-oiled collaboration machine
                    </p>
                    <div class="user-info">
                        
                        <i class="fa-solid fa-user"></i>
                        <div>
                            <h2>Satish Patel</h2>
                            <p>Files and Folders</p>
                        </div>
                    </div>
                </div>
                
            </div>
        </div>
        <!---------- End Users  -------------->
        
    </div>
    
</template>

<script>
export default {
    name:'HomeView'
}
</script>


<style>

.container {
    max-width: 1000px;
    margin: 0 auto;
    color: #fff;
}
.home {
    width: 100%;
    text-align: center;
}
.home img {
    margin: 0 auto;
}
.home .home-text {
    margin: 20px auto;
}
.home-text h1 {
    font-size: 30px;
}
.home-text p {
    margin: 10px 0px;
    font-size: 18px;
}
.home-text button {
    background-color: #4cc2d3;
    padding: 10px 100px;
    border-radius: 20px;
    font-size: 20px;
    margin-top: 40px;
}

/* ---------------------- Start About ---------------------- */
.about {
    margin: 40px auto;
}

.row {
    justify-content: center;
    gap: 50px;
}
.cards {
    display: flex;
    flex-direction: column;
    gap: 10px;
}
.cards h3 {
    font-size: 25px;
}
i {
    color: #468385;
    font-size: 30px;
}
/* ----------------------- End About ------------------------------ */


/* ----------------------- Start Services ------------------------------ */
.services {
    margin: 100px auto;
}
.service-con {
    display: flex;
    gap: 100px;
    align-items: center;
}
.service-con div img {
    width: 1000px;
}
.fylo-link {
    text-decoration: solid !important;
    color: #468385;
}
.service-con div h1 {
    font-size: 25px;
}
/* ----------------------- End Services ------------------------------ */


/* ----------------------- Start Comments ------------------------------ */
.users {
    margin: 100px auto;
}

.comments {
    display: flex;
    gap: 70px;
}
.comments div {
    text-align: left;
    padding: 5px;
    background-color: #10161e;
}
.comments .user-info {
    margin: 10px 0;
    display: flex;
    align-items: center;
}
/* ----------------------- End Comments ------------------------------ */
</style>

