<template>
    <div container-fluid>
        <img
          src="https://i.postimg.cc/xC3g1HmH/banner.jpg"
          class="img-fluid position-relative"
          alt="banner"
          style="width: 100%; height: 100%;"
        />

        <div class="heading">
          <h2>Thokozani Nqwili</h2>
          <p>An Aspiring <span>Web Developer </span></p>
        </div>
      </div>
   

</template>

<style>

.heading{
    position: absolute;
    top: 30%;
    padding-left: 10rem;
}
.heading p{
    font-size: 1.5rem;
    margin-left: 3.5rem ;
    margin-top: 1rem;
    overflow: hidden;
    border-right: .15em solid black;
    white-space: nowrap;
    margin: 0 auto;
    letter-spacing: .15em;
    animation: typing 5s steps(40, end),
    blink-caret .75s step-end infinite;
    animation-iteration-count: infinite;

}
.heading span{
    color: #FA9494;
    font-size: 35px;
    font-weight: bold;
   
}


@keyframes typing {
        0% { width: 0 }
        50% { width: 100% }
      }



@keyframes blink-caret {
        from, to { border-color: transparent }
        50% { border-color:black; }
      }
.heading h2{
 font-size: 60px;
}

</style>