<template>
    <div class="services-container">
        
       <h1 class="title">Our Services</h1>
       <div class="container">
        <div class="gallery">
            <div class="img-box"><h2>Buy a House</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quae?</p></div>
            <div class="img-box"><h2>Rent a House</h2> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quae?</p></div>
            <div class="img-box"><h2>Sell a House</h2> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quae?</p></div>
            <div class="img-box"><h2>Sell a House</h2> <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad, quae?</p></div>
        </div>
       </div>
    
    </div>
    </template>
    
    <script>
    export default {
        name: "Services",
    }
    </script>
    
    <style>

    .services-container{
        margin-top: 60px;
    }
    .title{
font-size: 35px;
text-align: center;
    }

    .container{
        width: 100%;
        height: 50vh;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .gallery{
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .img-box{
        width:250px;
        height:250px;
        margin:25px;
        border-radius: 20px;
        background: url(../assets/p6.jpg);
        background-size:cover;
        background-position: center;
        position: relative;
        transition: width 0.5s;

    }
    .img-box:nth-child(2){
        background: url(../assets/p2.jpg);
        background-size:cover;
        background-position: center;
    }
    .img-box:nth-child(3){
        background: url(../assets/p5.jpg);
        background-size:cover;
        background-position: center;
    }
    .img-box:nth-child(4){
        background: url(../assets/p4.jpg);
        background-size:cover;
        background-position: center;
    }

    .img-box h2{
        color: #FEFEFD;
        position: absolute;
        top: 70px;
        left: 70px
        
    }
    .img-box p{
        margin-top:20px;
        color: #FEFEFD;
        position: absolute;
        top: 100px;
        left: 50px
        
    }


    .img-box:hover{
        width:300px;
        height: 350px;
        cursor: pointer;
    }

    .img-box:hover h2{
        bottom: 25px;
    }

    </style>