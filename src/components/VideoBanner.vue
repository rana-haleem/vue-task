<template>
    <div class="mobile">
        <video poster="../assets/Video.svg">
            <source src="https://www.youtube.com/watch?v=WVRBzHgvneU&t=3s" type="video/mp4">
        </video>
         <div class="flex buttons-container"> 
            <button><img src="../assets/view.svg">3,678</button>
            <button><img src="../assets/download.svg">Download</button>
            <button><img src="../assets/share.svg">Share</button>
        </div>
        <span class="mobile banner-text">The most annoying customer ever orders a pizza. See how fast you can get them to rage!</span>
    </div>
    <div class="desktop">
        <div class="container-fluid"> 
            <div class="row">
                <div class="col-9"> 
                    <video poster="../assets/vid-dsk.svg">
                        <source src="https://www.youtube.com/watch?v=WVRBzHgvneU&t=3s" type="video/mp4">
                    </video>
                    <div class="banner-text-desktop flex items-center"> 
                        <span>Rakesh Boiling Point Pizza Order</span>
                        <div class="flex buttons-container justify-center"> 
                            <button><img src="../assets/view.svg">3,678</button>
                            <button><img src="../assets/download.svg">Download</button>
                            <button><img src="../assets/share.svg">Share</button>
                        </div>
                    </div>
                     <span class="video-text">The most annoying customer ever orders a pizza. See how fast you can get them to rage!</span>
                </div> 
                <div class="col-3"> 
                    <VoicedBy/>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    import VoicedBy from '@/components/VoicedBy.vue'
    export default {
        components: {
            VoicedBy
        }
    }
</script>
<style>
    video {
        width: 100%;
    }
    button {
        background: #FFFFFF;
        border: 1px solid rgba(47, 56, 78, 0.1);
        border-radius: 10px;
        padding: 12px 10px;
        margin-right: 12px;
        font-size: 12px;
        font-family: Montserrat-Bold;
        transition: .3s all ease-in;
    }
    .banner-text {
        color: #393A3A;
        font-size: 12px;
        padding: 0px 20px;
        text-align: left;
    }
    .banner-text-desktop {
        justify-content: space-between;
    }
    .banner-text-desktop span {
        font-family: Montserrat-Bold;
        font-size: 24px;
    }
    .video-text {
        font-size: 16px;
        text-align: left;
        width: 50%;
        color: #393A3A;
        display: block;
        line-height: 19.5px;
    }
    .banner-text-desktop .buttons-container {
        padding-right: 0;
    }
    .mobile .buttons-container {
        justify-content: space-between;
    }
    button:last-child {
        margin-right: 0!important;    
    }
    .buttons-container button:first-child {
        font-family: Montserrat;
        color: #ACB2C1;
    }
    .flex button {
        margin-right: 5px;
    }
    .buttons-container {
        padding: 12px 20px;
    }
    button img {
        margin-right: 10px;
    }
    @media (min-width:375px) {
        button {
            padding: 12px 16px; 
        }
        .flex button {
            margin-right: 10px;
        }
    }
    @media (min-width:375px) {
        .buttons-container button:hover {
            background: #0dcaf026;
            transition: .3s all ease-in;
        }
    }
</style>
