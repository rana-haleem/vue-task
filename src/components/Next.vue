<template>
    <div class="next-container">
        <div class="flex next-title"> 
            <span>Next</span>
            <div class="flex items-center autoplay"> 
                <span>AUTOPLAY</span>
                <img src="../assets/enable.svg">
            </div>
        </div>
        <swiper
            :slides-per-view="1.2"
            :breakpoints="swiperOptions.breakpoints"
            @swiper="onSwiper"
            @slideChange="onSlideChange"
        >
              <swiper-slide>
                <div class="flex swiper-next-container"> 
                    <img src="../assets/nxt1.svg">
                    <div class="flex nxt-text"> 
                        <span>City Waste</span>
                        <div class="flex items-center views">
                            <img src="../assets/view.svg">
                            <span>11,675</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
                  <swiper-slide>
                <div class="flex swiper-next-container"> 
                    <img src="../assets/nxt1.svg">
                    <div class="flex nxt-text"> 
                        <span>City Waste</span>
                        <div class="flex items-center views">
                            <img src="../assets/view.svg">
                            <span>11,675</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div class="flex swiper-next-container"> 
                    <img src="../assets/nxt1.svg">
                    <div class="flex nxt-text"> 
                        <span>Raki Wifi Thief</span>
                        <div class="flex items-center views">
                            <img src="../assets/view.svg">
                            <span>3,675</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
            <swiper-slide>
                <div class="flex swiper-next-container"> 
                    <img src="../assets/nxt1.svg">
                    <div class="flex nxt-text"> 
                        <span>City Waste</span>
                        <div class="flex items-center views">
                            <img src="../assets/view.svg">
                            <span>11,675</span>
                        </div>
                    </div>
                </div>
            </swiper-slide>
        </swiper>
    </div>
</template>
<script>
 import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
 
  export default {
    data () {
      return { // Retourn the API Dates
        swiperOptions: {
            breakpoints: {       
                320: {       
                    slidesPerView: 1.2,
                    spaceBetween: 15     
                },          
                768: {       
                    slidesPerView: 2,       
                    spaceBetween: 50     
                },   
            
                1200: {       
                    slidesPerView: 4,       
                    spaceBetween: 30     
                } 
            }   
        }
      }
    },
    components: {
      Swiper,
      SwiperSlide,
    },
    methods: {
      onSwiper(swiper) {
        console.log(swiper);
      },
      onSlideChange() {
        console.log('slide change');
      },
    },
  };
</script>
<style>
    .next-container {
        padding:15px 20px;
        background: rgba(0, 0, 0, 0.02);
        box-shadow: inset 0px -1px 0px rgba(0, 0, 0, 0.05);
    }
    .swiper-next-container {
        background: #FFFFFF;
        box-shadow: 0px 2px 6px rgba(0, 0, 0, 0.05);
        border-radius: 8px;
        width:100%;
        cursor: pointer;
    }
    .swiper-next-container img {
        border-top-left-radius: 8px;
        border-bottom-left-radius: 8px;
    }
    .swiper-slide {
        min-width: 265px!important;
    }
    .nxt-text span {
        font-family: Montserrat;
        font-weight: 600;
        font-size: 13px;
        line-height: 16px;
        color: #393A3A;
    }
    .next-title {
        margin-bottom: 20px;
    }
    .views img {
        margin-right: 8px;
    }
    .views span {
        font-weight: 600;
        font-size: 11px;
        line-height: 13px;
        color: #ACB2C1;
        margin-top: 1px;
    }
    .next-container .next-title {
        justify-content: space-between;
    }
    .next-title span {
         font-family: Montserrat-Bold;
         font-size: 18px;
    }
    .autoplay span {
        font-size: 12px;
        color: #393A3A;
        margin-bottom: 0px!important;
        margin-right: 10px;
    }
    .nxt-text {
        flex-direction: column;
        align-items: start;
        padding: 10px 12px;
        width: 100%;
        justify-content: space-between;
        transition: .3s all ease-in;
    }
    @media(min-width: 1200px){
        .next-container {
            padding:15px 65px;
        }   
        .swiper-next-container:hover .nxt-text {
            background: #0dcaf02e;
            transition: .3s all ease-in;
            border-radius: 8px;
        }
    }
</style>
