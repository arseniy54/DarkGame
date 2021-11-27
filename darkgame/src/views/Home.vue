<template>
  <div>
    <div class="first_screen">
      <div class="header_bar">
        <a href="" id="advantages">Преимущества</a>
        <a href="" id="periphery">Переферия</a>
        <a href="" id="news">Новости</a>
        <a href="" id="contact">Контакты</a>
      </div>
      <img id="setting" src="../assets/setting.svg" />
      <img src="../assets/fon.png" />
      <img id="logo" src="../assets/logo.svg" />
      <div class="slang">
        <span id="slang_1">Игры для тех</span>
        <br />
        <span id="slang_2">Кому важна</span>
        <br />
        <span id="slang_3">Производительность</span>
      </div>
    </div>
    <div class="second_screen">
      <img src="../assets/fon_second.png" />
      <span id="name_space">ТОПОВОЕ ИГРОВОЕ ПРОСТРАНСТВО ДЛЯ ВСЕХ</span>
      <div class="advantage">
        <img id="rhomb" class="rhomb" src="../assets/rhomb.svg" />
        <span id="game">Загрузка твоих любимых игр</span>
        <img id="rhomb_1" class="rhomb" src="../assets/rhomb.svg" />
        <span id="efficiency">Высокая производительность станций</span>
        <img id="rhomb_2" class="rhomb" src="../assets/rhomb.svg" />
        <span id="time">Почасовые тарифы</span>
        <img id="rhomb_3" class="rhomb" src="../assets/rhomb.svg" />
        <span id="cafeteria">Кафетерий</span>
        <img id="rhomb_4" class="rhomb" src="../assets/rhomb.svg" />
        <span id="atmosphere"
          >Приятная атмосфера в современном игровом интерьере</span
        >
        <img id="rhomb_5" class="rhomb" src="../assets/rhomb.svg" />
        <span id="wifi">Бесплатный WIFI для клиентов</span>
      </div>
    </div>
    <div class="third_screen">
      <img src="../assets/fon_third.png" />
      <span id="name_iron">ИГРОВОЕ ЖЕЛЕЗО</span>
      <div class="block_rooms">
        <img
          id="ordinary_room"
          src="../assets/ordinary_room.png"
          @click="vip"
        />
        <div class="price_ordinary"><span>59₽ час</span></div>
        <img id="vip_room" src="../assets/vip_room.png" />
        <div class="price_vip"><span>149₽ час</span></div>
        <img id="console_room" src="../assets/console_room.png" />
        <div class="price_console"><span>149₽ час</span></div>
      </div>
      <div class="description">
        <!--<span id="name_room"> {{ name }}</span>-->
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />
        <span id="text_room_1">{{ text_1 }}</span>
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />
        <span id="text_room_2">{{ text_2 }}</span>
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />
        <span id="text_room_3">{{ text_3 }}</span>
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />
        <span id="text_room_4">{{ text_4 }}</span>
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />

        <span id="text_room_5">{{ text_5 }}</span>
        <img
          id="rhomb_room"
          class="rhomb_room"
          src="../assets/rhomb_blue.svg"
        />
        <span id="text_room_6">{{ text_6 }}</span>
      </div>
    </div>
    <div class="four_screen">
      <img src="../assets/four_screen.png" />
      <span id="name_news">НОВОСТИ НАШЕГО КЛУБА</span>
      <div class="blocks_news">
        <div id="block_news" v-for="item in a" :key="item.a">
          <img id="img_news" src="../assets/img_news.png" />
          <div class="description">
            <span
              >Проведение локального турнира между двумя лучшими команда...</span
            >
          </div>
          <span id="date">24.08.2021</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      a: [1, 2, 3]
    }
  }
};
</script>

<style scoped>
body {
  overflow: hidden;
}
#setting {
  position: absolute;
  width: 2%;
  height: 2%;
  left: 92%;
  top: 3%;
}
.header_bar {
  position: absolute;
  width: 60%;
  height: 5%;
  left: 20%;
  top: 2%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 81.69%;
  /* or 16px */

  align-items: center;
  text-align: center;
}

