<template>
  <div class="bg">
   
    <!-- <div class="icon">BrainForce</div>
    <pre class="tagline">
        Take control!
    </pre> -->

    <div class="content">
      <h1>Our mission</h1>
      <div class="flex-container">
        <div class="msg">
          More than <span class="emphasis"><b>4 million</b></span> americans cannot use their hands or fingers to operate a touchscreen, keyboard or mouse.
          Our mission at <span class="inline-icon">BrainForce</span> is to empower them with <span class="emphasis"><b>hands-free</b></span> operation of computers and smartphones.
        </div>
        <img class="image float-right" :src="require(`../assets/Picture3.png`)">
      </div>
      <br>
      <hr>
      <!---------------------------------------------------------------------------------------------->
      <h1>Head Mouse</h1>
      <div class="flex-container">
        <img class="image float-right" :src="require(`../assets/Picture1.png`)">  
        <div class="msg">
          Select any <span class="inline-icon">BrainForce</span> device.
          Do you wear prescription glasses? Why not use <span class="inline-icon">BrainForce</span> glasses!
          Don't want glasses? We have earbuds too!
          Both have special motion sensors for tracking user's head movements.
        </div>
        <div class="msg">
          Wear any device and control the mouse cursor with your head. Look up to move the cursor up, look down to move the cursor down.
          It's like magic!
        </div>
        <img class="image float-right" :src="require(`../assets/Picture2.png`)">
      </div>
      <hr>
      <!---------------------------------------------------------------------------------------------->
      <h1>Want to try it out?</h1>
      <div class="flex-container">
        <div class="msg">
          Sign up for a demo today! Either fill out the form below or reach out to us at:
          <ul>
            <li><a href="mailto:parthshah@brainforce.us">parthshah@brainforce.us</a></li>
            <li><a href="mailto:mohitpatil@brainforce.us">mohitpatil@brainforce.us</a></li>
          </ul>
        </div>      
      </div>
      <br>
      <br>
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdxhVYFVfOgdrkV48Mt5FEHtOUvk6_XwhyupsekxMf6H9wh1Q/viewform?embedded=true" width="640" height="1000" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
      
    </div>
    
    <!-- <div class="msg">
      Coming soon..
    </div>
    <a class="button" href="http://demo.brainforce.us/">
      Try our demo
    </a> -->
    
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Lobster&display=swap');

$title-bar-padding: 15px;
$title-font-size: 40px;
$box-shadow: 0 5px 20px rgba(0,0,0,0.19), 0 3px 6px rgba(0,0,0,0.23);
$box-shadow-highlight: 0 5px 30px rgba(0,0,0,0.19), 0 3px 15px rgba(0,0,0,0.23);
$content-padding: 40px;
$orange: #f46524;

.bg{
  height: 100%;
  text-align: center;
  // background-color: #fc5603;
  font-family:  Arial, Helvetica, sans-serif;
}
.inline-icon{
  font-family: 'Lobster', cursive;
  color: $orange;
}
// .icon{
//   font-family: 'Lobster', cursive;
//   font-size: 7rem;
//   color: #fc5603;
// }
// .tagline{
//   color: #fc5603;
//   font-style: italic;
//   font-size: 2rem;
// }
.content{
  padding: $content-padding;
  margin: auto;
  margin-top: ($title-font-size + 2*$title-bar-padding - $content-padding);
}
h1{
  color: $orange;
  font-family: "Courgette";
  font-size: 3rem;
}
.emphasis{
  color: $orange;
  font-size-adjust: 2;
}
.msg{
  // display: inline;
  text-align: justify;
  text-justify: inter-word;
  font-size: 1.2rem;
  max-width: 400px;
  margin: 10px;
}
a{
  color: $orange;
}
.image{
  width: 100%;
  max-width: 600px;
}
$btn-color: #673AB7;
.button{
  text-decoration: none;
  width: max-content;
  margin: 20px auto;
  display: block;
  border-radius: 20px;
  box-shadow: $box-shadow;
  color: white;
  border: 2px solid $btn-color;
  background-color: $btn-color;
  transition: 0.3s;
  padding: 8px 10px;
  cursor: pointer;
  -webkit-user-select: none;  /* Chrome all / Safari all */
  -moz-user-select: none;     /* Firefox all */
  -ms-user-select: none;      /* IE 10+ */
  user-select: none;    
  font-size: 1.2rem;

  &:hover{
    border: 2px solid $btn-color;
    background-color: #EDE7F6;
    color: #512DA8;
    box-shadow: $box-shadow-highlight;
  }
  &:active{
    background-color: #B39DDB;
  }
  &:focus{
    outline: none;
  }
}
</style>
