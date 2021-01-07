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
      <div id="topLink">
        <a href="#">PayPayモール「WINTER ZOZOSALE」開催中</a>
        <a href="#">ご当地テレビ 全国の放送局の番組をお届け</a>
      </div>


      <div id="main">
        <div class="col-1 col"><!-- left -->
          <ul class="left1">
            <li>ショッピング</li>
            <li>PayPayモール</li>
            <li>ヤフオク！</li>
            <li>PayPayフリマ</li>
            <li>ZOZOTOWN</li>
            <li>LOHACO</li>
            <li>トラベル</li>
            <li>一休.com</li>
            <li>一休.comレストラン</li>
            <li>ニュース</li>
            <li>天気・災害</li>
            <li>スポーツナビ</li>
            <li>フィナンス</li>
            <li>テレビ</li>
            <li>映画</li>
            <li>GYAO!</li>
            <li>ゲーム</li>
            <li>Yahoo!モバゲー</li>
            <li>ebookjapan</li>
            <li>占い</li>
            <li>地図</li>
            <li>路線情報</li>
            <li>Retty</li>
            <li>クラシル</li>
            <li>不動産</li>
            <li>自動車</li>
            <li>TRILL</li>
            <li>パートナー</li>
            <li>サービス一覧</li>
          </ul>

          <ul class="left2">
            <li><strong>ビジネスで活用するなら</strong></li>
            <li>スマホ経済を無料で導入</li>
            <li>Yahooに広告を出そう</li>
            <li>ネットショップ開業無料</li>
            <li>データで生活者分析</li>
            <li>Tポイント提携店募集</li>
          </ul>

          <ul class="left3">
            <li><strong>社会的な取組</strong></li>
            <li>ネット募金</li>
            <li>ボランティア</li>
            <li>エールマーケット</li>
            <li>Yahoo!基金で支援助生</li>
          </ul>

          <ul class="left4">
            <li><strong>ヤフーからのお知らせ</strong></li>
            <li>「ポテンシャル採用」の応募を受付中</li>
          </ul>
        </div> 

        <div class="col-2 col">
          <ul class="middle1">
            <div class="navbar"><!-- changing tab here -->
              <button :class="[tabSelected === 'news' ? 'selected': 'notSelected']" @click="changeTab('news')">ニュース</button>
              <button :class="[tabSelected === 'economy' ? 'selected': 'notSelected']" @click="changeTab('economy')">経済</button>
              <button :class="[tabSelected === 'enttertainment' ? 'selected': 'notSelected']" @click="changeTab('enttertainment')">エンタメ</button>
              <button :class="[tabSelected === 'sports' ? 'selected': 'notSelected']" @click="changeTab('sports')">スポーツ</button>
              <button :class="[tabSelected === 'domestic' ? 'selected': 'notSelected']" @click="changeTab('domestic')">国内</button>
              <button :class="[tabSelected === 'international' ? 'selected': 'notSelected']" @click="changeTab('international')">国際</button>
              <button :class="[tabSelected === 'science' ? 'selected': 'notSelected']" @click="changeTab('science')">IT・科学</button>
              <button :class="[tabSelected === 'local' ? 'selected': 'notSelected']" @click="changeTab('local')">地域</button>
              <!-- :class="[(tabSelected = 'economy') ? selected:notSelected]" -->
            </div>
            <div class="content">
              <small>1/6（水）18:42更新</small>
              <ul v-if="tabSelected === 'news'"><!-- news -->
                <li><a href="#">国内間５７００人</a></li>
                <li><a href="#">緊急宣言</a></li>
                <li><a href="#">千葉３１１人</a></li>
              </ul>

              <ul v-if="tabSelected === 'economy'"><!-- economy -->
                <li><a href="#">ANAとJAL結構</a></li>
                <li><a href="#">雇用助成金特例</a></li>
                <li><a href="#">店舗ごと１日６万円</a></li>
              </ul>

              <ul v-if="tabSelected === 'enttertainment'"><!-- entertainment  -->
                <li><a href="#">YOUTUBEヒット曲の変化</a></li>
                <li><a href="#">大泉洋 紅白司会割れる評価</a></li>
                <li><a href="#">中村倫衝撃</a></li>
              </ul>

              <ul v-if="tabSelected === 'sports'"><!-- sports -->
                <li><a href="#">西武ドラ 体重１１８kgで入寮</a></li>
                <li><a href="#">アーモンドアイ 年度代表馬に</a></li>
                <li><a href="#">白血病の北別府氏 コロナ怖い</a></li>
              </ul>

              <ul v-if="tabSelected === 'domestic'"><!-- domstic -->
                <li><a href="#">国会議員の会食 ルール作庭へ</a></li>
                <li><a href="#">大雪や猛吹雪警戒 警戒発表</a></li>
                <li><a href="#">平成表記 免許うっかり失効も</a></li>
              </ul>

              <ul v-if="tabSelected === 'international'"><!-- international -->
                <li><a href="#">金氏 党大会で経済不振認める</a></li>
                <li><a href="#">トランプ氏 私の圧勝だった</a></li>
                <li><a href="#">米グラミー賞 コロナで延期</a></li>
              </ul>

              <ul v-if="tabSelected === 'science'"><!-- local -->
                <li><a href="#">米、中国アリペイなどを禁止</a></li>
                <li><a href="#">国産ワクチン開発 実用まだ</a></li>
                <li><a href="#">寒い冬 快適な睡眠のコツは？</a></li>
              </ul>

              <ul v-if="tabSelected === 'local'"><!-- science -->
                <li><a href="#">都１５９１人感染</a></li>
                <li><a href="#">女性遺棄 殺人容疑で再逮捕</a></li>
                <li><a href="#">愛知緊急宣言</a></li>
              </ul>
              <li class="bottomList"><a href="#">もっと見る</a></li>
              <li class="bottomList"><a href="#">トピックス一覧</a></li>


            </div>
          </ul>
          <ul class="middle2">
            <strong>緊急事態宣言 小池知事が臨時会見</strong>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/oYE2aCTDKVs" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen ></iframe>
            <span>映像提供:THE PAGE</span>
          </ul>

        </div> <!-- middle -->


        <div class="col-3 col"><!-- right -->
          <div class="ads">
            <img src="https://s.yimg.jp/bdv/yahoo/20191008test/0b9cc53336_350x240_shopping_24htimesale_2.png" style="width:20.5em">
          </div>
          <div class='covid'><!-- covid -->
            <img src="https://s.yimg.jp/images/yjtop/hazard/coronavirus/2021/infected/pc0107_03.png" style="width:20.5em">  
          </div>

          <div class='widget'><!-- login and weather -->
            <span>ログイン[ID取得]</span>
            <button>登録情報</button>
            
            <div class="login">
              <div>
                <ul class="row">
                  <li class="loginItem">
                    <img src="https://p7.hiclipart.com/preview/663/97/225/email-computer-icons-message-bounce-address-email-icon.jpg" >
                    <a href="#" class="loginCaption">メール</a>
                  </li>
                  <li class="loginItem">
                    <img src="https://cdn.iconscout.com/icon/premium/png-512-thumb/t-letter-1-840447.png">
                    <a href="#" class="loginCaption">ポイント確認</a>
                  </li>
                  <li class="loginItem">
                    <img src="data:image/jpeg;base64,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">
                    <a href="#" class="loginCaption">PayPay残高確認</a>
                  </li>
                </ul>
              </div>
              <hr>
              <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTfR1DVTw5gS33YS1B6RsLKDO9UJ_ANlpOlgg&usqp=CAU" alt="" class="chestbox"><strong>ログインすると毎日1回くじが引ける</strong>
            </div>

            <div>
              <div class="date"><!-- date and location-->
                <span>2021年1月7日(木)</span>
                <span>港区</span>
              </div>
              <div class="weather">
                <div class="today">
                  <strong class="when">今日の天気</strong>
                  <img src="https://s.yimg.jp/images/weather/general/next/101_night.png" alt="">
                  <spna class="hot">13°C</spna>
                  <small>|</small>
                  <span class="cold">3°C</span>
                  <spna class="rainChance">0%</spna>
                </div>
                <div class="tomorrow">
                  <strong class="when">明日の天気</strong>
                  <img src="https://s.yimg.jp/images/weather/general/next/101_day.png" alt="">

                  <spna class="hot">7°C</spna>
                  <small>|</small>
                  <span class="cold">0°C</span>
                  <spna class="rainChance">10%</spna>
                </div>
              </div>
            </div>
          </div>

          <div class="pickup"><!-- pickup -->
            <strong>ピックアップ</strong>
          </div>

          <div class='trending'><!-- trending -->
            <strong>リアルタイム検索で話題のキーワード</strong>
          </div>

          <div><!-- copyright --></div>

        </div>
        
      </div>

    </div>


    
  </body>

