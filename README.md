<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Meena Bazaar Social Links</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html,body{
    width:100%;
    min-height:100%;
}

body{
    font-family:'Segoe UI',Tahoma,Geneva,Verdana,sans-serif;
    min-height:100svh;
    overflow:hidden;
    position:relative;
    display:grid;
    place-items:center;
}

/* VIDEO BACKGROUND */
#bg-video{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    object-fit:cover;
    z-index:-2;
}

/* DARK OVERLAY */
body::before{
    content:"";
    position:fixed;
    inset:0;
    background:rgba(0,0,0,0.35);
    z-index:-1;
}

/* CENTER CONTENT */
.container{
    width:min(90vw,420px);
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    text-align:center;
}

/* LOGO */
.logo{
    width:min(160px,40vw);
    height:auto;
    margin-bottom:10px;
    border-radius:12px;
}

/* HEADING */
h1{
    color:#fff;
    font-size:clamp(24px,5vw,34px);
    margin-bottom:20px;
    text-shadow:0 2px 5px rgba(0,0,0,.4);
}

/* BUTTONS */
.social-links{
    width:100%;
    display:flex;
    flex-direction:column;
    align-items:center;
    gap:14px;
}

.social-links a,
.social-links .location-card{
    text-decoration:none;
    color:white;
    width:100%;
    max-width:270px;
    padding:14px 20px;
    border-radius:14px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    font-size:17px;
    font-weight:600;
    transition:all .3s ease;
}

.social-links a img,
.social-links .location-card img{
    width:24px;
    height:24px;
    flex-shrink:0;
}

/* LOCATION CARD TEXT */
.location-card{
    text-align:left;
    line-height:1.35;
    font-size:14.5px;
    font-weight:500;
    cursor:default;
}

.location-card strong{
    display:block;
    font-size:16px;
    font-weight:700;
    margin-bottom:2px;
}

/* COLORS */
.head-office{
    background:#106185;
}

.get-location{
    background:#8B1E3F;
    cursor:pointer;
}

.whatsapp-customer{
    background:#128C7E;
}

.website{
    background:#ff3399;
}

.instagram{
    background:#ffc014;
}

.youtube{
    background:#FF0000;
}

/* HOVER */
.social-links a:hover,
.get-location:hover{
    transform:scale(1.05);
    box-shadow:
    0 0 10px #ffee02,
    0 0 20px #ff2727,
    0 0 30px #0effcb,
    0 0 40px currentColor;
}

/* LOCATION DROPDOWN */
.location-box{
    width:100%;
    max-width:270px;
    display:none;
    flex-direction:column;
    gap:8px;
    margin-top:-5px;
}

.location-box a{
    width:100%;
    max-width:270px;
    padding:11px 14px;
    border-radius:10px;
    background:rgba(255,255,255,0.95);
    color:#222;
    text-decoration:none;
    font-size:13px;
    font-weight:600;
    text-align:left;
    transition:.2s;
}

.location-box a:hover{
    background:#fff;
    transform:scale(1.02);
}

/* MOBILE */
@media(max-width:380px){

    .social-links a,
    .social-links .location-card{
        max-width:240px;
        font-size:16px;
        padding:12px 16px;
    }

    .location-card{
        font-size:13.5px;
    }

    .location-box,
    .location-box a{
        max-width:240px;
    }

    .location-box a{
        font-size:12.5px;
    }

    .logo{
        width:130px;
    }
}
</style>
</head>

<body>

<!-- VIDEO BACKGROUND -->
<video autoplay muted loop playsinline id="bg-video">
    <source src="https://raw.githubusercontent.com/Datamanagermbkb/embvideo/main/Sequence%2001_1.mp4" type="video/mp4">
</video>