#advantages {
  position: absolute;
  width: 10.5%;
  left: 0%;

  text-decoration: none;
  color: #ffffff;
}

#periphery {
  position: absolute;
  width: 10.5%;

  left: 25.5%;

  text-decoration: none;
  color: #ffffff;
}

#news {
  position: absolute;
  width: 10.5%;
  left: 51%;
  text-decoration: none;
  color: #ffffff;
}

#contact {
  position: absolute;
  width: 10.5%;
  left: 76.5%;
  text-decoration: none;
  color: #ffffff;
}

.first_screen {
  width: 120%;
  overflow: hidden;
}

.first_screen > img {
  width: 100%;
}

#logo {
  position: absolute;
  width: 465px;
  height: 255px;
  left: 6.5%;
  top: 19.5%;
}

.slang {
  position: absolute;
  width: 39%;
  height: 39%;
  top: 26%;
  left: 52%;
  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 78px;
  line-height: 81.69%;

  display: flex;
  flex-direction: column;
  align-items: center;

  color: #ffffff;
}

#slang_1 {
  position: relative;
  width: 580px;
  height: 130px;
}

#slang_2 {
  position: relative;
  width: 555px;
  height: 130px;
}
#slang_3 {
  position: relative;
  width: 939px;
  height: 130px;
}

.second_screen {
  position: relative;
  width: 120%;
  top: -20px;
  margin-left: -10%;
}

.second_screen > img {
  width: 100%;
}

#name_space {
  position: absolute;
  width: 100%;
  height: 4.5%;
  left: 0px;
  top: 7.12%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 54px;

  text-align: center;
  color: #ffffff;
}

.advantage {
  position: absolute;
  width: 100%;
  height: 25%;
  top: 35%;
  left: 20%;
  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 21px;
  line-height: 24px;
  display: flex;
  align-items: center;

  color: #ffffff;
}

.rhomb {
  position: absolute;
  width: 17.86px;
  height: 17.86px;
  top: 0;

  background: #6d6caf;
  transform: rotate(-45deg);
}

#rhomb {
  top: 0px;
}

#rhomb_1 {
  top: 50%;
}

#rhomb_2 {
  top: 100%;
}

#rhomb_3 {
  left: 38%;
}

#rhomb_4 {
  left: 38%;
  top: 50%;
}

#rhomb_5 {
  left: 38%;
  top: 100%;
}

.advantage span {
  position: absolute;
  width: 25%;
  height: 6%;
}

#game {
  top: 0%;
  left: 2.5%;
}

#efficiency {
  left: 2.5%;
  top: 50%;
}

#time {
  left: 2.5%;
  top: 100%;
}

#cafeteria {
  left: 40.5%;
  top: 0%;
}

#atmosphere {
  left: 40.5%;
  top: 50%;
}

#wifi {
  left: 40.5%;
  top: 100%;
}

.third_screen {
  position: relative;
  width: 100%;
  margin-top: -6%;
}

.third_screen > img {
  width: 100%;
}

