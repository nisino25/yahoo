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
      <div id="masterHead">
        <ul class="row"><!-- 1st three logos -->

          <li class="item">
            <img src="https://images.vexels.com/media/users/3/128931/isolated/preview/c8701214b16da5fc13b83946691e8b27-travel-bag-icon-by-vexels.png" alt="Girl in a jacket" >
            <a href="#" class="caption">トラベル</a>
          </li>
          <li class="item">
            <img src="https://png.pngtree.com/png-vector/20190704/ourlarge/pngtree-hammer-judge-icon-png-image_1541693.jpg" alt="Girl in a jacket" >
            <a href="#" class="caption">ヤフオク！</a>
          </li>
          <li class="item">
            <img src="https://cdn.iconscout.com/icon/premium/png-256-thumb/shopping-cart-71-543136.png" alt="Girl in a jacket" >
            <a href="#" class="caption">ショッピング</a>
          </li>

          <li>
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b5/Yahoo_Japan_Logo.svg/1280px-Yahoo_Japan_Logo.svg.png" alt="Girl in a jacket" width="200" height="75">
          </li>

          <li class="item">
            <img src="https://cdn3.iconfinder.com/data/icons/currency-2/460/Yen-512.png" alt="Girl in a jacket" >
            <a href="#" class="caption">PayPay</a>
          </li>
          <li class="item">
            <img src="https://thumbs.dreamstime.com/b/credit-card-icon-flat-style-illustration-vector-web-79711478.jpg" alt="Girl in a jacket" >
            <a href="#" class="caption">カード</a>
          </li>
          <li class="item">
            <img src="https://cdn.iconscout.com/icon/premium/png-256-thumb/shopping-cart-71-543136.png" alt="Girl in a jacket" >
            <a href="#" class="caption">メール</a>
          </li>

          
          
        </ul>

       

        <!-- <div>last three logos
          <img src="https://cdn3.iconfinder.com/data/icons/currency-2/460/Yen-512.png" alt="Girl in a jacket" width="75" height="75">
          <img src="https://thumbs.dreamstime.com/b/credit-card-icon-flat-style-illustration-vector-web-79711478.jpg" alt="Girl in a jacket" width="75" height="75">
          <img src="https://i.pinimg.com/564x/1f/5c/79/1f5c79832b4d0fddf889e3fc956a992c.jpg" alt="Girl in a jacket" width="75" height="75">
        </div> -->

      </div>
      <section id="search">
        <ul class='row'>
          <li>ウェブ</li>
          <li>画像</li>
          <li>動画</li>
          <li>知恵袋</li>
          <li>地図</li>
          <li>リアルタイム</li>
          <li>一覧</li>
        </ul>

        <form>
          <input type="text" placeholder="検索" name="name" maxlength="300" class="input">
          <button>検索</button>
        </form>

      </section>

      <div id="topLink"></div>

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

ul {
  list-style-type: none;
}


#wrapper{
  margin-left: auto;
  margin-right: auto;
  width: 60em
}

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


#masterHead li:nth-of-type(1),
#masterHead li:nth-of-type(2),
#masterHead li:nth-of-type(5),
#masterHead li:nth-of-type(6){
  margin-right: 1em;
}

#masterHead li:nth-of-type(1){
  margin-left: 5em;
}
#masterHead li:nth-of-type(3),
#masterHead li:nth-of-type(4){
  margin-right: 1em;
}
.row{
  display: flex;
}
li.item {
  margin-top: -0.5em;
  /* width: 1em; */
  /* flex: 1; additionally, equal width */
  padding: 0.5em;
}
.item img{
  width: 50px;
  height: 50px;
}
.caption {
  font-size: 75%;
  margin-top: -0.5em;
  display: block;
}



#search{
  background-color: #f1f5ff;
  width: 52em;
  /* height: 20em; */
  border: 5px solid #beccea;
  padding: 1.5em;
  
  margin: 25px;
}

#search li{
  margin-top: -2.5rem;
  font-size: 115%;
  color: #4682B4;
}

#search li:nth-of-type(1){
  margin-left: 3rem;
  color: black;
}

#search li:nth-of-type(1),
#search li:nth-of-type(2),
#search li:nth-of-type(3),
#search li:nth-of-type(4),
#search li:nth-of-type(5),
#search li:nth-of-type(6),
#search li:nth-of-type(7){
  margin-right: 1em;
}

/* #emptyBox{
  background-color: white;
  width: 60%;
  border: 5px solid grey;
  padding: 20px;
  margin-top: -40px;
  margin-left: 5rem;
} */

#search form{
  margin-top: -1em;
}

input[type=text] {
  margin-top: -10em;
  margin-left: 6em;
  width: 38em;
  height: 2em;
  border: 2px solid grey;
  border-radius: 0px;
}

#search button{
  width: 10em;
  height: 2em;
  margin-left: 1em;
  border-radius: 0px;
  background-color: #0080ff;
}






</style>
