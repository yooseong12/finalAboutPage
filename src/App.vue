<template>
  <div class="app">
    <div class="header">
      <h1>팀원 발표</h1>
    </div>
      <div class="mainBox">
        <div class="mainLogo">
          <img src="./assets/image1.png" alt="">
          <h1>Javascript</h1>
        </div>

      <div class="mainImage1">
      <img src="https://cdn.clien.net/web/api/file/F01/9145237/44ba366a36a84a.jpg?w=780&h=30000" class="img1"/>
      <h2>김유성</h2>
      <div class="aTagBox">
        <ModalView1 v-if="isModalViewed1" @close-modal="isModalViewed1 = false">
          <yooseong />
          </ModalView1>
      <a href="javascript:void(0)" class="aTag" @click="isModalViewed1 = true">느낀 점</a>
          <ModalView2 v-if="isModalViewed2" @close-modal="isModalViewed2 = false">
          <yooseongImg />
          </ModalView2>      
      <a href="javascript:void(0)" class="aTag1" @click="isModalViewed2 = true">만든 페이지</a>
      </div>
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSwweEo7T_CjjdRSV5koIvroo8gtNaI1_E9iQ&usqp=CAU" class="img2"/>
      <h2>고진혁</h2>
      <div class="aTagBox">
       <ModalView3 v-if="isModalViewed3" @close-modal="isModalViewed3 = false">
          <jinhyuk />
          </ModalView3>
      <a href="javascript:void(0)" class="aTag" @click="isModalViewed3 = true">느낀 점</a>
          <ModalView4 v-if="isModalViewed4" @close-modal="isModalViewed4 = false">
          <jinhyukImg />
          </ModalView4>
      <a href="javascript:void(0)" class="aTag1" @click="isModalViewed4 = true">만든 페이지</a>
      </div>
      </div>

      <div class="mainImage2">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSCTBt3IdD6fo2-sNraGURr0GlUvNOTVywZOQ&usqp=CAU" class="img1"/>
      <h2>신성철</h2>
      <div class="aTagBox">
      <ModalView5 v-if="isModalViewed5" @close-modal="isModalViewed5 = false">
          <Seongcheol />
          </ModalView5>
      <a href="javascript:void(0)" class="aTag" @click="isModalViewed5 = true">느낀 점</a>
                        <ModalView6 v-if="isModalViewed6" @close-modal="isModalViewed6 = false">
          <SeongcheolImg />
          </ModalView6>
      <a href="javascript:void(0)" class="aTag1" @click="isModalViewed6 = true">만든 페이지</a>
      </div>
      <img src="https://scontent-ssn1-1.xx.fbcdn.net/v/t1.6435-9/131335717_3828397587199389_4155341957141734026_n.jpg?_nc_cat=106&ccb=1-5&_nc_sid=973b4a&_nc_ohc=S147VM8Nq7AAX_Q8inl&_nc_oc=AQnwYSwO-Iv0WlTTEWtBWAhkPucyoYsW_qXClFfXr-Dwnn-qy1Et50CAjniMixA2Fp4&_nc_ht=scontent-ssn1-1.xx&oh=97cc1ff2885ca66567143822976c61ed&oe=61AE4C56" class="img2"/>
      <h2>남정훈</h2>
      <div class="aTagBox">
       <ModalView7 v-if="isModalViewed7" @close-modal="isModalViewed7 = false">
          <jeonghoon />
          </ModalView7>
      <a href="javascript:void(0)" class="aTag" @click="isModalViewed7 = true">느낀 점</a>
                        <ModalView8 v-if="isModalViewed8" @close-modal="isModalViewed8 = false">
          <jeonghoonImg />
          </ModalView8>
      <a href="javascript:void(0)" class="aTag1" @click="isModalViewed8 = true">만든 페이지</a>
      </div>
      
      
      </div>

      
      

    </div>
    
    
 
  </div>
  
</template>
<script>
import ModalView1 from "./components/ModalView/ModalView1";
import ModalView2 from "./components/ModalView/ModalView2";
import ModalView3 from "./components/ModalView/ModalView3";
import ModalView4 from "./components/ModalView/ModalView4";
import ModalView5 from "./components/ModalView/ModalView5";
import ModalView6 from "./components/ModalView/ModalView6";
import ModalView7 from "./components/ModalView/ModalView7";
import ModalView8 from "./components/ModalView/ModalView8";


import yooseong from "./components/person/yooseong";
import jinhyuk from "./components/person/jinhyuk";
import Seongcheol from "./components/person/Seongcheol";
import jeonghoon from "./components/person/jeonghoon";
import yooseongImg from "./components/person/yooseongImg";
import jinhyukImg from "./components/person/jinhyukImg";
import SeongcheolImg from "./components/person/SeongcheolImg";
import jeonghoonImg from "./components/person/jeonghoonImg";

export default{
  name: "App",
  components:{
    yooseong,
    jinhyuk,
    Seongcheol,
    jeonghoon,
    ModalView1,
    ModalView2,
    ModalView3,
    ModalView4,
    ModalView5,
    ModalView6,
    ModalView7,
    ModalView8,
    yooseongImg,
    jinhyukImg,
    SeongcheolImg,
    jeonghoonImg

  },
  data(){
    return{
      isModalViewed1:false,
      isModalViewed2:false,
      isModalViewed3:false,
      isModalViewed4:false,
      isModalViewed5:false,
      isModalViewed6:false,
      isModalViewed7:false,
      isModalViewed8:false,
      
    }
  }
}

</script>



<style scoped>

h2{
  padding-top: 10px;
  text-align: center;
}
  .header{
    padding-top:30px;
    text-align: center;
  }

  .mainBox{
    width: 1400px;
    margin: 0 auto;
    display: flex;
    background-color:rgb(243, 199, 248);
    border-radius:10%;
    box-shadow: 5px 5px 8px 5px gray;
  }
  .mainLogo{
    padding-top:180px;

  }
  .mainLogo img{
    width: 350px;
    height: 400px;
  }
  .mainLogo h1{
    margin-top: -30px;
    margin-left: 70px;
    font-size: 3em;
  }

  .img1{
    width: 300px;
    height: 200px;
    border-radius: 70%;
  }

  .aTag{
    margin-left: 20px;
    border: #555555 solid 1px;
    border-radius: 40px;
    color: #000000;
    padding: 18px 28px;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 600;
  }

  .aTag:hover{
    border: #fdd000 solid 2px;
    background-color: #fdd000;
    border-radius: 40px;
    color: #000000;
    padding: 18px 28px;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 600;
  }

  .aTag1{
    margin-left : 20px;
    border: #555555 solid 1px;
    border-radius: 40px;
    color: #000000;
    padding: 18px 28px;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 600;
  }

  .aTag1:hover{
    border: #fdd000 solid 2px;
    background-color: #fdd000;
    border-radius: 40px;
    color: #000000;
    padding: 18px 28px;
    text-decoration: none;
    font-size: 1rem;
    font-weight: 600;
  }
  
  
  

  .aTagBox{
    margin-top:30px;
  }

  .img2{
    width: 300px;
    height: 200px;
    border-radius: 70%;
    margin-top:60px;
  }
  
  .mainImage1{
    margin-left: 100px;
  padding : 50px;

  }
  .mainImage2{
    padding : 50px;
  }
  
  
</style>