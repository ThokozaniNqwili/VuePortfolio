<template>
  <div container-fluid>
    <img
      src="https://i.postimg.cc/SNtSLXyB/banner2.png"
      class="img-fluid banner position-relative"
      alt="banner"
      style="width: 60%; height: 60%"
    />

    <div class="heading">
      <div class="name">Thokozani Nqwili</div>
      <div class="position">Web Developer</div>
      <ul class="social_icon">
        <a href="https://www.linkedin.com/in/thokozani-nqwili-5b5a8517a"
          ><i class="fab fa-linkedin-in fa-bounce"></i
        ></a>
        <a href="https://www.instagram.com/_thokzin/"
          ><i class="fab fa-instagram fa-bounce"></i>
        </a>
        <a href="https://github.com/ThokozaniNqwili"
          ><i class="fa-brands fa-github fa-bounce"></i
        ></a>
      </ul>
    </div>
  </div>
</template>

<style>
.container-fluid {
  width: 100%;
  height: 100%;
}
.banner {
  transform: translateX(25rem);
}

.social_icon {
  margin-left: 9rem;
  margin-top: 2rem;
  display: flex;
  align-items: center;
  position: relative;
  display: flex;
  align-items: center;
}
.social_icon a {
  font-size: 2em;
  color: #067814;
  margin: 0 1rem;
  display: inline-block;
  transition: 0.5s;
}
.position {
  font-size: 1.9rem;
  margin-left: 1rem;
  margin-top: 0.5rem;
  overflow: hidden;
  white-space: nowrap;
  margin: 0 auto;
  letter-spacing: 0.1em;
  animation: typing 5s steps(40, end), blink-caret 0.75s step-end infinite;
  animation-iteration-count: infinite;
}
@keyframes typing {
  0% {
    width: 0;
  }
  50% {
    width: 100%;
  }
}

@keyframes blink-caret {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: black;
  }
}

.name {
  font-weight: bold;
  position: relative;
  display: block;
  font-size: 4rem;
  text-shadow: 0 0.1rem 0.2rem #0b0bc4;
  transition: all 0.3s ease-in-out;
}

.name::after {
  content: "";
  position: absolute;
  z-index: 1;
  font-size: 3.5rem;
  opacity: 0;
  text-shadow: 0 0.5rem 1.5rem #0b0bc4;
  transition: opacity 0.3s ease-in-out;
}

.make-it-fast {
  text-shadow: 0 0.2rem 0.4rem #0b0bc4;
}

.make-it-fast::after {
  text-shadow: 0 0.5rem 1.5rem #0b0bc4;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.make-it-fast:hover::after {
  opacity: 1;
}

.name:hover {
  transform: scale(1.1, 2);
  margin: 1.2rem;
}

.name:hover::after {
  opacity: 1;
}

.heading {
  transform: translateY(-28rem);
  padding-left: 8rem;
}

@media screen and (min-width: 300px) and (max-width: 719px) {
  .heading {
    transform: translateY(-5.5rem);
    padding-left: 0.9rem;
  }

  .name {
    font-size: 1.1rem;
  }
  .position {
    font-size: 0.54rem;
  }
  .social_icon a {
    font-size: 1em;
  }
  .social_icon {
    margin-top: 0.5rem;
    margin-left: 1.2rem;
  }
  .social_icon a {
    margin: 0 0.3rem;
  }
  .name:hover {
    transform: scale(1.1, 1.3);
    margin: 0.4rem;
  }
  .banner {
    transform: translateX(6.5rem);
  }
}
@media screen and (min-width: 720px) and (max-width: 1079px) {
  .banner {
    transform: translateX(14rem);
  }
  .heading {
    transform: translateY(-13rem);
    top: 10%;
    padding-left: 3rem;
  }
  .name {
    font-size: 2.5rem;
  }
  .position {
    font-size: 1.23rem;
  }
  .social_icon {
    margin-top: 0.8rem;
    margin-left: 4em;
  }
}
@media screen and (min-width: 1080px) and (max-width: 1495px) {
  .heading {
    transform: translateY(-20rem);
    top: 10%;
    padding-left: 3rem;
  }
}
</style>
