<template >
    <div class="card">
    <div class="flip-card" v-for="testimonial in testimonials ">
        <div class="flip-card-inner">
          <div class="flip-card-front">
            <img :src="testimonial.image" alt="Avatar" style="width:300px;height:300px;">
          </div>
          <div class="flip-card-back">
            <h1>{{ testimonial.name }}</h1> 
            <p>{{ testimonial.relation }}</p> 
            <p>{{ testimonial.comment }}</p>
          </div>
        </div>
      </div>
    </div>
</template>
<script>
export default {
    data() {
    return {
testimonials:[
    {name: 'Kelebogile Nobomvu',
image:'https://i.postimg.cc/HLcBCKX5/lebo.jpg' ,
relation:'Life Choices Academy,Colleague ',
comment:"Uzukhanye is a grounded and loving individual who easily adapts to changes,works hard on completing her tasks and developing her skills."
},
{name: 'Oslin Johnson', 
    image: 'https://i.postimg.cc/HkSQn2d2/pic2.jpg',
    relation:'Life Choices Academy,Lecturer ',
    comment: `Uzukhanye is a the definition of dynamite comes in small packages, as she has good potential that she is slowly realizing it. Her attitude to finding a solution to problems is admired and she doesn't lay down to anything which is admirable.`
    },
    {name: 'Abdul-Azeez Kemp',
        image: 'https://i.postimg.cc/fRNjtLGH/abdul.jpg',
        relation:'Life Choices Academy,Colleague ',
        comment: `Uzukhanye, she's a wonderful being, great to work with,
        always puts her 100% effort in working and a great team
        player.`
        },
        {name: 'Nikita Ramawoothar',
            image: 'https://i.postimg.cc/XN5f5kXg/IMG-6122.jpg',
            relation:'Life Choices Academy,Colleague ',
            comment:`Uzukhanye is a very creative individual and is always
            pleasant company to have within the workplace. She is not only
            helpful but also an exceptional developer that you can always
            count on to get some ideas and inspiration from.`
            },
            {name: 'Candice Amon',
                image: 'https://i.postimg.cc/3rb3x0vT/candice-2022.jpg',
                relation:'Life Choices Academy,Facilitator ',
                comment:  `Uzukhanye is very likable amongst her peers due to her
                positive bubbly nature. Has very strong social skills and can
                easily adapt to an environment. Can be an awesome team player
                and displays great boldness.`
                },
                {name: 'Deno Rautenbach',
                    image: 'https://i.postimg.cc/s2hRxT5d/Deno.jpg',
                    relation:'Life Choices Academy,Colleague ',
                    comment:  `A woman of class and elegance, a prepossessing sight and of
                    course consisting of unfathomable intelligence. Always happy
                    to help, even if she's always tired. Uzukhanye's friendly aura
                    invites a sense of comfort whenever we assist one another on
                    work. She radiates joy and that translates into her code as
                    her flair for design triumphs any I've seen so far. Poor
                    eyesight aside, anything she creates is always vibrant and a
                    feast for the eye's.`
                    },
]
    }
},
}
</script>
<style scoped>

.card{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 4rem;
    background-color: lightgrey;
    margin: 4rem;
    border: none;
    
}
.flip-card {
    background-color: transparent;
    width: 300px;
    height: 300px;
    perspective: 1000px;
  }
  
  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.6s;
    transform-style: preserve-3d;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  }
  
  .flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
  }
  
  .flip-card-front,
  .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
  }
  
  .flip-card-front {
    background-color: #bbb;
    color: black;
  }
  
  .flip-card-back {
    background-color: plum;
    color:white;
    transform: rotateY(180deg);
    overflow-y: auto;
    font-weight: bold;
  }
  
</style>