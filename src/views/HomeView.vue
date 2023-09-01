<script>
import Swiper from "../components/Swiper.vue"
export default {
  data(){
    return{
      info: [
        {
          id: 1,
          title: "Grant 2024",
          items: [
            {
              title: "Rossiyada oliy ta’lim",
              text: [
                `Rossiya OTMlari malakali ta’lim hamda talabalarga qulayliklar yaratib berish 
bo’yicha, dunyo reytinggida yuqori o’rinlarni egallab keladi. Bu yerda har bir 
talaba malakali mutaxasis bo’lib yetishishi uchun barcha sharoitlar yaratilgan.
`,
              ],
            },
            {
              title: "Qulayliklar  ",
              text: [
                `Yotoqxona`,
                "Stipendiya",
                "Bepul to’garaklar",
                "Sport",
                "Va boshqa qulayliklar",
              ],
            },
            {
              title: "Oliygohlar ro’yxat  ",
              text: [
                ` Московского государственного университета имени М.В.Ломоносова`,
                " Российский университет дружбы народов",
                "Российский экономический университет имени Г.В. Плеханова",
                "Национальный исследовательский технологический университет МИСИС",
                "РГУ нефти и газа (НИУ) имени И.М. Губкина",
                " Московский государственный строительный университет",
                "Первый Московский государственный медицинский университет имени И.М. Сеченова",
                "Московский государственный медико-стоматологический университетим.А.И.Евдокимова",
                "Московский авиационный институт",
                "Казанский федеральный университет",
                "Санкт-Петербургский государственный университет гражданской авиации",
                "Высшая школа экономики» (НИУ ВШЭ)",
                "Первый Санкт-Петербургский государственный медицинский университет имени академика И. П. Павлова",
              ],
            },
          ],
        },
        {
          id: 4,
          title: "O’qishga kirish",
          items: [
            {
              title: "Hujjatlar",
              text: [
                `Passport(ID karta)`,
                `Passport(ID karta) notarial tarjimasi `,
                `Attestat(Diplom, Shahodatnoma)`,
                `Attestat(Diplom, Shahodatnoma) notarial tarjima`,
                `3x4 rasm 6 dona `,
                `086-У tibbiy ma’lumotnoma`,
                `OITS bo’lmaganligi to’grisida tibbiy ma’lumotnoma `,
              ],
            },
            {
              title: "Universitetlar",
              text: [
                ` Московского государственного университета имени М.В.Ломоносова`,
                " Российский университет дружбы народов",
                "Российский экономический университет имени Г.В. Плеханова",
                "Национальный исследовательский технологический университет МИСИС",
                "РГУ нефти и газа (НИУ) имени И.М. Губкина",
                " Московский государственный строительный университет",
                "Первый Московский государственный медицинский университет имени И.М. Сеченова",
                "Московский государственный медико-стоматологический университетим.А.И.Евдокимова",
                "Московский авиационный институт",
                "Казанский федеральный университет",
                "Санкт-Петербургский государственный университет гражданской авиации",
                "Высшая школа экономики» (НИУ ВШЭ)",
                "Первый Санкт-Петербургский государственный медицинский университет имени академика И. П. Павлова",
              ],
            },
            {
              title: "O’qishni ko’chirish muddati:",
              text: [
                `Siz o’qishingizni yilda 2 marta yozda hamda qishda ko’chirib ketish huquqiga ega bo’lasiz, 
arizangiz ko’rib chiqlishi uchun 15-35 kungacha vaqt talab qilinadi hamda har bir talaba 
DTM test sinovidan o’tkazilib O’zbekiston OTMlariga qabul qilinad`,
              ],
            },
          ],
        },
        {
          id: 3,
          title: "O’qishni ko’chirish ",
          items: [
            {
              title: "O’qishni ko’chirish tartibi",
              text: [
                `Agar siz Rossiya universitetlarida kunduzgi kechki hamda sirtqi ta’limda o’qiydigan 
bo’lsangiz, o’qishingizni O’zbekistondagi davlat hamda nodavlat OTMlariga ko’chirish 
imkoniyatiga egasiz!`,
              ],
            },
            {
              title: "Kerakli hujjatlar ro’yxat",
              text: [
                `Passport`,
                `Akademik ma’lumotnoma(transkript)`,
                ` Talabalikni tasdiqlovchi oquv joyidan ma’lumotnoma`,
                `3x4 rasm`,
              ],
            },
            {
              title: "O’qishni ko’chirish muddati:",
              text: [
                `Siz o’qishingizni yilda 2 marta yozda hamda qishda ko’chirib ketish huquqiga ega bo’lasiz, 
arizangiz ko’rib chiqlishi uchun 15-35 kungacha vaqt talab qilinadi hamda har bir talaba 
DTM test sinovidan o’tkazilib O’zbekiston OTMlariga qabul qilinad`,
              ],
            },
          ],
        } ,
      ],
      ch  : [],
      yonalish: false,
      univers_menu: false,
      textSelect: "Yo`nalishni tanlang",
      otherSelect: false,
    }
  },
  methods: {
    close_infoblock(){
      let fourblocks = document.querySelector(".four-blocks")
      fourblocks.classList.remove("four-blocks-active")
      let fourblocks1 = document.querySelector(".four-blocks1")
      fourblocks1.classList.remove("four-blocks-active")
      let fourblocks2 = document.querySelector(".four-blocks2")
      fourblocks2.classList.remove("four-blocks-active")
      let fourblocks3 = document.querySelector(".four-blocks3")
      fourblocks3.classList.remove("four-blocks-active")
      
      let fourwrapper = document.querySelector(".four-wrapper")
      fourwrapper.classList.remove("four-wrapper-active")
        fourwrapper.classList.remove("four-wrapper-active-width")
      let fourwrapper1 = document.querySelector(".four-wrapper1")
      fourwrapper1.classList.remove("four-wrapper-active")
        fourwrapper1.classList.remove("four-wrapper-active-width")
      let fourwrapper2 = document.querySelector(".four-wrapper2")
      fourwrapper2.classList.remove("four-wrapper-active")
        fourwrapper2.classList.remove("four-wrapper-active-width")
      let fourwrapper3 = document.querySelector(".four-wrapper3")
      fourwrapper3.classList.remove("four-wrapper-active")
        fourwrapper3.classList.remove("four-wrapper-active-width")
    },
    fourblocks(){
      console.log(event.currentTarget.dataset.id);
      let fourblocks = document.querySelector(".four-blocks")
      fourblocks.classList.add("four-blocks-active")
      
      let fourwrapper = document.querySelector(".four-wrapper")
      console.log(fourwrapper);
      fourwrapper.classList.add("four-wrapper-active")
      setTimeout(() => {
        fourwrapper.classList.add("four-wrapper-active-width")
      }, 200);

    },
    fourblocks1(){
      console.log(event.currentTarget.dataset.id);
      let fourblocks = document.querySelector(".four-blocks1")
      fourblocks.classList.add("four-blocks-active")
      
      let fourwrapper = document.querySelector(".four-wrapper1")
      console.log(fourwrapper);
      fourwrapper.classList.add("four-wrapper-active")
      setTimeout(() => {
        fourwrapper.classList.add("four-wrapper-active-width")
      }, 200);

    },
    fourblocks2(){
      console.log(event.currentTarget.dataset.id);
      let fourblocks = document.querySelector(".four-blocks2")
      fourblocks.classList.add("four-blocks-active")
      
      let fourwrapper = document.querySelector(".four-wrapper2")
      console.log(fourwrapper);
      fourwrapper.classList.add("four-wrapper-active")
      setTimeout(() => {
        fourwrapper.classList.add("four-wrapper-active-width")
      }, 200);

    },
    fourblocks3(){
      console.log(event.currentTarget.dataset.id);
      let fourblocks = document.querySelector(".four-blocks3")
      fourblocks.classList.add("four-blocks-active")
      
      let fourwrapper = document.querySelector(".four-wrapper3")
      console.log(fourwrapper);
      fourwrapper.classList.add("four-wrapper-active")
      setTimeout(() => {
        fourwrapper.classList.add("four-wrapper-active-width")
      }, 200);

    },
    close(){
      let blocksitems= document.querySelectorAll(".blocks-items")
      let count = 0
      let int = setInterval(() => {
        blocksitems[count].classList.remove("rightactive")
        count++
        if(count == blocksitems.length){
          clearInterval(int)
        }
        }, 100);
      let menu = document.querySelector(".univers_menu")
      let univers_menu_inner_back = document.querySelector(".univers_menu_inner_back")
      if(this.univers_menu == true){

        univers_menu_inner_back.classList.remove("univers_menu_inner_back_active_height")
        setTimeout(() => {
          univers_menu_inner_back.classList.remove("univers_menu_inner_back_active_width")
        }, 300);

        menu.classList.remove("univers_menu_active")
        setTimeout(() => {
            menu.style.background = "transparent"
            menu.style.backdropFilter = "none"

        }, 0);
        this.univers_menu = false
      }
    },
    open_univers_popup(){
      let blocksitems= document.querySelectorAll(".blocks-items")
      let count = 0
      console.log();
      setTimeout(() => {
        let int = setInterval(() => {
        blocksitems[count].classList.add("rightactive")
        count++
        if(count == blocksitems.length){
          clearInterval(int)
        }
      }, 300);
      }, 1000);
      let menu = document.querySelector(".univers_menu")
      let univers_menu_inner_back = document.querySelector(".univers_menu_inner_back")
      if(this.univers_menu == false){

        univers_menu_inner_back.classList.add("univers_menu_inner_back_active_height")
        setTimeout(() => {
          univers_menu_inner_back.classList.add("univers_menu_inner_back_active_width")
        }, 300);

        menu.classList.add("univers_menu_active")
        setTimeout(() => {
            menu.style.background = "rgba(255, 255, 255, 0.454)"
            menu.style.backdropFilter = "blur(10px)"

        }, 1000);
        this.univers_menu = true
      }
    },
    sending() {
      let btn = document.querySelector(".send");
      let sendedtext = document.querySelector(".sended-text");
      btn.style.animationPlayState = "running";
      sendedtext.classList.add("sended-text-activated");
    },
    
    openFacultate(){
      if(event.currentTarget.dataset.opens == "false"){
        event.currentTarget.classList.add("itemsactive")
        event.currentTarget.dataset.opens = "true"
      }else{
        event.currentTarget.dataset.opens = "false"
        event.currentTarget.classList.remove("itemsactive")
      }
    },
    showAns(){
      
      let dates = document.querySelectorAll(".question")
      for(let i of dates){
        console.log(i);
        i.dataset.open = "false"
        i.style.height = 70 + 'px'
      }

      if(event.currentTarget.dataset.open == "false"){
        event.currentTarget.dataset.open = "true"
        event.currentTarget.style.height = (event.currentTarget.children[1].getBoundingClientRect().height + 100) + "px"

      }else if(event.currentTarget.dataset.open == "true"){
        event.currentTarget.dataset.open = "false"
        event.currentTarget.style.height = 70 + 'px'
      }
    },
    masking() {

    let e = event.target.value
    let e_last = e[e.length - 1].charCodeAt()

    if (e_last > 47 && e_last < 58) {
      let arr = e.split("");
    
      let mask = (i, num, simbol) => {
        i == num && arr[num] != simbol ? arr.splice(num, 0, simbol) : false;
      }
    
      for (let i = 0; i < arr.length; i++) {
        mask(i, 0, "+")
        mask(i, 4, " ")
        mask(i, 5, "(")
        mask(i, 8, ")")
        mask(i, 9, " ")
        mask(i, 13, " ")
        mask(i, 16, " ")
      }
    
      arr.length > 19 ? arr.pop() : false
      e = "";
      e = arr.join("");
    }
    else e = e.substr(0, e.length - 1)
    event.target.value = e

    let filtered = event.target.value.split("").filter(item => item.charCodeAt() > 47 && item.charCodeAt() < 58).join("")

    this.phoneNumber = filtered

    this.phoneNumber.length == 12 ? this.tel = true : this.tel = false

    },
    yonalishfunc(){
      console.log('asd');
      this.yonalish = !this.yonalish
      console.log(this.yonalish);
    },
    textselectt(){
      this.otherSelect = false
      this.textSelect = event.target.dataset.text
    },
    ohter(){
      this.otherSelect = true
      setTimeout(() => {
        document.querySelector(".otherother").focus()
      }, 100);
    }
    
  },
  mounted(){
  },
  components:{
    Swiper,
  }
};
</script>

