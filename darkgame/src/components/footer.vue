<template>
<div>
<div class="footer">
      <img src="../assets/footer.png" />
      <div class="name_footer">
        <span id="foot_1">DARKGAME</span><br /><span id="foot_2"
          >ИГРОВОЙ КЛУБ</span
        >
      </div>
      <span id="adress">г.Тула, ул.Республики д.49</span>
      <img id="map" src="../assets/map.png" />
      <div class="information">
        <img id="vk" src="../assets/vk.svg" />
        <a id="vk_span">darkgame_tula</a>
        <img id="instagram" src="../assets/insta.svg" />
        <a id="insta_span">darkgame_tula</a>
        <span id="nomer_span">Контактный номер телефона</span>
        <span id="tel">+7(929)123-21-32</span>
      </div>
      <span id="copirating">© 2024 DARKGAME</span>
    </div>
</div>
</template>


<style scoped>
.footer {
  position: relative;
  width: 100%;
}

.name_footer {
  position: absolute;
  left: 3.5%;
  top: 13%;
  font-size: 24px;
  font-family: "Roboto" sans-serif;
  font-weight: bold;
  line-height: 27px;
}

#foot_1 {
  color: #ffffff;
}
#foot_2 {
  font-size: 20px;
  color: #7e7e7e;
}

#adress {
  position: absolute;
  width: 13%;
  left: 3%;
  font-family: "Roboto" sans-serif;
  top: 65%;
  color: #a4a4a4;
}
#map {
  position: absolute;
  top: 5%;
  left: 20.5%;
}
#vk {
  position: absolute;
  top: 14%;
  left: 68%;
}
#vk_span {
  position: absolute;
  width: 5.5%;
  height: 1.5%;
  top: 16%;
  left: 71%;

  color: #bbbbbb;
}
#instagram {
  position: absolute;
  top: 36.5%;
  left: 68%;
}
#insta_span {
  position: absolute;
  width: 5.5%;
  height: 1.5%;
  top: 38.5%;
  left: 71%;

  color: #bbbbbb;
}
#nomer_span{
  position: absolute;
  color: #ffffff;
  top: 19%;
  left: 81%;
}
#tel{
  position: absolute;
  top: 32%;
  left: 81%;
  font-size: 28px;

  color: #ffffff;
}
#copirating{
  position: absolute;
  right: 1%;
  top: 85%;
  color: #707070;
}

@media screen and (max-width: 1290px) {
    .name_footer{
    font-size: 18px;
  }
  #adress{
    font-size: 16p;
  }
  #map{
    width: 40%;
    top: 12.5%;
    left: 22.5%;
  }
  #vk{
    width: 20px;
    height: 20px;
  }
  #instagram{
    width: 20px;
    height: 20px;
  }
  #vk_span{
    font-size: 12px;
  }
  #insta_span{
    font-size: 12px;
  }
  #nomer_span{
    font-size: 13.8px;
  }
  #tel{
    font-size: 18px;
  }
  #copirating{
    font-size: 14px;
  }
  #foot_2{
    font-size: 16px;
  }
}

@media screen and (min-width: 901px) {
}

@media screen and (max-width: 900px) {
    #vk{
    width: 16px;
    height: 16px;
  }
  #vk_span{
    font-size: 10px;
  }
  #instagram{
    width: 16px;
    height: 16px;
    top: 30%;
  }
  #insta_span{
    font-size: 10px;
    top: 30%;
  }
  #nomer_span{
    top: 50%;
    left: 68%;
    font-size: 12px;
  }
  #tel{
    font-size: 12px;
    top: 62%;
    left: 68%;
  }
  .name_footer{
    width: 18%;
    word-wrap: break-word;
    font-size: 16px;
  }
  #foot_2{
    font-size: 12px;
  }
}

@media screen and (min-width: 591px) {
}

@media screen and (max-width: 590px) {
    .name_footer{
    font-size: 12px;
  }
  #foot_2{
    font-size: 10px;
  }
  #adress{
    width: 20%;
    font-size: 12px;
  }
  #vk_span{
    left: 73%;
  }
  #insta_span{
    top: 32%;
    left: 73%;
  }
  #nomer_span{
    top: 55%;
    left: 30%;
  }
  #tel{
    top: 67%;
    left: 41%;

  }
}

@media screen and (min-width: 431px) {
}

@media screen and (max-width: 430px) {
     #name_footer{
    font-size: 10px;
  }
  #foot_2{
    font-size: 8px;
  }
  #adress{
    top: 85%;
    width: 90%;
    font-size: 10px;
  }
}
</style>