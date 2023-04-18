<template>
  <div class="about">
    <h1>About Me</h1>

    <div class="container">
      <div class="row">
        <div class="col-sm-4">
          <img
            class="img-fluid rounded w-65"
            src="https://i.postimg.cc/qB8hjz3G/my-Picture.jpg"
            alt="MyPicture"
          />
        </div>

        <div class="col-sm-8 fs-6">
          <h3>Web Developer</h3>
          <p>
            I am a goal-driven Information Systems Graduate from the University
            of Cape Town, I have passion for programming. I have the
            skills and training needed to help develop and maintain software
            programs and to make improvements that will enhance functionality. I
            have outstanding problem-solving skills with the ability to
            troubleshoot technical issues.My good qualities also include strong
            communication with the ability to work directly with
            clients,willingness to learn new programming language and innovative
            mindset.
          </p>
          <br />
         
          

          <div class="row row-cols-2 fs-6">
            <div class="col">Name: Thokozani Nqwili</div>
            <div class="col">Birthday: 20 August 1999</div>
            <div class="col">Degree: Bcom Information Systems</div>
            <div class="col">Phone: 0812326542</div>
            <div class="col">Email: simthokozile@gmail.com</div>
            <div class="col">Address: Khayelitsha,Cape Town</div>
            <div class="col">Driver's license: Yes</div>
            <div class="col">Willing to relocate: Yes</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.about h3 {
  font-size: 2.5rem;
  text-align: center;
  margin: 1rem;
}
.container {
  margin-bottom: 2rem;
}
@media screen and (min-width: 300px) and (max-width: 719px) {
  .col-sm-8 p {
    font-size: 0.8rem !important;
  }
  .row {
    font-size: 0.8rem !important;
  }
  .col-sm-8 h3 {
    font-size: 1.2rem;
  }
}
@media screen and (min-width: 720px) and (max-width: 1079px) {
  .col-sm-8 p {
    font-size: 0.8rem !important;
  }
  .row {
    font-size: 0.8rem !important;
  }
  .col-sm-8 h3 {
    font-size: 1.3rem;
  }
}
</style>
