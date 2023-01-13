<template >
  <div class="container">
  <div class="card-2" style="width: 18rem; display:flex; background-color: white; height:24rem" v-for="project in projects">
    <div class="card-whole">
    <img :src="project.image" class="card-img-top" alt="...">
    <div class="card-body">
      <h2 class="card-title">{{project.name}}</h2>
      <a :href="project.github" ><button>Check code</button ></a >
      <a :href="project.netlify"><button>Go Live</button></a>
    </div>
  </div>
</div>
</div>

</template>
<script>
export default {
    data(){
      return {
        projects:[
          {
          name: "Black Technology",
          image: "https://i.postimg.cc/DZvh5W2q/2.png",
          github: "https://github.com/Azukiwe/black-technology",
          netlify: "https://black-technology.netlify.app",
        },
        {
          name: "Calculator",
          image: "https://i.postimg.cc/NMyVNGwN/homepage.jpg",
          github: "https://github.com/Azukiwe/calculator",
          netlify: "https://calc-ud.netlify.app",
        },
        {
          name: "Free People Boutique",
          image: "https://i.postimg.cc/WpBXMLb7/people.jpg",
          github: "https://github.com/Azukiwe/Free-People-Boutique",
          netlify: "https://free-people.netlify.app",
        },
        {
          name: "Sneaker",
          image: "https://i.postimg.cc/BQHgRHKf/hi2-removebg-preview.png",
          github: "https://github.com/Azukiwe/sneaker_site_2",
          netlify: "https://sneaker2.netlify.app",
        },
        {
          name: "Bootstrap portfolio",
          image: "https://i.postimg.cc/c4t7kK2y/49260-20210426-vr-premium-w660.jpg",
          github: "https://github.com/Azukiwe/Uzu-portfolio",
          netlify: "https://uzukhanye-portfolio.netlify.app",
        },
        {
          name: "Cards",
          image: "https://i.postimg.cc/pTQ6zML1/6-removebg-preview.png",
          github: "",
          netlify: "",
        },
      ]
    }
}
}
</script>
<style scoped>
  .container{
    display: grid;
    grid-template-columns: auto auto auto;
    gap: 2rem;
    margin: 6rem;
   
  }
  button{
   margin:1.5rem;
   border: 0.2rem solid plum;
   background-color: plum;
  border-radius: 20%;
  }


 
</style>