<template>
    <div class="container">
        <h1>Testimonials</h1>
        <div class="row">
          <div class="col-6 col-sm-4" v-for="item in items">

            <div class="card">
                <img :src="item.img" class="card-img-top" alt="Image" style="height:24rem;">
                <div class="card-body">
                  <h3 class="card-title">{{item.name}}</h3>
                  <h5>{{item.relation}}</h5>
                  <p class="card-text">{{item.message}}</p>
                  
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
        items: [
            {
                name:"Oslin Johnson",
                img: "https://i.postimg.cc/L8wCbRwL/Oslin.jpg",
                relation: "Lecturer",
                message:"Thokozani is a very diligent person with the will to push herself to attain her goals to the best of her ability and to her satisfaction. She doesn't let anything get her down and always makes it her duty to find how she will understand things"

            },
            {
                name:"Duwayne Jewell",
                img: "https://i.postimg.cc/qqTGdvx6/duwayne.jpg",
                relation: "iStore Manager",
                message:  "Throughout the time with our organization, she demonstrated critical skills that would make her an excellent employee at any company.Thokozani did a terrific job in her position and was an asset to our Support team"
                
            },
            {
                name:"Tsepang Tihoeng-Matebese",
                img:"https://i.postimg.cc/VLSXHM8Z/tsepang.jpg",
                relation:"Friend",
                message:"Thokozani is a hardworking, diligent worker. She never gives upon difficult tasks, she always strives to achive the best results.When met with opportunities, she tries to maximise on them & she is not afraid to try things outside of her comfort zone"

            },
            {
                name:"Buhle Qampi",
                img: "https://i.postimg.cc/NM9rPvh9/Buhle.jpg",
                relation:"Life Choices Academy Peer",
                message:"Thoko's work is exceptionally well curated. Her code is neat and coherent. She's a team player and a good addition to any workplace"

            },
            {
                name:"Phelo Madubela",
                img: "https://i.postimg.cc/LshTR7KR/phelo.jpg",
                relation:"Former Colleague",
                message:"Thokozani is a young dedicated individual with a positive mindset. I got to see this because we worked together, her work ethic is impeccable. She always willing to help and learn, she works with a smile on her face. She's definetly loyal, trustworthy and reliable"


            },
            {
                name:"Uzukhanye Dywili",
                img:"https://i.postimg.cc/nzFTgzFR/Uzukhanye.jpg",
                relation:"Life Choices Academy Peer",
                message:""
            }

        ]     
    }
  },
}
</script>

<style>
.card{
    padding: 0.5rem;
    margin:1rem;
    width: 23rem;
    height:40rem;
}
@media (width: 300px){
    .card{
        width: 15rem;
        height:50%;
        font-size: 50%;
        margin: 0;
        padding: 0.1rem;
    }
    h3{
        font-size: 90%;
    }
    h5{
        font-size: 90%;
    }

}
    

</style>

