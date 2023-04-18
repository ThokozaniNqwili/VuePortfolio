<template>
  <div class="testimonial">
    <h1>Testimonials</h1>
    <div class="row">
      <div class="col-6 col-sm-4" v-for="item in items">
        <div class="card">
          <img
            :src="item.img"
            class="card-img-top img-fluid"
            alt="Image"
            style="height: 22rem"
          />
          <div class="card-body">
            <h3 class="card-title">{{ item.name }}</h3>
            <h5>{{ item.relation }}</h5>
            <p class="card-text">{{ item.message }}</p>
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
          name: "Oslin Johnson",
          img: "https://i.postimg.cc/xCRd46mZ/oslin2.png",
          relation: "Life Choices Academy Lecturer",
          message:
            "Thokozani is a very diligent person with the will to push herself to attain her goals to the best of her ability and to her satisfaction. She doesn't let anything get her down and always makes it her duty to find how she will understand things",
        },
        {
          name: "Duwayne Jewell",
          img: "https://i.postimg.cc/qqTGdvx6/duwayne.jpg",
          relation: "iStore Manager",
          message:
            "Throughout the time with our organization, she demonstrated critical skills that would make her an excellent employee at any company.Thokozani did a terrific job in her position and was an asset to our Support team",
        },
        {
          name: "Tsepang Matebese",
          img: "https://i.postimg.cc/VLSXHM8Z/tsepang.jpg",
          relation: "Friend",
          message:
            "Thokozani is a hardworking, diligent worker. She never gives upon difficult tasks, she always strives to achive the best results.When met with opportunities, she tries to maximise on them & she is not afraid to try things outside of her comfort zone",
        },
        {
          name: "Buhle Qampi",
          img: "https://i.postimg.cc/NM9rPvh9/Buhle.jpg",
          relation: "Life Choices Academy Peer",
          message:
            "Thoko's work is exceptionally well curated. Her code is neat and coherent. She's a team player and a good addition to any workplace",
        },
        {
          name: "Phelo Madubela",
          img: "https://i.postimg.cc/LshTR7KR/phelo.jpg",
          relation: "Former iStore Colleague",
          message:
            "Thokozani is a young dedicated individual with a positive mindset. I got to see this because we worked together, her work ethic is impeccable. She always willing to help and learn, she works with a smile on her face. She's definetly loyal, trustworthy and reliable",
        },
        {
          name: "Ryan Thomas",
          img: "https://i.postimg.cc/gjVHQFsW/ryan2.jpg",
          relation: "Life Choices Academy Lecturer",
          message:
            "Thokozani is someone who refuses to give up or take a loss. She always strives to deliver her utmost best and it shows in her work ethic as well as the results of what she delivers.",
        },
      ],
    };
  },
};
</script>

<style>
.card {
  padding: 0.5rem;
  margin: 0.8rem;
  width: 23rem;
  height: 40rem;
 
}
@media screen and (min-width: 300px) and (max-width: 719px) {
  .row {
    display: grid !important;
    grid-template-columns: auto !important;
    margin: 0 !important;
  }
  .card {
    width: 14rem;
    height: 22rem;
    font-size: 56%;
    margin: 0.5rem;
    padding: 0.3rem;
  }
  .card-body h3 {
    font-size: 0.9rem;
  }
  .card-body h5 {
    font-size: 0.9rem;
  }

  .card-img-top {
    height: 11rem !important;
  }
}
@media screen and (min-width: 720px) and (max-width: 1079px) {
  .row {
    display: grid !important;
    grid-template-columns: auto auto !important;
    margin: 0 !important;
  }
  .card {
    width: 18rem;
    height: 30rem;
    font-size: 72%;
    margin: 0.5rem;
    padding: 0.3rem;
  }
  .card-body h3 {
    font-size: 1.2rem;
  }
  .card-body h5 {
    font-size: 1.2rem;
  }

  .card-img-top {
    height: 16rem !important;
  }
}
@media screen and (min-width: 1080px) and (max-width: 1495px) {
  .row {
    margin: 0;
  }
  .card {
    padding: 0.4rem;
    margin: 0.8rem;
    font-size: 85%;
    width: 20rem;
    height: 34rem;
  }
  .card-body h3 {
    font-size: 1.3rem;
  }
  .card-body h5 {
    font-size: 1.3rem;
  }
  .card-img-top {
    height: 18rem !important;
  }
}
</style>
