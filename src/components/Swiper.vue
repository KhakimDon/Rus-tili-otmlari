<template>
    <swiper :pagination="{
        type: 'fraction',
    }" :navigation="true" :modules="modules" class="mySwiper">
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>Rossiya xalqlar do'stligi universiteti</h2>
                <p>
                    KPSS Markaziy komiteti va SSSR Ministrlar Sovetining 1960 — yil 5-fevraldagi qarori bilan xalqlar do'stligi universiteti sifatida ta'sis etilgan, 1961-yil 22-fevralda Patris Lumumba nomi bilan atalgan, 1992-yil 5-fevraldan Rossiya xalqlar do'stligi universiteti.
                </p>
                <button class="btnbtnbtn" @click="emits()">Barcha Universitetlar</button>
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>G.V.Plexanov nomidagi Rossiya <br> iqtisodiyot universiteti</h2>
                <p>
                    1907 yilda tadbirkor Aleksey Vishnyakov tomonidan Rossiya imperiyasida tijorat ta'limini tarqatish bo'yicha birinchi ixtisoslashtirilgan oliy o'quv yurti sifatida tashkil etilgan. Bugungi kunda bu iqtisodiyot, tovarshunoslik va texnologiya sohasida yuqori malakali mutaxassislarni tayyorlash bo'yicha eng yirik o'quv va ilmiy markazdir.
                </p>
                <button class="btnbtnbtn" @click="emits()">Barcha Universitetlar</button>   
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>M.V.Lomonosov nomidagi <br> Moskva davlat universiteti</h2>
                <p>
                    1940 yildan Mixail Vasilievich Lomonosov nomini olgan. To'liq nomi - "M. V. Lomonosov nomidagi Moskva davlat universiteti"federal davlat byudjet oliy ta'lim muassasasi.
                </p>
                <button class="btnbtnbtn" @click="emits()">Barcha Universitetlar</button>   
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="rotate-block"></div>
            <div class="content">
                <h2>I. M. Gubkin nomidagi <br> neft va gaz RGU (NIU) </h2>
                <p>
                    1930 yilda tashkil etilgan, 1945 yilda mehnat qizil bayrog'i ordeni, 1980 yilda oktyabr inqilobi ordeni, 2000 yilda Vetnam Sotsialistik Respublikasi xalqlari do'stligi ordeni, 2010 yilda Vetnam Sotsialistik Respublikasining III darajali mehnat ordeni, 2017 yilda <b>O'zbekiston Respublikasi</b> Do'stlik ordeni bilan mukofotlangan.
                </p>
                <button class="btnbtnbtn" @click="emits()">Barcha Universitetlar</button>   
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
    methods:{
        emits(){
            this.$emit("openmodal")
        }
    },
    setup() {
        return {
            modules: [Pagination, Navigation],
        };
    },
};
</script>
  

<style>
.btnbtnbtn{
    width: max-content !important;
    padding: 0px 13px;
}
</style>