#name_iron {
  position: absolute;
  width: 100%;
  left: 0%;
  top: 10%;
  font-family: "Roboto" sans-serif;

  font-style: normal;
  font-weight: 900;
  font-size: 54px;
  line-height: 63px;
  text-align: center;

  color: #ffffff;
}
.block_rooms {
  position: absolute;
  width: 81%;
  height: 27%;
  left: 15%;
  top: 26%;
  display: flex;
  flex-direction: row;
}
#vip_room {
  position: relative;
  left: 5%;
}
#console_room {
  position: relative;
  left: 7.5%;
}
.price_ordinary {
  position: absolute;
  width: 9%;
  height: 7%;
  bottom: -5%;
  left: 9%;
  background-color: #118fab;
}
.price_ordinary span {
  position: absolute;
  left: 22.5%;
  top: 15%;
  font-family: "Roboto" sans-serif;

  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 81.69%;

  display: flex;

  align-items: center;
  text-align: center;

  color: #ffffff;
}
.price_vip {
  position: absolute;
  width: 9%;
  height: 7%;
  bottom: -5%;
  left: 39%;
  background-color: #a57a0e;
}
.price_vip span {
  position: absolute;
  left: 20.5%;
  top: 15%;
  font-family: "Roboto" sans-serif;

  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 81.69%;

  display: flex;

  align-items: center;
  text-align: center;

  color: #ffffff;
}
.price_console {
  position: absolute;
  width: 9%;
  height: 7%;
  bottom: -5%;
  left: 67%;
  background-color: #a50e0e;
}
.price_console span {
  position: absolute;
  left: 15.6%;
  top: 15%;
  font-family: "Roboto" sans-serif;

  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 81.69%;

  display: flex;

  align-items: center;
  text-align: center;

  color: #ffffff;
}
.description {
  position: relative;
  width: 79%;
  height: 32.5%S;
}
#name_room {
  position: absolute;
  width: 20%;
  height: 6%;
}

.four_screen {
  position: relative;
  width: 100%;
  background-color: #181823;
}

.four_screen > img {
  width: 100%;
}

#name_news {
  position: absolute;
  width: 100%;
  height: 14%;
  left: 0%;
  top: 5%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 900;
  font-size: 54px;
  line-height: 63px;
  text-align: center;

  color: #ffffff;
}

.blocks_news {
  position: absolute;
  width: 75%;
  height: 35%;
  top: 33%;
  left: 18%;
  display: flex;
  justify-content: space-around;
  flex-direction: row;
}
#block_news {
  position: relative;
  width: 25%;
  background-color: #0e1016;
}
#img_news {
  position: relative;
  width: 100%;
  top: 0;
  left: 0;
}

.description {
  position: relative;
  left: 0%;
  width: 100%;
  height: 4.5%;
  top: 0%;
  font-size: 16px;
  color: #ffffff;
  word-wrap: break-word;
}
#date{
  position: relative;
  width: 7.6%;
  font-size: 12px;
  color: #ffffff;
  left: 70%;
  top: 50%;
  word-wrap: break-word;

}

@media screen and (max-width: 1280px) {
  #block_news{
    width: 20%;
  }
  .description{
    font-size: 12px;
  }
  #date{
    left: 60%;
  }
  #logo {
    width: 290px;
    height: 159px;
  }
  #name_news{
    font-size: 32px;
  }
  .slang {
    top: 19.5%;
    font-size: 55px;
    height: 25%;
    left: 69%;
  }
  .header_bar {
    font-size: 24px;
    left: 7.5%;
    width: 80%;
  }
  #name_space {
    font-size: 32px;
  }
  .advantage {
    height: 30%;
    font-size: 16px;
    left: 20%;
  }
  .advantage span {
    width: 30%;
  }
  .rhomb {
    width: 14px;
    height: 14px;
  }
  .block_rooms {
    font-weight: normal;
  }
  .price_console span {
    font-size: 15px;
    left: 12%;
    top: 20%;
    font-weight: 400;
  }
  .price_vip span {
    font-size: 15px;
    top: 20%;
    left: 12%;
    font-weight: 400;
  }
  .price_ordinary span {
    font-size: 16px;
    left: 20%;
    top: 25%;
    font-weight: 400;
  }
  #name_iron {
    font-size: 32px;
  }
  .third_screen {
    margin-top: -10%;
  }
}

@media screen and (min-width: 901px) {
}

