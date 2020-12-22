<template>
  <div class="bg">
    <div class="heading">BrainForce</div>
    <pre class="tagline">
        Just look...
        &emsp;&emsp;&emsp;&emsp;  ... and think!
    </pre>
    <div class="msg">
      Coming soon..
    </div>
    <a class="button" href="http://demo.brainforce.us/">
      Try our demo
    </a>
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

$padding: 120px;
$box-shadow: 0 5px 20px rgba(0,0,0,0.19), 0 3px 6px rgba(0,0,0,0.23);
$box-shadow-highlight: 0 5px 30px rgba(0,0,0,0.19), 0 3px 15px rgba(0,0,0,0.23);

.bg{
  height: 100%;
  text-align: center;
  background-color: #fc5603;
  font-family:  "Lucida Grande", sans-serif;
}
.heading{
  padding-top: $padding;
  height: calc(100% - $padding);
  font-family: 'Lobster', cursive;
  font-size: 7rem;
  color: white;
}
.tagline{
  color: white;
  font-style: italic;
  font-size: 2rem;
}
.msg{
  
  font-size: 1.5rem;
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