<template>

<!-- 4 blocks  -->

  <div class="four-blocks">
    <div class="four-wrapper">
      <div class="four-wrapper-item" >
        <h2>Onlayn Konsultatsiya  <span @click="close_infoblock">&times;</span></h2>
        <form class="consult" action="#">
            <div class="inp">
              <span>Ism Familiya :</span>
              <input placeholder="Ivan Ivanov" type="text">
            </div>
            <div class="inp">
              <span>Telefon raqam :</span>
              <input @input="masking" value="+998" type="text">
            </div>
            <div>
              <span  >Qaysi yo'nalishda o`qimoqchisiz ?</span>
              <div @click="yonalishfunc()" class="select">
                <span> {{ this.textSelect }} </span>
                <ol :class="{activeyonalish: this.yonalish == true}">
                  <li data-text="Tibbiyot" @click="textselectt()">Tibbiyot</li>
                  <li data-text="Yuristpridensiya" @click="textselectt()">Yuristpridensiya</li>
                  <li data-text="Iqtisodiyot" @click="textselectt()">Iqtisodiyot</li>
                  <li data-text="Ta’lim" @click="textselectt()">Ta’lim</li>
                  <li data-text="Neft-Gaz" @click="textselectt()">Neft-Gaz</li>
                  <li data-text="Aviatsiya" @click="textselectt()">Aviatsiya</li>
                  <li data-text="Boshqa (yozish uchun joy)" @click="ohter">Boshqa</li>
                </ol>
              </div>
            </div>
            <input class="otherother" v-if="this.otherSelect" type="text"> <br v-if="this.otherSelect">
            <button>Ariza Qoldirish</button>
        </form>
      </div>
    </div>
  </div>
  <div class="four-blocks1">
    <div class="four-wrapper1">
      <div class="four-wrapper-item" >
        <h2>{{ this.info[1].title }}  <span @click="close_infoblock">&times;</span></h2>

        <div v-for="item of this.info[1].items" :key="item.id">
          <h3>{{item.title}}</h3>
          <ul v-for="item of item.text" :key="item.id">  
          <li> {{ item }} </li> 
        </ul> 
        </div>
        <form class="grantariza" action="#">
          <h3>Universitetlar haqida hamda yo’nalishlar va ulardagi kontrakt narxlar haqida ma’lumot
