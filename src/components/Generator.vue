<template>
  <div id="gen">
    <div class="gen_img">
      <div class="img_blueline"></div>

      <div class="img_background">
        <p >{{tittle}}</p>
       <p> Damian Szmurło</p>
      </div>
      <div class="img_description">
        <h2>A bit more about project</h2>
        <p>{{description}}</p>
      </div>
      <div class="img_skill">
        <h2>Skills</h2>
        <p>Technologies used:</p>
        <ul>
          <li v-if="skill1 != ''">{{skill1}}</li>
          <li v-if="skill2 != ''">{{skill2}}</li>
          <li v-if="skill3 != ''">{{skill3}}</li>
          <li v-if="skill4 != ''">{{skill4}}</li>
          <li v-if="skill5 != ''">{{skill5}}</li>
        </ul>
      </div>
    </div>

    <div class="gen_generator">
      <div></div>
      <div>
        <label for>Tittle</label>
        <input v-model="tittle" type="text" />
      </div>
      <div>
        <label for> Description</label>
        <input v-model="description" type="text" />
      </div>
      <div>
        <label for>Skill</label>
        <input v-model="skill1" type="text" />
        <input v-model="skill2" type="text" />
        <input v-model="skill3" type="text" />
        <input v-model="skill4" type="text" />
        <input v-model="skill5" type="text" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tittle: "PSD TO HTML",
      description: "Simple psd to html website nothing amazing",
      skill1: "HTML5",
      skill2: "CSS",
      skill3: "SASS",
      skill4: "VUE",
      skill5: ""
    };
  }
};
</script>

<style  scoped>
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}
.gen_img {
  margin: 0 auto;
  height: 558px;
  width: 442px;
}
.gen_generator {
  margin: 0 auto;
  margin-top: 40px;
  width: 442px;
  height: 300px;
  background-color: white;
  padding: 15px;
}
.gen_generator > div {
  display: flex;
  flex-direction: column;
  text-align: left;
  margin-bottom: 10px;
  font-size:20px;
}
.gen_generator > div > input {
  margin-top: 5px;
  border:none;
  border-bottom: 1px solid grey;
  text-align: center;
  padding: 2px;
}
.img_blueline {
  width: 100%;
  height: 3px;
  background-color: #16cae6;
}
.img_background {
  height: 236px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-image: url("https://media.licdn.com/dms/image/C4E16AQGu1PMz5Rarbw/profile-displaybackgroundimage-shrink_350_1400/0?e=1571875200&v=beta&t=bhSi6bjzKTwuCx0vreeKNskost66jA9rQXEKQIcraAo");
  background-position: center;
  background-size: 150% 100%;
}
.img_background > p {
  color: white;
  font-size: 1.8em;
  opacity: 0.95;
}
.img_background > p:last-child{
  margin-top: 5px;
  font-size:16px;
  color: white;
  opacity: .7;
}
.img_description {
  text-align: left;
  padding: 20px;
  background-color: white;
  height: 100px;
}
.img_description > p {
  margin-top: 10px;
}
.img_description > h2 {
  font-size: 22px;
}
.img_skill {
  color: white;
  background-color: #16cae6;
  height: 200px;
  text-align: left;
  padding: 15px;
}
.img_skill > h2 {
  margin-bottom: 5px;
}
.img_skill > ul {
  margin-top: 10px;
  margin-left: 20px;
}
.img_skill > ul > li {
  margin-top: 5px;
}

</style>