</template>
<script>
export default {
  name: 'App',
  data(){
    return{
      tabSelected: 'news',

    }
  },

  methods:{
    changeTab(tab){
      console.log(tab)
      this.tabSelected = tab;
      console.log(`this tabseldctef: ${this.tabSelected}`)
    },
  }
  
}
</script>
<style>

/* background-color: #f1f5ff;
border: 5px solid #beccea;
color: #4682B4; */

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


#topLink{
  margin-top: -1em;
}
#topLink a:link, a:visited{
  text-decoration:none;
  color: #4682B4;
}
#topLink a:nth-of-type(1){
  margin-left: 7em;
}
#topLink a:nth-of-type(2){
  margin-left: 2em;
}


.col-1 ul  {
  left: 0;
  background-color: #f1f5ff;
  width: 9em;
  border: 5px solid #beccea;
  margin-left: -5em;
  position: relative;
  margin-top: 2em;

  padding: 1.5em;

  margin: 25px;
  margin-right: -0.5em;
  margin-left: 0em;
}
.col-1 li{
  margin-bottom: 0.25em;
  margin-left: -0.5em;
  color: #4682B4;
}


.col-2{
  position: absolute;
  top: 18.7em;
  left: 52em;
  width: 26em;
  border: 5px solid #beccea;
  
  margin: 25px;
  margin-right: -0.5em;
}
.navbar{
  width: 26em;
  overflow: hidden;
  /* border: 5px solid #beccea; */
  
  margin-left: -2.4em;
  /* margin-right: 0.5em; */
  margin-top: -0.9em;
}
.navbar button {
  font-size: 80%;
  /* color: #1d3994; */
  /* background-color: #f1f5ff; */
  /* background-color: pink; */
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  transition: 0.3s;
}
.navbar button:nth-of-type(8){
  /* margin-left: 1em; */
  margin-right: 1em;
}
.notSelected{
  color: #1d3994;
  background-color: #f1f5ff;
}
.selected{
  color: black;
  background-color: white;
}
.navbar button:hover {
  background-color: #ddd;
}
.navbar button.active {
  background-color: #ccc;
}
.content small{
  /* position: relative; */
  left: 0em;
  color: grey;
}
.content ul{
  margin-top: 0.5em;
}
.bottomList{
  margin-top: 0.8em;
  margin-bottom: 1em;
  float: left;
  margin-right: 0.8em;
}
.content ul li{
  position: relative;
  margin-left: -2em;
  list-style-type: square;
  margin-top: 0.5em;
}


