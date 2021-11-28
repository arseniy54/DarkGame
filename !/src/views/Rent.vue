<template>
  <div>
    <div class="base">
      <img src="../assets/fon_rent.png" />
      <img id="logo" src="../assets/logo_rent.svg" />
      <div class="form_rent">
        <span id="user_name">Имя</span>
        <input type="text" id="name_input" placeholder="Ваше Имя" />
        <span id="user_phone">Номер телефона</span>
        <input type="text" id="phone_input" placeholder="+7(123)456-78-90" />
        <span id="user_email">Электронная почта</span>
        <input type="text" id="email_input" placeholder="Example@gamedark.ru" />
        <span id="type_room">Тип игрового зала</span>
        <div class="radio_room">
            <input type="radio" name="room" class="custom_radio" id="standart_room">
            <span id="standart_span">Standart</span>    
            <input type="radio" name="room" class="custom_radio" id="vip_room">
            <span id="vip_span">Premium</span>
            <input type="radio" name="room" class="custom_radio" id="console_room">
            <span id="console_span" >Console</span>
        </div>
        <span id="time_game">Время брони</span>
        <input list="limittime" type="time" id="time_game_start">
        <input  list="limittime"  type="time" id="time_game_end">
        <button @click="OnSubmit()">Бронь</button>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios';
  data:{
    return {
      books: [],
      addBooking: {
        Name: '',
        Number: '',
        Email: '',
        Type: ''
      },
    }
  };
  
  methods: {
  addBook(payload);{
  const path = '';
  axios.post(path, payload)
    .then(() => {
     console.log("Пост запрос выполнен");
    })
    .catch((error) => {
      // eslint-отключение следующей строки
      console.log(error);
      
    });
  }
  initForm();{
      this. Name= '';
      this.Number = '';
      this.Email = '',
      this.Type = ''
     
    }
    onSubmit(evt);{
      evt.preventDefault();
      this.$refs.addBookModal.hide();
      let read = false;
      if (this.addBookForm.read[0]) read = true;
      const payload = {
        Name: this.Name,
        Number:this.Number,
        Email:this.Email,
        occude:this.Type
      };
      this.addBook(payload);
      this.initForm();
    }
       
  }
</script>

<style  scoped>
.base {
  width: 100%;
}
#logo {
  position: absolute;
  left: 7.03%;
  top: 10.02%;
}
.form_rent {
  position: absolute;
  width: 62%;
  height: 110%;
  top: 43.6%;
  left: 20.5%;
}
#user_name,
#user_phone,
#user_email,
#type_room,
#time_game{
  position: absolute;
  width: 100%;
  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 37px;
  line-height: 43px;
  display: flex;
  align-items: center;

  color: #ffffff;
}
#user_name {
  left: 2.5%;
}
#user_phone {
  top: 21%;
  left: 2.5%;
}
#user_email {
  top: 42.5%;
  left: 2.5%;
}

#time_game{
    top: 90%;
}

input[type=time]{
    position: absolute;
    top: 95%;
}

input[type=text]{
  position: absolute;
  width: 100%;
  height: 66px;
  background: rgba(0, 0, 0, 0.35);
  border: 1px solid rgba(255, 255, 255, 0.09);
  border-radius: 6px;
  color: #ffffff;
  font-size: 37px;
padding-left: 1.5%;
}


#name_input {
  top: 4%;
}

#phone_input {
  top: 25%;
  left: 0%;
}

#email_input {
  top: 46.5%;
}

#type_room{
top: 63%;

}
.radio_room{
    position: absolute;
    width: 100%;
    top: 70%;
}

input[type=radio]{
    position: absolute;
    width: 38px;
    height: 38px;
}

#standart_room{
    left: 2%;
}

#standart_span{
    left: 7%;
}

#vip_room{
    left: 42% ;
}

#vip_span{
    left: 47%;
}

#console_room{
    left: 82%;
}

#console_span{
    left:  87%;
}


#standart_span, #vip_span, #console_span{
position: absolute;
font-family: "Roboto" sans-serif;
font-style: normal;
font-weight: bold;
font-size: 37px;
line-height: 43px;
display: flex;
align-items: center;

color: #FFFFFF;
}

::-webkit-input-placeholder {
  position: absolute;
  top: 20%;
  left: 1.5%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 33px;
  line-height: 39px;

  color: rgba(255, 255, 255, 0.17);
}
::-moz-placeholder {
  position: absolute;
  top: 20%;
  left: 1.5%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 33px;
  line-height: 39px;

  color: rgba(255, 255, 255, 0.17);
} /* Firefox 19+ */
:-moz-placeholder {
  position: absolute;
  top: 20%;
  left: 1.5%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 33px;
  line-height: 39px;

  color: rgba(255, 255, 255, 0.17);
} /* Firefox 18- */
:-ms-input-placeholder {
  position: absolute;
  left: 1.5%;
  top: 10%;

  font-family: "Roboto" sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 33px;
  line-height: 39px;

  color: rgba(255, 255, 255, 0.17);
}
</style>