olmoqchi bo’lsangiz ariza qoldiring va biz siz bilan tez orada bog’lanamiz.</h3>
          <input placeholder="Ism" type="text">
          <input value="+998" @input="masking()" type="text">
          <button>Ariza qoldirish</button>
        </form>
      </div>
    </div>
  </div>
  <div class="four-blocks2">
    <div class="four-wrapper2">
      <div class="four-wrapper-item" >
        <h2>{{ this.info[0].title }} <span @click="close_infoblock">&times;</span></h2>

        <div v-for="item of this.info[0].items" :key="item.id">
          <h3>{{item.title}}</h3>
          <ul v-for="item of item.text" :key="item.id">  
          <li> {{ item }} </li> 
        </ul> 
        </div>
        <form class="grantariza" action="#">
          <h3>Grantda asosida talaba bo’lish uchun qo’shimcha ma’lumotlar olish uchun biz bilan bog’laning!</h3>
          <input placeholder="Ism" type="text">
          <input value="+998" @input="masking()" type="text">
          <button>Ariza qoldirish</button>
        </form>
      </div>
    </div>
  </div>
  <div class="four-blocks3">
    <div class="four-wrapper3">
      <div class="four-wrapper-item" >
        <h2>{{ this.info[2].title }}  <span @click="close_infoblock">&times;</span></h2>

        <div v-for="item of this.info[2].items" :key="item.id">
          <h3>{{item.title}}</h3>
          <ul v-for="item of item.text" :key="item.id">  
          <li> {{ item }} </li> 
        </ul> 
        </div>
        <form class="grantariza" action="#">
          <h3>O’qishni nodavlat hamda davlat OTMlariga ko’chirish borasida qo’shimcha ma’lumot olmoqchi bo’lsangiz biz bilan bo’glaning!</h3>
          <input placeholder="Ism" type="text">
          <input value="+998" @input="masking()" type="text">
          <button>Ariza qoldirish</button>
        </form>
      </div>
    </div>
  </div>




  <div class="univers_menu">
    <div class="univers_menu_inner_back"></div>
    <div class="univers_menu_inner">
      <h2>Rossiyanig eng nufuzli universitetlari.🎓 <span @click="close">&times;</span></h2>
      <div>
        <div data-opens="false" @click="openFacultate" class="items blocks-items">
            <div class="top">
              <h3>1. M. V. Lomonosov nomidagi Moskva davlat universiteti</h3>
              <h3>Fakultetlar:</h3>

            </div>
            <div class="bottom">
              <figure></figure>
              <ul>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
              </ul>
            </div>
        </div>
        <div data-opens="false" @click="openFacultate" class="items blocks-items">
            <div class="top">
              <h3>1. M. V. Lomonosov nomidagi Moskva davlat universiteti</h3>
              <h3>Fakultetlar:</h3>

            </div>
            <div class="bottom">
              <figure></figure>
              <ul>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
              </ul>
            </div>
        </div>
        <div data-opens="false" @click="openFacultate" class="items blocks-items">
            <div class="top">
              <h3>1. M. V. Lomonosov nomidagi Moskva davlat universiteti</h3>
              <h3>Fakultetlar:</h3>

            </div>
            <div class="bottom">
              <figure></figure>
              <ul>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
              </ul>
            </div>
        </div>
        <div data-opens="false" @click="openFacultate" class="items blocks-items">
            <div class="top">
              <h3>1. M. V. Lomonosov nomidagi Moskva davlat universiteti</h3>
              <h3>Fakultetlar:</h3>

            </div>
            <div class="bottom">
              <figure></figure>
              <ul>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
                <li>Metalurgiya</li>
                <li>Formatevtika</li>
                <li>Mashinasozlik</li>
                <li>Texnik</li>
                <li>Elktrotarmoqlar</li>
                <li>Buxgalteriya</li>
              </ul>
            </div>
        </div>
        
      </div>
    </div>
  </div>




  <main>
    <section class="one-screen">
      <figure class="mobile-logo">
        <img src="../assets/logo-5000pix.png" alt="" />
      </figure>
      <div class="wrapper">
        <div class="left">
          <h1>
            ASSALOMU ALEYKUM !
            <br />
            <span class="font-[600]"> @Rossiya_OTMlari</span>
            telegram <br />
            kanalining rasmiy saytiga xush kelibsiz.
          </h1>
          <form @submit.prevent="sending()" action="#">
            <input required placeholder="Ismingiz" class="txt" type="text" />
            <input @input="masking" value="+998" required placeholder="Telefon raqam" class="txt" type="text" />
            <div class="send-wp">
              <input class="send" value="Ariza qoldirish" type="submit" />
              <span class="sended-text">Arizangiz qabul qilindi. <br />
                Siz bilan tez orada ulanamiz.</span>
            </div>
          </form>
        </div>
        <div class="right">
          <div class="logo-wrp">
            <img class="logo" src="../assets/logo-5000pix.png" alt="" />
          </div>
          <div class="blocks">
            <div @click="fourblocks()" data-id="1" class="items">
              <span>Onlayn <br />
                Konsultatsiya
                <img class="mouse" src="../assets/klick-click.gif" alt="asd">
              </span>
                
            </div>
            <div @click="fourblocks1()" data-id="2" class="items">
              <span>O'qishga <br />
                kirish</span>
            </div>
            <div @click="fourblocks2()" data-id="3"  class="items">
              <span>Grant 2024</span>
            </div>
            <div @click="fourblocks3()" data-id="4" class="items">
              <span>O'qishni <br />
                ko'chirish</span>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="second-screen">
      <div class="wrapper">
        <div class="left">
          <h1>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M9.813 15.904L9 18.75l-.813-2.846a4.5 4.5 0 00-3.09-3.09L2.25 12l2.846-.813a4.5 4.5 0 003.09-3.09L9 5.25l.813 2.846a4.5 4.5 0 003.09 3.09L15.75 12l-2.846.813a4.5 4.5 0 00-3.09 3.09zM18.259 8.715L18 9.75l-.259-1.035a3.375 3.375 0 00-2.455-2.456L14.25 6l1.036-.259a3.375 3.375 0 002.455-2.456L18 2.25l.259 1.035a3.375 3.375 0 002.456 2.456L21.75 6l-1.035.259a3.375 3.375 0 00-2.456 2.456zM16.894 20.567L16.5 21.75l-.394-1.183a2.25 2.25 0 00-1.423-1.423L13.5 18.75l1.183-.394a2.25 2.25 0 001.423-1.423l.394-1.183.394 1.183a2.25 2.25 0 001.423 1.423l1.183.394-1.183.394a2.25 2.25 0 00-1.423 1.423z" />
            </svg>
            Nega aynan biz ?
          </h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga aut
            nemo quidem? Repellendus quos nemo, laudantium sint aut tempore
            placeat impedit commodi, distinctio error laboriosam odio cupiditate
            vel repudiandae corporis odit!
            <span>
              Commodi animi blanditiis quibusdam amet nihil unde officiis libero
              culpa eos </span>consequuntur rem ullam excepturi id dolor quidem iusto fugiat quos
            tempore, illum dolorem officia dolore recusandae sint. Rerum magni
            quaerat necessitatibus illum aut dignissimos soluta obcaecati
            explicabo molestias animi! Voluptatem adipisci sed, dicta aperiam,
            deleniti animi cum similique exercitationem sequi voluptate commodi
            neque error necessitatibus vitae. Cum tempore voluptatum expedita?
            <br />
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z" />
            </svg>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z" />
            </svg>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M11.48 3.499a.562.562 0 011.04 0l2.125 5.111a.563.563 0 00.475.345l5.518.442c.499.04.701.663.321.988l-4.204 3.602a.563.563 0 00-.182.557l1.285 5.385a.562.562 0 01-.84.61l-4.725-2.885a.563.563 0 00-.586 0L6.982 20.54a.562.562 0 01-.84-.61l1.285-5.386a.562.562 0 00-.182-.557l-4.204-3.602a.563.563 0 01.321-.988l5.518-.442a.563.563 0 00.475-.345L11.48 3.5z" />
            </svg>
          </p>
          <div></div>
        </div>
        <div class="right">
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
              stroke="currentColor" class="w-6 h-6">
              <path stroke-linecap="round" stroke-linejoin="round"
                d="M15.59 14.37a6 6 0 01-5.84 7.38v-4.8m5.84-2.58a14.98 14.98 0 006.16-12.12A14.98 14.98 0 009.631 8.41m5.96 5.96a14.926 14.926 0 01-5.841 2.58m-.119-8.54a6 6 0 00-7.381 5.84h4.8m2.581-5.84a14.927 14.927 0 00-2.58 5.84m2.699 2.7c-.103.021-.207.041-.311.06a15.09 15.09 0 01-2.448-2.448 14.9 14.9 0 01.06-.312m-2.24 2.39a4.493 4.493 0 00-1.757 4.306 4.493 4.493 0 004.306-1.758M16.5 9a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0z" />
            </svg>
            FAST
          </div>
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" d="M15.042 21.672L13.684 16.6m0 0l-2.51 2.225.569-9.47 5.227 7.917-3.286-.672zm-7.518-.267A8.25 8.25 0 1120.25 10.5M8.288 14.212A5.25 5.25 0 1117.25 10.5" />
            </svg>
            Correct

          </div>
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M15.75 17.25v3.375c0 .621-.504 1.125-1.125 1.125h-9.75a1.125 1.125 0 01-1.125-1.125V7.875c0-.621.504-1.125 1.125-1.125H6.75a9.06 9.06 0 011.5.124m7.5 10.376h3.375c.621 0 1.125-.504 1.125-1.125V11.25c0-4.46-3.243-8.161-7.5-8.876a9.06 9.06 0 00-1.5-.124H9.375c-.621 0-1.125.504-1.125 1.125v3.5m7.5 10.375H9.375a1.125 1.125 0 01-1.125-1.125v-9.25m12 6.625v-1.875a3.375 3.375 0 00-3.375-3.375h-1.5a1.125 1.125 0 01-1.125-1.125v-1.5a3.375 3.375 0 00-3.375-3.375H9.75" />
</svg>
document
          </div>
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 18.75a60.07 60.07 0 0115.797 2.101c.727.198 1.453-.342 1.453-1.096V18.75M3.75 4.5v.75A.75.75 0 013 6h-.75m0 0v-.375c0-.621.504-1.125 1.125-1.125H20.25M2.25 6v9m18-10.5v.75c0 .414.336.75.75.75h.75m-1.5-1.5h.375c.621 0 1.125.504 1.125 1.125v9.75c0 .621-.504 1.125-1.125 1.125h-.375m1.5-1.5H21a.75.75 0 00-.75.75v.75m0 0H3.75m0 0h-.375a1.125 1.125 0 01-1.125-1.125V15m1.5 1.5v-.75A.75.75 0 003 15h-.75M15 10.5a3 3 0 11-6 0 3 3 0 016 0zm3 0h.008v.008H18V10.5zm-12 0h.008v.008H6V10.5z" />
</svg>
economy
          </div>
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M6.429 9.75L2.25 12l4.179 2.25m0-4.5l5.571 3 5.571-3m-11.142 0L2.25 7.5 12 2.25l9.75 5.25-4.179 2.25m0 0L21.75 12l-4.179 2.25m0 0l4.179 2.25L12 21.75 2.25 16.5l4.179-2.25m11.142 0l-5.571 3-5.571-3" />
</svg>
materials

          </div>
          <div class="block">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M6.633 10.5c.806 0 1.533-.446 2.031-1.08a9.041 9.041 0 012.861-2.4c.723-.384 1.35-.956 1.653-1.715a4.498 4.498 0 00.322-1.672V3a.75.75 0 01.75-.75A2.25 2.25 0 0116.5 4.5c0 1.152-.26 2.243-.723 3.218-.266.558.107 1.282.725 1.282h3.126c1.026 0 1.945.694 2.054 1.715.045.422.068.85.068 1.285a11.95 11.95 0 01-2.649 7.521c-.388.482-.987.729-1.605.729H13.48c-.483 0-.964-.078-1.423-.23l-3.114-1.04a4.501 4.501 0 00-1.423-.23H5.904M14.25 9h2.25M5.904 18.75c.083.205.173.405.27.602.197.4-.078.898-.523.898h-.908c-.889 0-1.713-.518-1.972-1.368a12 12 0 01-.521-3.507c0-1.553.295-3.036.831-4.398C3.387 10.203 4.167 9.75 5 9.75h1.053c.472 0 .745.556.5.96a8.958 8.958 0 00-1.302 4.665c0 1.194.232 2.333.654 3.375z" />
