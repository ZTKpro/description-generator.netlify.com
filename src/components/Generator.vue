<template>
  <div id="gen">
    <div class="gen_img">
      <div class="img_blueline">
     </div>

      <div class="img_background">
         <p>
        {{tittle}}
        </p>
     </div>
      <div class="img_description">
      <h2>A bit more</h2>
      <p>{{description}}</p>
      </div>
      <div class="img_skill">
      <h2>Skills</h2>
      <p> Technologies uses: </p>
      <ul>
        <li>
        {{skill1}}
        </li>
        <li>
        {{skill2}}
        </li>
        <li>
        {{skill3}}
        </li>
        <li>
        {{skill4}}
        </li>
        <li>
        {{skill5}}
        </li>
      </ul>
      </div>
    </div>

     <div class="gen_generator">
      <input type="text">
      <input type="text">
      </div>
  </div>
</template>

<script>
export default {
data() {
  return {
  tittle:"PSD TO HTML",
  description:'Simple psd to html website nothing amazing',
  skill1:'HTML5',
  skill2:'CSS',
  skill3:'SASS',
  skill4:'VUE',
  skill5:'',
  }
},
}
</script>

<style  scoped> 
*{
  margin:0px;
  padding:0px;
  box-sizing:border-box;
}
.gen_img{
  margin:0 auto;
    height: 558px;
        width: 442px;
}
.gen_generator{
   margin:0 auto;
  margin-top:40px;
  width: 442px;
}
.img_blueline{
  width:100%;
  height:3px;
  background-color:#16cae6;
}
.img_background{
  height:236px;
  background-color:grey;
  display: flex;
  justify-content: center;
  align-items:center;
  background-image: url("https://media.licdn.com/dms/image/C4E16AQGu1PMz5Rarbw/profile-displaybackgroundimage-shrink_350_1400/0?e=1571875200&v=beta&t=bhSi6bjzKTwuCx0vreeKNskost66jA9rQXEKQIcraAo");
background-position: center;
    background-size: 150% 100%;
 
}
.img_background > p{
 color:white;    
  font-size:2em;
  opacity:.95;
}
.img_description{
  background-color:white;
  height: 100px;
}
.img_skill{
  background-color:#16cae6;
  height: 200px;
}
</style>
