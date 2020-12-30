<template>
  <body>
    <div id="wrapper">
      <div id="header">
        <a href="#">ホームページに設定する</a>
        
        <a href="#">Yahoo!BB</a><small>|</small>
        <a href="#">きっず版</a><small>|</small>
        <a href="#">アプリ版</a><small>|</small>
        <a href="#">ヘルプ</a>

        <hr>



      </div>

      <div id="main">
        
      </div>
    </div>





    
  </body>

</template>
<script>

export default {
  name: 'App',
  
}
</script>
<style>

/* body{
  background-color: black;
  width: 974px;
  margin: 0 auto;
}

#contents{
  background-color: yellow;
  width: 500px;
  margin: 0 auto;

} */

#wrapper{
  margin-left: auto;
  margin-right: auto;
  width: 60em
}

/* .header a:nth-of-type(1){
} */

#header a:link, a:visited,
#header hr {
  color: #4000ff;
  text-decoration:none;
}


#header small{
  color: black;
  font-size: 100%;
  margin-left: 0.25em;
}
#header a:nth-of-type(2){
  margin-left: 30em;
}
#header a:nth-of-type(3){
  margin-left: 0.5em;
}
#header a:nth-of-type(4){
  margin-left: 0.5em;
}
#header a:nth-of-type(5){
  margin-left: 0.5em;
}

</style>
