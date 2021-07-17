<template>
    <div class="mobile voicedBy">
        <div class="flex voicedBy-container"> 
            <div class="flex upper-voicedBy"> 
                <span class="txt-1">Voiced By</span>
                <span class="txt-2">Rakesh</span>
            </div>
              <div class="absolute">
                <img src="../assets/rakesh.svg" alt="rakesh">
            </div>
        </div>
        <div>
            <div class="flex items-center lower-voicedBy"> 
                <span>Follow My Content</span>
                <div class="flex items-center"> 
                    <img class="img-1" src="../assets/like.svg" alt="fb">
                    <img src="../assets/youtube.svg" alt="youtube">
                </div>
                <button>More Pranks with <b class="ml-1"> Rakesh </b><img src="../assets/arrow.svg"></button>
            </div>
        </div>
    </div>
    <div class="desktop"> 
         <div class="flex voicedBy-container"> 
            <div class="flex items-center justify-center upper-voicedBy"> 
                <span class="txt-1">Voiced By</span>
                <span class="txt-2">Rakesh</span>
                <img class="raksh-img" src="../assets/rakesh.svg" alt="rakesh">
                <div class="lower-voicedBy"> 
                    <button>More Pranks with <b class="ml-1"> Rakesh </b><img src="../assets/arrow.svg"></button>
                </div>
            </div>
            <div class="follow-content"> 
                <span>Follow My Content</span>
                <div class="flex align-center justify-center"> 
                    <img src="../assets/utube1.svg">
                    <img src="../assets/fb1.svg">
                </div>
                <div class="flex align-center justify-center"> 
                    <img src="../assets/pin.svg">
                    <img src="../assets/tiktok.svg">
                </div>
            </div>
        </div>
    </div>
</template>
<style>
    .voicedBy-container {
        border-radius: 10px;
        flex-direction: column;
        position: relative;
        border-bottom-color: transparent;
    }
    .ml-1 {
        margin-left: 3px;
    }
    .desktop .upper-voicedBy {
        background: url("../assets/square.svg")!important;
        background-position: bottom;
        background-size: cover;
        min-height: 415px!important;
        background-repeat: no-repeat;
        padding: 30px;
        border-right: 1px solid rgba(47, 56, 78, 0.1);
        border-left: 1px solid rgba(47, 56, 78, 0.1);
    }
    .col-3 {
        padding-right: 0!important;
    }
    .col-3 .desktop {
        height: 100%;
    }
    .desktop .voicedBy-container {
        height: 100%;
    }
    .follow-content span {
        margin-top: 7.5px;
        margin-bottom: 10px;
        font-size: 21px;
        display: block;
        font-family: 'Montserrat-Bold';     
    }
    .follow-content .flex img {
        margin-right: 10px;
        margin-bottom: 14.5px;
    }
    .follow-content .flex img:last-child {
        margin-right: 0px;
    }
    .desktop .txt-1 {
        font-size: 14px;
        margin-top: -30px;
    }
    .desktop .txt-2 {
        font-size: 24px;
    }
    .raksh-img {
        min-width: 203px;
    }
    .voicedBy {
        padding: 20px;
    }
    .absolute {
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        bottom: -60px;
    }
    .mobile .lower-voicedBy {
        flex-direction: column;
        border: 1px solid rgba(47, 56, 78, 0.1);
        border-top-color: transparent;
        padding: 20px;
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
    }
    .follow-content {
        flex-direction: column;
        border: 1px solid rgba(47, 56, 78, 0.1);
        border-top-color: transparent;
        padding: 20px;
        border-bottom-left-radius: 10px;
        height: 100%;
        border-bottom-right-radius: 10px;
    }
    .lower-voicedBy span {
        font-family: Montserrat-Bold;
        margin-bottom: 16px;
        margin-top: 40px;
    }
    .mt-2 {
        margin-top: 35px;
    }
    .lower-voicedBy button {
        margin-top: 24px;
        background: linear-gradient(0deg, rgba(47, 219, 217, 0.1), rgba(47, 219, 217, 0.1)), #FFFFFF;
        border: 1px solid rgba(47, 56, 78, 0.1);
        box-sizing: border-box;
        border-radius: 10px;
        font-family: Montserrat!important;
        transition: .3s all ease-in;
    }
    .lower-voicedBy img {
        margin-left: 14px;
        margin-right:0px!important;
    }
    .upper-voicedBy {
        background: #2FDBD9;
        width:100%;
        border-radius: 10px;
        padding: 20px;
        flex-direction: column;
        min-height: 130px;
        border-bottom-left-radius: 0;
        border-bottom-right-radius: 0;
    }
    .img-1 {
        margin-right: 10px;
    }
    .txt-1 {
        color: #000;
        display: block;
        font-size: 12px;
        font-family: Montserrat-Bold;
    }
    .txt-2 {
        margin-top: 5px;
        color: #fff;
        display: block;
        font-size: 16px;
        font-family: Montserrat-Bold;
    }
</style>