.middle2{
  position: absolute;
  top: 12em;
  width: 23.2em;
  height: 21em;
  border: 5px solid #beccea;
  /* margin-left: -3em; */
  
  /* margin: 25px; */
  margin-right: -0.5em;
  background-color: white;
  z-index: 2;
}

.middle2 strong{
  margin-left: -2em;
}
iframe{
  position: absolute;
  left: 0.7em;
  margin-top: 2em;
  width: 95%;
  height: 15em;
}
.middle2 span{
  position: absolute;
  margin-top: 18em;
  left: 1em;
}



.ads{
  position: absolute;
  top: 18.7em;
  left: 79em;
  width: 20em;
  /* border: 5px solid #beccea; */
  
  margin: 25px;
  margin-right: -0.5em;
}


.covid{
  position: absolute;
  top: 33.5em;
  left: 79em;
  width: 20em;
  /* border: 5px solid #beccea; */
  
  margin: 25px;
  margin-right: -0.5em;
}


.widget{
  position: absolute;
  top: 40.3em;
  left: 79em;
  width: 20em;
  height: 22em;
  border: 5px solid #beccea;
  
  margin: 25px;
  margin-right: -0.5em;
  background-color: #f1f5ff;
  z-index: 1;
}
.widget span{
  margin-top: 0.5em;
  margin-left: 0.75em;
  margin-right: 7em;
}
.widget button{
  margin-top: 0.5em;
  border-radius: 0%;
}

