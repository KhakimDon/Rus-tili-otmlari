<script>
export default{
  methods:{
    sending(){
      let btn = document.querySelector(".send")
      let sendedtext = document.querySelector(".sended-text")
      btn.style.animationPlayState = 'running'
      sendedtext.classList.add("sended-text-activated")
    }
  }
}
</script>

<template>
  <main>
    <section class="one-screen">
      <div class="wrapper">
        <div class="left">
          <h1>
            ASSALOMU ALEYKUM !
            <br />
            <span> @Rossiya_OTMlari</span>
            telegram <br />
            kanalining rasmiy saytiga xush kelibsiz.
          </h1>
          <form @submit.prevent="sending()" action="#">
            <input placeholder="Ismingiz" class="txt" type="text" />
            <input placeholder="Telefon raqam" class="txt" type="text" />
            <div class="send-wp">
              <input class="send" value="Ariza qoldirish" type="submit" />
              <span class="sended-text">Arizangiz qabul qilindi. <br> Siz bilan tez orada ulanamiz.</span>
            </div> 
          </form>
        </div>
        <div class="right">
          <div class="logo-wrp">
            <img class="logo" src="../assets/logo-5000pix.png" alt="" />
          </div>
          <div class="blocks">
            <div class="items">
              <span>Onlayn <br> Konsultatsiya</span>
            </div>
            <div class="items">
              <span>O'qishga <br> kirish</span>
            </div>
            <div class="items">
              <span>Grant 2024</span>
            </div>
            <div class="items">
              <span>O'qishni <br> ko'chirish</span>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="second-screen"></section>
  </main>
</template>
