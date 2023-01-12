<template>
  <div class="grid-container">
    <div class=" flip-card" v-for="key in projects">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img
            :src="key.image"
            alt="project"
            style="width: 15rem; height: 15rem;"
          />
         <h5 class="card-title">{{key.project}}</h5>
        </div>
        <div class="flip-card-back">
          <div class="card-body">
            
            <p class="card-text">
              {{key.description}}
            </p>
          </div>

          <div class="card-body text-center">
            <a
              :href= key.live
              class="card-link mybtn"
              >Live</a
            >
            <a
              :href=key.github
              class="card-link mybtn"
              >Github</a
            >
          </div>
        </div>
      </div>
    </div>
</div>
</template>

<script>

export default {
  data() {
    return {
        projects: [
            {
                project:"Calculator",
                image:"https://i.postimg.cc/d07JQ1H3/calculator.jpg",
                description:"Standard Calculator, made using HTML,CSS and JavaScript",
                live:"https://calculator-thokozani.netlify.app/",
                github:"https://github.com/ThokozaniNqwili/CalculatorTask.git"
            },
            {
                project:"Flip Cards",
                image:"https://i.postimg.cc/K8WyQtQv/5907.jpg",
                description:" A card with content on both sides, back and front, made with CSS and HTML",
                live:"https://myflipcards.netlify.app/",
                github:"https://github.com/ThokozaniNqwili/Flip-Cards.git"
            },
            {
                project:"Travel Addicts",
                image:"https://i.postimg.cc/Qd2vMv8Y/glen-boutique-hotel.jpg",
                description:"E-commerce website for holiday accomodation, made with HTML,CSS and JavaScript",
                live:"https://travel-addicts.netlify.app/",
                github:"https://github.com/ThokozaniNqwili/TravelAddicts.git"
            },
            {
                project:"Foodies Market",
                image:"https://i.postimg.cc/bwmvPGTK/logo.png",
                description:"A food market e-commerce created using Bootsrap and HTML.",
                live:"https://foodiesmarket.netlify.app/",
                github:"https://github.com/ThokozaniNqwili/Foodies.git"
            },
            {
                project:"BMI Calculator",
                image:"https://i.postimg.cc/Dz7Y5YsT/bmi.jpg",
                description:"Calculates BMI using height and weight, made with Javascript, HTML and CSS",
                live:"https://thokozanibmicalculator.netlify.app/",
                github:"https://github.com/ThokozaniNqwili/BMICalculator.git"
            },
            {
                project:"Temperature Convertor",
                description:"",
                live:"",
                github:""
            }
        ]
    }
},

}
</script>

<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto auto;
  padding: 1rem;
  margin: 1rem;
  
}
.flip-card {
  background-color: #FFDEDE;
  width: 18rem;
  height: 20rem;
  perspective: 1000px;
  margin: 1rem;
  

}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 #EB4747;
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color:#ABC9FF;
  color: black;
}

.flip-card-back {
  padding-top: 50px;
  background-color:#FFDEDE;
  color: black;
  transform: rotateY(180deg);
}
@media (width: 300px){
  .grid-container {
    display: grid;
    grid-template-columns: auto;
  
  }
  .flip-card {
    width:14rem;
    height: 15rem;
  }

}
</style>