</svg>
feedbacks
          </div>
        </div>
      </div>
    </section>
    <section class="slider-wrapper">
      <Swiper @openmodal="open_univers_popup"/>
    </section>

    <section class="questions">

      <h2>Ko`p  so`raladigan savollar :</h2>
      <div class="wrapper">
        <div class="left">
          <img src="../assets/logo-5000pix.png" alt="">
          <h2>Telegram kanalimizga a`zo bo`ling va barcha yangilioklardan xabardor bo`ling !</h2>
          <a href="https://t.me/Rossiya_OTMlari"><button>Kanalga a'zo bo`lish</button></a>
          
        </div>
        <div class="right">
          <div style="height: 200px;" data-open="true" @click="showAns()" class="question">
            <span>Nechta universitet mavjud ? 🤔</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, aliquid, officia, quos perspiciatis pariatur dolor quasi.</p>
          </div>
          <div data-open="false" @click="showAns()" class="question">
            <span>O'qishga borish nechpul ? 💵</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, aliquid, officia, quos perspiciatis pariatur dolor quasi. Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque, deserunt.</p>
          </div>
          <div data-open="false" @click="showAns()" class="question">
            <span>Kontrakni bo'lib to'lasa bo'ladimi ? 🏦</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, aliquid, officia, quos perspiciatis pariatur dolor quasi. Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque, deserunt.</p>
          </div>
          <div data-open="false" @click="showAns()" class="question">
            <span>Qanaqa dokumentlar kerak ? 📄</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, aliquid, officia, quos perspiciatis pariatur dolor quasi. Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque, deserunt.</p>
          </div>
          <div data-open="false" @click="showAns()" class="question">
            <span>Garantiya bormi ? 💯</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Commodi, aliquid, officia, quos perspiciatis pariatur dolor quasi. Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque, deserunt.</p>
          </div>
        </div>
      </div>

    </section>

  </main>
  <footer>
    <div class="wrapper">
      <div>
        <img src="../assets/logo-5000pix.png" alt="">
      </div>
      <ul>
        <li><a href="#">Socials :</a></li>
        <li><a href="">Telegram<img src="../assets/tg.png" alt=""></a></li>
        <li><a href="https://youtube.com/@Rossiya_OTMlari?si=UitUdv4G3U8of-9-">You tube<img src="../assets/inst.png" alt=""></a></li>
      </ul>
      <ul>
        <li><a href="">Contacts :</a></li>
        <li><a href="tel:+998915491754">
          <svg height="20" xmlns="http://www.w3.org/2000/svg" class="ionicon" viewBox="0 0 512 512"><path d="M451 374c-15.88-16-54.34-39.35-73-48.76-24.3-12.24-26.3-13.24-45.4.95-12.74 9.47-21.21 17.93-36.12 14.75s-47.31-21.11-75.68-49.39-47.34-61.62-50.53-76.48 5.41-23.23 14.79-36c13.22-18 12.22-21 .92-45.3-8.81-18.9-32.84-57-48.9-72.8C119.9 44 119.9 47 108.83 51.6A160.15 160.15 0 0083 65.37C67 76 58.12 84.83 51.91 98.1s-9 44.38 23.07 102.64 54.57 88.05 101.14 134.49S258.5 406.64 310.85 436c64.76 36.27 89.6 29.2 102.91 23s22.18-15 32.83-31a159.09 159.09 0 0013.8-25.8C465 391.17 468 391.17 451 374z" fill="black" stroke="currentColor" stroke-miterlimit="10" stroke-width="32"/></svg>+998 (91) 549-17-54</a></li>
        <li><a href="tel:+7 966 865 2020">
          <svg height="20" xmlns="http://www.w3.org/2000/svg" class="ionicon" viewBox="0 0 512 512"><path d="M451 374c-15.88-16-54.34-39.35-73-48.76-24.3-12.24-26.3-13.24-45.4.95-12.74 9.47-21.21 17.93-36.12 14.75s-47.31-21.11-75.68-49.39-47.34-61.62-50.53-76.48 5.41-23.23 14.79-36c13.22-18 12.22-21 .92-45.3-8.81-18.9-32.84-57-48.9-72.8C119.9 44 119.9 47 108.83 51.6A160.15 160.15 0 0083 65.37C67 76 58.12 84.83 51.91 98.1s-9 44.38 23.07 102.64 54.57 88.05 101.14 134.49S258.5 406.64 310.85 436c64.76 36.27 89.6 29.2 102.91 23s22.18-15 32.83-31a159.09 159.09 0 0013.8-25.8C465 391.17 468 391.17 451 374z" fill="black" stroke="currentColor" stroke-miterlimit="10" stroke-width="32"/></svg>+7 966 865 2020</a></li>
      </ul>
      <ul>
        <li><a href="">Bepul darsliklar : </a></li>
        <li><a href="https://t.me/Rossiya_OTMlari_admin">👉 Rus tilidan darslik</a></li>
        <li style="opacity:0; pointer-events: none;"><a href="">Contacts</a></li>
      </ul>
      
    </div>
  </footer>
</template>
<style>

</style>