@media screen and (max-width: 900px) {
  #logo {
    width: 170px;
    height: 90px;
  }
  .description{
    font-size: 10.5px;
  }
  #date{
    font-size: 10.5px;
    left: 50%;
    top: 0%;
  }
   #name_news{
    font-size: 22px;
  }
  .slang {
    font-size: 42px;
    height: 15%;
    left: 70%;
  }
  #slang_3 {
    left: 40%;
  }
  .header_bar {
    font-size: 14px;
    left: 10%;
    width: 80%;
  }
  #setting {
    top: 2%;
  }
  #name_space {
    font-size: 22px;
  }
  .advantage {
    height: 35%;
    font-size: 11.5px;
  }
  .advantage span {
    margin-top: -0.5%;
    width: 30%;
  }
  .price_console {
    width: 10%;
    left: 68.5%;
  }
  .price_vip {
    width: 10%;
  }
  .price_ordinary {
    width: 10%;
  }
  .price_console span {
    font-size: 11px;
    left: 4.5%;
    top: 15%;
    font-weight: 400;
  }
  .price_vip span {
    font-size: 11px;
    font-weight: 400;
    left: 4.5%;
    top: 15%;
  }
  .price_ordinary span {
    font-size: 11px;
    font-weight: 400;
    left: 11%;
    top: 15%;
  }
  #name_iron {
    font-size: 22px;
  }
}

@media screen and (min-width: 591px) {
}

@media screen and (max-width: 590px) {
  #name_news{
    left: -10%;
  }
  .blocks_news{
    width: 70%;
  left: 10%;
  }
  #date{
    font-size: 8.5px;
    top: 40%;
  }
  .four_screen{
    width: 135%;
  }
  .description{
    word-wrap:unset;
    font-size: 8.5px;
    font-weight: normal;
  }
  #block_news{
    left: -10%;
  }
  #logo {
    width: 130px;
    height: 70px;
    top: 15%;
  }
   #name_news{
    font-size: 12px;
  }
  .slang {
    font-size: 24px;
    left: 90%;
    top: 15%;
  }
  .header_bar {
    font-size: 12px;
    width: 80%;
    left: 10%;
  }
  .second_screen {
    height: 400px;
    background-color: #1e1e28;
  }
  #name_space {
    font-size: 12px;
  }
  .advantage {
    font-size: 10.5px;
    top: 20%;
    left: 30%;
    height: 25%;
  }
  .advantage span {
    width: 90%;
  }
  .rhomb {
    width: 10px;
    height: 10px;
  }
  #rhomb_3 {
    left: 0%;
    top: 150%;
  }
  #rhomb_4 {
    left: 0%;
    top: 200%;
  }
  #rhomb_5 {
    left: 0%;
    top: 250%;
  }
  #game {
    left: 5%;
    top: -5%;
  }
  #efficiency {
    left: 5%;
    top: 45%;
  }
  #time {
    left: 5%;
    top: 95%;
  }
  #cafeteria {
    left: 5%;
    top: 145%;
  }
  #atmosphere {
    left: 5%;
    top: 195%;
  }
  #wifi {
    left: 5%;
    top: 245%;
  }
  #name_iron {
    font-size: 12px;
  }
  .price_console span {
    font-size: 9px;
    left: 9%;
  }
  .price_vip span {
    font-size: 9px;
    left: 9%;
  }
  .price_ordinary span {
    font-size: 9px;
  }
}

@media screen and (min-width: 431px) {
}

@media screen and (max-width: 430px) {
  #logo {
    width: 80px;
    top: 8%;
    left: 10%;
  }
  .slang {
    font-size: 16px;
    top: 10%;
    height: 90px;
    left: 110%;
  }
  #slang_3 {
    left: 90%;
  }
  .header_bar {
    font-size: 9px;
    width: 80%;
  }
  #setting {
    left: 85%;
    top: 1.5%;
  }
  .advantage {
    left: 20%;
  }
  .advantage span {
    width: 70%;
  }
  .price_console span {
    font-size: 7.5px;
    left: 7.5%;
  }
  .price_vip span {
    font-size: 7.5px;
    left: 7.5%;
  }
  .price_ordinary span {
    left: 15%;
    font-size: 7.5px;
  }
  .block_rooms {
    width: 100%;
    height: 30%;
    left: 10%;
  }
  .price_vip {
    left: 37.5%;
  }
  .price_console {
    left: 64.5%;
  }
  .price_ordinary {
    left: 8%;
  }
}
</style>