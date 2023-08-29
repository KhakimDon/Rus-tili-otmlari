<template>
    <swiper :pagination="{
        type: 'fraction',
    }" :navigation="true" :modules="modules" class="mySwiper">
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>Moskva davlat M. V. Lomonosov <br> nomidagi Universitet  </h2>
                <p>
                    Rossiyaning eng qadimgi va eng yirik klassik universitetlaridan biri, Moskvada joylashgan Rossiya fan va madaniyati markazlaridan biri. 1940 yildan Mixail Vasilievich Lomonosov nomini olgan
                </p>
                <button>Batafsil</button>
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>Lorem ipsum dolor sit Lorem, <br> ipsum dolor</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem distinctio amet culpa voluptate, fuga iure? Tempore sunt animi sed saepe et, dicta magni beatae veniam corporis sit ipsam eos soluta eveniet consectetur inventore? Minima ipsa quidem, assumenda veniam asperiores numquam.
                </p>
                <button>click this</button>
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>Lorem ipsum dolor sit Lorem,<br>  ipsum dolor</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem distinctio amet culpa voluptate, fuga iure? Tempore sunt animi sed saepe et, dicta magni beatae veniam corporis sit ipsam eos soluta eveniet consectetur inventore? Minima ipsa quidem, assumenda veniam asperiores numquam.
                </p>
                <button>click this</button>
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>Lorem ipsum dolor sit Lorem, <br> ipsum dolor</h2>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Autem distinctio amet culpa voluptate, fuga iure? Tempore sunt animi sed saepe et, dicta magni beatae veniam corporis sit ipsam eos soluta eveniet consectetur inventore? Minima ipsa quidem, assumenda veniam asperiores numquam.
                </p>
                <button>click this</button>
            </div>
        </swiper-slide>
    </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';
import 'swiper/css/navigation';

import '../assets/swiper.css';

// import required modules
import { Pagination, Navigation } from 'swiper/modules';

export default {
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
        return {
            modules: [Pagination, Navigation],
        };
    },
};
</script>
  