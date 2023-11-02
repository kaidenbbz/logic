<template>
  <div class = "registration">
    <div class = "registration_form">
      <div class = "registration_form__leftside">
        <div class = "img1"></div>
        <p class = "icon">
          REGISTRATION
          <img src="https://pic.onlinewebfonts.com/thumbnails/icons_68882.svg" class = "icon1">
        </p>
        
      </div>
      <div class = "registration_form__rightside">
        <div class = "registration_form__name">
          <p class = "title">Name</p>
          <input type="text" class = "text" placeholder="Write here...">
        </div>
        
        <div class = "registration_form__sex">
          <p class = "title">Sex</p>
          <div class = "radio-containers">
            <div class = "radio-container">
              <input type="radio" class = "radio" name="gender">
              <p class="sex-picture">♂</p>
              <span>Man</span>  
            </div>
            <div class = "radio-container">
              <input type="radio" class = "radio" name="gender">
              <p class="sex-picture2">♀</p>
              <span>Woman</span>  
            </div>
          </div>
        </div>
        <div class = "registration_form__email">
          <p class = "title">Email</p>
          <input type="text" class = "text" placeholder="Write here...">
        </div>
        <div class="registration_form__country">
          <div class="title">Country</div>
            <div class = "country-select">
              <select>
                <option value ="0"> Select a country</option>
                <option value="1">Россия</option>
                <option value="2">Амэрика</option>
                <option value="3">Ураина</option>
              </select>
            </div>
        </div>
        <div class = "registration-form__submit">
          <button class = "submit">Отправить</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  .registration{
    width: 100vw;
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: "Loopy V2";
  }
  .icon{ 
    font-size: 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 25px;
    .icon1{
      height: 50px;
      width: 50px;
    }
  }
  .registration_form{
    display: grid;
    width: 70vw;
    height: 80vh;
    border-radius: 30px;
    grid-template-columns: 1fr 2fr;
  }
  .registration_form__leftside{
    background-color: red;
    border-top-left-radius: 30px;
    border-bottom-left-radius: 30px;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20% 0 30% 0;
    flex-direction: column;
    font-weight: bolder;
    
  }
  .img1{
    height: 150px;
    width: 150px;
    border-radius: 50%;
    background-color: white;
  }
  .registration_form__rightside{
    padding: 5vh 3vw;
    display: flex;
    border-top-right-radius: 30px;
    border-bottom-right-radius: 30px;
    background-color: grey;
    flex-direction: column;
    gap: 30px;
    p{
      font-size: 20px;
    }
  }
  .text{
    height: 40px;
    font-size: 20px;
    width: 100%;
    
    
  }   
  .gender{
    display: flex;
    gap: 20px;
  }
  .radio{
    height: 50px;
    width: 50px;
    margin: 0;
    padding: 0;
  }
  .radio-container{
    margin-right: 30px;
    display: flex;
    align-items: center;
    gap: 30px;
    justify-content: center;
    span{
      font-size: 20px;
    }
  }
  .registration_form__sex{
    display: flex;
    justify-content: center;
    flex-direction: column;
  }
  .sex-title{
    display: inline-flex;
  }
  .radio-containers{
    display: flex;
    justify-content: center;
    gap: 100px  ;
  }
  .title{
    font-size: 20px;
    font-weight: bolder;
  }
  .sex-picture{
    position: absolute;
    transform: translate(-37px, 0px);
    cursor: default;
    user-select: none;
    pointer-events: none;
  }
  .sex-picture2{
    position: absolute;
    transform: translate(-53px, 0px);
    cursor: default;
    user-select: none;
    pointer-events: none;
  }
  .title-country{
    height: 40px;
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    font-size: 20px;
  }
  .registration_form__country{
    gap: 20px;
    display: flex;
    flex-direction: column;
    select{
    height: 40px;
    width: 100%;
    font-size: 20px;
  }
  }
  .registration-form__submit{
    height: 100%;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }

  .submit{
    font-size: 40px;
    background-color: purple;
    color: white;
    outline: none;
    margin: 0;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    border-radius: 15px;
  }
  

 
</style>
<script setup>

</script>
