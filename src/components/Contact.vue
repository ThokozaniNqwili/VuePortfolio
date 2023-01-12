<template>
  <div class="contact">
    <h1>Contact Me</h1>
    
    <div class="container">
      <div class="row">
        <div class="col-sm-8">
          <form action="https://formspree.io/f/myyvbwyw" method="POST">
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label"
                >Name</label
              >
              <input
                type="text"
                class="form-control"
                id="exampleFormControlInput1"
                placeholder="Name and Surname"
                name="Name"
                required
              />
            </div>
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label"
                >Email_address</label
              >
              <input
                type="email"
                class="form-control"
                id="exampleFormControlInput1"
                placeholder="Email Address"
                name="email"
                required
              />
            </div>
            <div class="mb-3">
              <label for="exampleFormControlInput1" class="form-label"
                >Phone Number</label
              >
              <input
                type="number"
                class="form-control"
                id="exampleFormControlInput1"
                placeholder="+27 82 656 5465"
                name="number"
              />
            </div>
            <div class="mb-3">
              <label for="exampleFormControlTextarea1" class="form-label"
                >Message</label
              >
              <textarea
                class="form-control"
                id="exampleFormControlTextarea1"
                rows="5"
                name="message"
              ></textarea>
            </div>

            <div class="col-auto">
              <button
                type="submit"
                class="btn"
                data-bs-toggle="modal"
                data-bs-target="#messageModal"
              >
                Send Message
              </button>
            </div>
          </form>
        </div>
        <div class="col-md-4">
          <div class="icons">
            <div class="row">
              <div class="col-sm-4">
                <i class="fas fa-phone" style="font-size: 36px"></i>
              </div>
              <div class="detail col-sm-8 fs-6">Call me on:+27 81 232 6542</div>
            </div>

            <div class="row">
              <div class="col-sm-4">
                <i class="far fa-envelope-open" style="font-size: 36px"></i>
              </div>
              <div class="detail col-sm-8 fs-6">simthokozile@gmail.com</div>
            </div>

            <div class="row">
              <div class="col-sm-4">
                <i class="fas fa-map-marker-alt" style="font-size: 36px"></i>
              </div>
              <div class="detail col-sm-8 fs-6">Khayelitsha, Cape Town</div>
             
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  
</template>

<style>
.contact p {
  font-size: 4.5rem;
  padding: 1rem;
  font-style: italic;
}
.contact .detail {
  font-weight: bold;
  padding-top: 3rem;
}
.contact .icons {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.contact .icons i {
  font-size: 2em;
  color: #eb1d36;
  margin: 0 1rem;
  display: inline-block;
  transition: 0.5s;
  padding: 1.5rem;
}
.contact .btn {
  border: 1px solid transparent;
  background-color: #eb1d36;
  border-radius: 1rem;
  justify-content: space-between;
  padding: 1rem;
  margin-right: 0.5rem;
  margin-top: 1rem;
  margin-bottom: 2rem;
  color: #f5eddc;
}
</style>