.login{
  position: absolute;
  left: 0em;
  width: 18.8em;
  /* top: 25.3em;
  left: 79em;
  width: 10em;
  height: 10em; */
  border: 5px solid #beccea;
  
  margin-top: 0.8em;
  margin-right: -0.5em;
  margin-left: 0.3em;
  background-color: white;
  z-index: 2;
  list-style-type: none;
}
.loginItem li{
  margin-top: -0.5em;
}
.loginItem img{
  width: 50px;
  height: 50px;
}
.loginItem :nth-of-type(1){
  margin-left: -1em;
  margin-right: 4em;
}
.loginItem :nth-of-type(2){
  margin-left: 4em;
}
.loginItem :nth-of-type(3){
  margin-left: 5em;
}
.loginCaption {
  margin-left: -1em;
  font-size: 70%;
  margin-top: -0.5em;
  display: block;
  left: -2em;
}
.login hr{
  width: 95%;
  background-color:#beccea;
  height: 1px;
  border: none;
}
.chestbox{
  width: 40px;
  height: 40px;
}
.login strong{
  position: absolute;
  margin-top: 0.8em;
  margin-left: 0.8em;
  font-size: 90%;
}

.date{
  background-color: #f1f5ff;
  position: absolute;
  left: 0em;
  width: 18.8em;
  border: 5px solid #beccea;
  
  margin-top: 12em;
  margin-right: -0.5em;
  margin-left: 0.3em;
  /* background-color: white; */
  z-index: 3;
  list-style-type: none;
}
.date span{
  margin-right: 3em;
}

.weather{
  background-color: white;
  position: absolute;
  left: 0em;
  width: 18.8em;
  border: 5px solid #beccea;
  
  margin-top: 13.6em;
  margin-right: -0.5em;
  margin-left: 0.3em;
  /* background-color: white; */
  z-index: 4;
  list-style-type: none;
}
.weather div{
  float: left;
  width: 7em;
  margin-left: 2em;
}
.weather strong{
  font-size: 80%;
  position: absolute;
}
.weather img{
  margin-top: 1em;
  width: 70px;
  height: 40px;
}
.weather small{
  margin-left: 0.3em;
  margin-right: -0.5em;
}
.weather .rainChance{
  margin-left: -6.5em;
}
.hot{
  color:  #ff3333;
}
.cold{
  color: #3385ff
}

.pickup{
  position: absolute;
  top: 63.5em;
  left: 79em;
  width: 20em;
  height: 10em;
  border: 5px solid #beccea;
  
  margin: 25px;
  margin-right: -0.5em;
  background-color: white;
  z-index: 1;
}

.trending{
  position: absolute;
  top: 80em;
  left: 79em;
  width: 20em;
  height: 22em;
  border: 5px solid #beccea;
  
  margin: 25px;
  margin-right: -0.5em;
  background-color: white;
  z-index: 1;
}









</style>
