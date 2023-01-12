<template>
    <div class="education text-center">
        <h2>Education</h2>
        
          <i
            class="fas fa-graduation-cap cap"
            style="font-size: 4rem; color: #ef798a"
          ></i>
         
        <div class="educationlist" v-for="i in education">
          <ul>
            <li>
              <span>{{i.year}}</span>
              <p>{{i.institution}}</p>
            </li>
          </ul>
        </div>
</div>
        <div class="skills">
          <h2>Technical skills</h2>
          
            <div class="grid-skill"  >
              <div class="skill" v-for="a in technical">
              <h6>{{a.skill}}</h6>
              <img
            :src="a.logo"
            alt="skill"
            class="logo"
          />
          </div>
            </div>  
          </div>

          <div class="experience">
            <h2>Work Experience</h2>
            <div class="timeline-items">
              <div class="timeline-item" v-for="work in experience">
                <div class="timeline-dot"></div>
                <div class="timeline-date">{{work.date}}</div>
                <div class="timeline-content">
                  <h4>{{work.position}} <br>{{work.company}}</h4>
                  <p class="text-sm-start">
                    {{work.duties}}
                  </p>
                </div>
              </div>
              </div>


          </div>




        
      

</template>

<script>
export default {
  data() {
    return {
        education:[
            {
                year:"2022 - Present",
                institution:"Life Choices Academy"

            },
            {
                year:"2018 - 2021",
                institution:"Bcom Information Systems - University Of Cape Towm"

            },
            {
                year:"2013-2017",
                institution:"Matric - Centre of Science and Technology"

            }



        ],
        technical:[
          {
            skill:"HTML",
            logo:"https://i.postimg.cc/cHXcbPnt/html2.png"
          },
          {
            skill:"CSS",
            logo:"https://i.postimg.cc/MTSWFFSw/css3.png"
          },
          {
            skill:"BOOSTRAP",
            logo:"https://i.postimg.cc/g2VSzLWp/bootstrap.png"
          },
          {
            skill:"C-Sharp",
            logo:"https://i.postimg.cc/jSTHx8cg/C-Sharp.png"
          },
          {
            skill:"JAVASCRIPT",
            logo:"https://i.postimg.cc/ZqY9W21R/javascriptlogo.png"
          },
          {
            skill:"VUEJS",
            logo:"https://i.postimg.cc/R0n59QR0/vue2.png"
          }
        ],
        experience:[
          {
            date:"May 2022 - September 2022",
            position:"Technical Support Consultant",
            company:"iStore Somerset",
            duties:"Troubleshoot problems and diagnose and solve technical issues"
          },
          {
            date:"February 2020 - November 2021",
            position:"Information Systems 1 Tutor",
            company:"University of Cape Town",
            duties:"Tutor students information technologies and its use in business"


          },
          
        ]

    }
}
}
</script>

<style>


.cap i{
    align-items: center;
    margin:  1rem;
}
.educationlist li{
    list-style: none;
    font-size: 1.3rem;
    padding: 0.5rem;
    align-items: center;
   
}
.educationlist li span{
    font-weight: bold;
}
.grid-skill {
  display: grid;
  grid-template-columns: auto auto auto;
  padding: 1rem;
  margin: 1;
  text-align: center;
  
}
.logo {
  width: 9rem;
  height: 7.5rem
}
.skill{
  margin:1.5rem;

}
.skill h5
.timeline-items{
  max-width: 40rem;
  margin: auto;
  display: flex;
  flex-wrap:wrap ;
  position: relative;
}
.timeline-items::before{
  content: '';
  position: absolute;
  width: 0.2rem;
  height: 20rem;
  background-color:#ABC9FF;
  left: calc(50% - 0.1rem);
 
}

.timeline-item{
  
  margin-bottom: 3rem;
  width: 100%;
  position: relative;
}
.timeline-item:last-child{
  margin-bottom: 0;
}
.timeline-item:nth-child(odd){
  padding-right: calc(50% + 3rem);
}
.timeline-item:nth-child(even){
  padding-left: calc(50% + 1rem);
}
.timeline-dot{
  height: 1rem;
  width: 1rem;
  background-color:#ABC9FF;
  position: absolute;
  left:calc(50% - 0.5rem);
  border-radius: 50%;
  top: 10px;
}
.timeline-date{
  font-size: 1rem;
  margin:1rem 0 1rem ;
  font-style: italic;
}

.timeline-content h4{
  border-color: black;
  font-size: 1rem;
  font-weight: bold;
  border-radius: 0.5rem;
}
h2{
  text-align: center;
  margin: 1.5rem;
  text-decoration: underline;
}
@media (width: 300px){
  .cap{
    font-size: 2rem !important;

  }
  .grid-skill {
  display: grid;
  grid-template-columns: auto auto;
  margin: 0;
  padding: 0;

  }
  .logo{
    width: 4rem;
    height: 3.5rem;
  }
  .timeline-date{
    font-size: 0.8rem;
  }
  .timeline-content h4{
    font-size: 0.8rem ;
    margin:0.2rem 0 0.2rem ;
  }
  .timeline-content p{
    font-size: 0.6rem !important;
  }
  .educationlist li{
    font-size: 0.8rem !important;
    padding: 0.1rem;

  }
  .timeline-items::before{
    height: 30rem;
  }
 
  

}
</style>