<template>
  <div>
    <footer>
      <ul class="social_icon text-center">
        <a href="https://www.linkedin.com/in/thokozani-nqwili-5b5a8517a" target="blank"
          ><i class="fab fa-linkedin-in"></i
        ></a>
        <a href="https://www.instagram.com/_thokzin/" target="blank"
          ><i class="fab fa-instagram"></i>
        </a>
        <a href="https://github.com/ThokozaniNqwili" target="blank"
          ><i class="fa-brands fa-github"></i
        ></a>
      </ul>
      <ul class="menu text-center">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#">Resume</a></li>
        <li><a href="#">Testimonials</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
      <p>&copy;2023 Thokozani Nqwili | All Rights Reserved</p>
    </footer>
  </div>
</template>

<style>
footer {
  position: relative;
  background-color: #eb1d36;
  min-height: 10%;
  width: auto;
  padding: 1em 3em;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-align: center;
}

footer .social_icon,
footer .menu {
  position: relative;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
footer .social_icon a {
  font-size: 1.5em;
  color: #f5eddc;
  margin: 0 10px;
  display: inline-block;
  transition: 0.5s;
}
footer .social_icon a:hover {
  transform: translateY(-10px);
}
footer .menu li {
  list-style: none;
}
footer .menu li a {
  font-size: 1.2em;
  color: #f5eddc;
  margin: 0 1em;
  display: inline-block;
  text-decoration: none;
  opacity: 0.75;
}
footer .menu li a:hover {
  opacity: 1;
}
footer p {
  color: #f5eddc;
  text-align: center;
  margin-top: 15px;
  margin-bottom: 10px;
  font-size: 0.7em;
}
@media screen and (min-width: 300px) and (max-width: 720px) {
  footer .menu {
    display: grid;
    grid-template-columns: auto auto auto;
  }
  footer .menu li a {
    font-size: 0.8em;
  }
}
</style>
