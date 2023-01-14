<template>
  <div class="resume">
    <div class="left">
      <div class="subtitle1">
        <h2>Education</h2>
      </div>
      <div class="life" v-for="school in education">
        <img class="image" :src="school.image" alt="" srcset="" />
        <h3>{{ school.title }}</h3>
        <h5>{{ school.year }}</h5>
        <div class="content">
          <p>{{ school.message }}</p>
        </div>
      </div>
    </div>
    <div class="right">
      <div class="subtitle2">
        <H2>Skills</H2>
      </div>
      <div class="star" v-for="skill in skills">
        <img :src="skill.image" alt="" srcset="" />
        <h4>{{ skill.text }}</h4>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star"></span>
      </div>
      <div class="subtitle2">
        <h2>Interests</h2>
      </div>
      <ul>
        <li>Volunteer work</li>
        <li>Music</li>
        <li>Hiking</li>
        <li>Outdoor Activities</li>
      </ul>
      <div class="icons">
        <a href="https://www.linkedin.com/in/uzukhanye-dywili-a6976b255" target="_blank">
          <i class="fa-brands fa-linkedin fa-bounce"></i
        ></a>
        <a href="https://www.instagram.com/uzukhanyedywili" target="_blank">
          <i class="fa-brands fa-instagram fa-bounce"></i
        ></a>
        <a href="https://www.github.com/Azukiwe" target="_blank">
          <i class="fa-brands fa-github fa-bounce"></i
        ></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      education: [
        {
          image:
            "https://i.postimg.cc/y8XQWmBj/life-choices-removebg-preview.png",
          year: 2022,
          title: "Challenge to self",
          message:
            "continued doing my N5 for the first 6 months of the year,slowly lost interest felt I like i was too comfortable and decide to challenge  myself by applying @ Life Choices Academy.",
        },
        {
          image: "https://i.postimg.cc/WbC7V1nM/images-removebg-preview.png",
          year: 2021,
          title: "College",
          message:
            "Accepted to study Business Management @ False Bay College,passed my N4 with 2 Distinctions.",
        },
        {
          image: "https://i.postimg.cc/8kvGLNkt/boy-removebg-preview.png",
          year: 2020,
          title: "Matric",
          message: "Doing my Matric and passed.",
        },
        {
          image:
            "https://i.postimg.cc/HnDWn9W3/Senior-Years-removebg-preview.png",
          year: 2018,
          title: "Senior Years",
          message:
            "Doing Grade 10 and chose my subjects(big decision). Chose Accounting,History, Mathematics, Life Sciences(including the mandatory languages) with the hopes that these subjects will gaurantee that I be excepted in Universities for Chartered Accountant..",
        },
        {
          image: "https://i.postimg.cc/MZFv218c/LHS-logo-removebg-preview.png",
          year: 2016,
          title: "High School",
          message: "started high school @ Livingstone High School.",
        },
      ],
      skills: [
        {
          image: "https://i.postimg.cc/02WgvVLp/csslogo-removebg-preview.png",
          text: "CSS",
        },
        {
          image: "https://i.postimg.cc/FKpgn2t5/java-logo-removebg-preview.png",
          text: "JAVASCRIPT",
        },
        {
          image: "https://i.postimg.cc/63BmsR57/html-logo-removebg-preview.png",
          text: "HTML",
        },
        {
          image:
            "https://i.postimg.cc/prb3dTv8/BOOTSTRAP-LOGO-removebg-preview.png",
          text: "BOOTSTAP",
        },
        {
          image:
            "https://i.postimg.cc/k4hkPc1j/vue-js-logo-removebg-preview.png",
          text: "VUE JS",
        },
      ],
    };
  },
};
</script>
<style scoped>
.resume {
  display: flex;
}
.left,
.right {
  width: 50vw;
  display: flex;
  flex-direction: column;
  gap: 4rem;
  padding: 0;
  margin:0;
}

.image {
  scale: 0.5;
  
}
.life {
  min-height: 18rem;
  font-family: "Courier New", Courier, monospace;
}
.star{
  scale: 0.8;
  min-height: 6rem;
}
.subtitle1::first-letter,
.subtitle2::first-letter {
  font-size: 4rem;
  color: plum;
}
.subtitle1, .subtitle2{
  font-family: Arial, Helvetica, sans-serif;
}
ul{
  list-style: none;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
 margin-left: 19rem;

}
ul li::before{
  content:"\2022";
  color:orangered;
  font-weight: bold;
}
.fa-bounce{
padding:2rem;
color: black;
font-size: 3rem;
}
.checked {
  color: orangered;
}
</style>