<div class="container">

    <img
      src="https://www.amanoramall.com/assets/images/brand/wr3jvWWCeYiL8xAwYx3XfJIG4gstAY.jpg"
      alt="Meena Bazaar Logo"
      class="logo">

    <h1>Connect with Meena Bazaar</h1>

    <div class="social-links">

        <!-- HEAD OFFICE -->
        <a href="https://maps.app.goo.gl/JViLEceJpPUNypLZ7"
           class="location-card head-office"
           target="_blank">
            <img src="https://img.icons8.com/?size=256w&id=YFY0zG9WOavq&format=png" alt="">
            <span>
                <strong>Visit our NEW FLAGSHIP STORE &amp; CORPORATE HEAD OFFICE -</strong>
                MOULSARI AVENUE
            </span>
        </a>


        <!-- GET LOCATION -->
        <a href="javascript:void(0)"
           class="get-location"
           onclick="toggleLocations()">

            <img src="https://img.icons8.com/?size=256w&id=7880&format=png" alt="">

            GET LOCATION

        </a>


        <!-- ALL LOCATIONS -->
        <div class="location-box" id="locationBox">

            <a href="https://maps.app.goo.gl/sppTruArBQHbdqQb6"
               target="_blank">
                📍 KAROL BAGH
            </a>

            <a href="https://maps.app.goo.gl/ESDS1ks4Vu7ZY9ur8"
               target="_blank">
                📍 KAMLA NAGAR
            </a>

            <a href="https://maps.app.goo.gl/71vWQB6jjSKtRnhd8"
               target="_blank">
                📍 CROWN PLAZA FARIDABAD
            </a>

            <a href="https://maps.app.goo.gl/xCGPFwRgJ3SzgHLG6"
               target="_blank">
                📍 EAST DELHI MALL
            </a>

            <a href="https://maps.app.goo.gl/DJTbH5g2fWXV49yY7"
               target="_blank">
                📍 GREAT INDIA PLACE
            </a>

            <a href="https://maps.app.goo.gl/rG7soXXA1KbudXJfA"
               target="_blank">
                📍 MALL OF INDIA
            </a>

            <a href="https://maps.app.goo.gl/yTBWo5CJR1iVwjiR9"
               target="_blank">
                📍 AMBIENCE MALL, GURUGRAM
            </a>

            <a href="https://maps.app.goo.gl/yTuBJBbCc6Ys4VRZ8"
               target="_blank">
                📍 GAUR CITY MALL
            </a>

            <a href="https://maps.app.goo.gl/ATTDZkqhrYRUR3m9A"
               target="_blank">
                📍 CENTRIO UNISON MALL, DEHRADUN
            </a>

            <a href="https://maps.app.goo.gl/F5n1CTZjgLcSj6A8A"
               target="_blank">
                📍 PATHANKOT - DOWNTOWN MALL
            </a>

            <a href="https://maps.app.goo.gl/KfsNtXDcTfKsaEwA7"
               target="_blank">
                📍 PACIFIC MALL, JASOLA
            </a>

            <a href="https://maps.app.goo.gl/KbBGAtZSDw6dt1Ti8"
               target="_blank">
                📍 LULU MALL, LUCKNOW
            </a>

            <a href="https://maps.app.goo.gl/dzPxP9oUHvnHx3hH9"
               target="_blank">
                📍 PALLADIUM MALL, AHMEDABAD
            </a>

            <a href="https://maps.app.goo.gl/7v8Tz8MowEpQKX9B7"
               target="_blank">
                📍 FORUM SOUTH BANGALORE
            </a>

            <a href="https://maps.app.goo.gl/XG2yVvYRDruBXdxn6"
               target="_blank">
                📍 CP 67, MOHALI
            </a>

            <a href="https://maps.app.goo.gl/HkLzVoMrHRCgni3R9"
               target="_blank">
                📍 THE MALL OF FARIDABAD
            </a>

            <a href="https://maps.app.goo.gl/vAQMxMQmoZ5G5JJJ9"
               target="_blank">
                📍 MALL OF RANCHI
            </a>

            <a href="https://maps.app.goo.gl/ADGcc2AU9MMfCStX8"
               target="_blank">
                📍 MALL OF AVADH, AYODHYA
            </a>

            <a href="https://maps.app.goo.gl/Jn99C4tRoMJ6fALp9"
               target="_blank">
                📍 BHUBANESWAR
            </a>

            <a href="https://maps.app.goo.gl/A3JdufYpzTgBD6pZ8"
               target="_blank">
                📍 ICON PLAZA MALL, MUZAFFARPUR
            </a>

            <a href="https://share.google/k5Ehzxhwqpc7xhVyg"
               target="_blank">
                📍 M5 ELECTRONIC CITY MALL, BENGALURU
            </a>

            <a href="https://share.google/o5s0NRQuv5dSaXvoJ"
               target="_blank">
                📍 CENTRAL MARKET, SECTOR 120, NOIDA
            </a>

            <a href="https://share.google/Kuf3IOpn6VVoQUJBL"
               target="_blank">
                📍 ZORA THE MALL, RAIPUR
            </a>

            <a href="https://share.google/fH5XVhnGD3B9sk1LM"
               target="_blank">
                📍 UNITY ONE ELEGANTE, PITAMPURA
            </a>

            <a href="https://maps.app.goo.gl/JViLEceJpPUNypLZ7"
               target="_blank">
                📍 MOULSARI AVENUE, GURUGRAM
            </a>

        </div>


        <!-- WEBSITE -->
        <a href="https://meenabazaar.com/"
           class="website"
           target="_blank">

            <img src="https://www.amanoramall.com/assets/images/brand/wr3jvWWCeYiL8xAwYx3XfJIG4gstAY.jpg" alt="">

            Website

        </a>


        <!-- INSTAGRAM -->
        <a href="https://www.instagram.com/meenabazaar/"
           class="instagram"
           target="_blank">

            <img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png" alt="">

            Instagram

        </a>


        <!-- YOUTUBE -->
        <a href="https://www.youtube.com/channel/UCxuqspu5N8CZThWFc8xa9ig"
           class="youtube"
           target="_blank">

            <img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png" alt="">

            YouTube

        </a>


        <!-- WHATSAPP -->
        <a href="https://api.whatsapp.com/send?phone=917303888641&text=Hi+I+have+a+query.+Can+you+help%3F"
           class="whatsapp-customer"
           target="_blank">

            <img src="https://cdn-icons-png.flaticon.com/512/733/733585.png" alt="">

            WhatsApp - Customer Care

        </a>

    </div>

</div>


<script>

function toggleLocations(){

    const box = document.getElementById("locationBox");

    if(box.style.display === "flex"){

        box.style.display = "none";

    }else{

        box.style.display = "flex";

    }

}

</script>

</body>
</html>
