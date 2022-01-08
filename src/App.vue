
<template>
  <div id="app">
    <div id="header-mini">
      <div id="link-info">
        <strong class="txt">교무실 : </strong>
        <a class="primary-color" href="#">054-832-2903</a>
        <strong class="txt">이메일 : </strong>
        <a class="primary-color" href="#">gbsw01@sc.gyo6.net</a>
      </div> 

      <div id="link-sns">
        <a href="" class="ico-padding">
          <v-icon class="primary-color">mdi-facebook</v-icon>
        </a>
        <a href="" class="ico-padding">
          <v-icon class="primary-color">mdi-instagram</v-icon>
        </a>
        <a href="" class="ico-padding">
          <v-icon class="primary-color">mdi-github</v-icon>
        </a>
      </div> 
    </div>
    <div id="header">
      <div id="nav">
        <a href="/" id="Logo">DoriMap<span id="logo-point">.</span> </a>
        <router-link class="tag" to="/">Home</router-link>
        <router-link class="tag" to="/about">About</router-link>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
@import url("./style/App.scss");
@import url('https://fonts.googleapis.com/css2?family=Righteous&display=swap');
template{
  margin: 0;
  padding: 0;
}
#header{
    position: sticky;
    top: 0;
    width: 100%;
    z-index: 2;
}
#Logo{
  font-family: 'Righteous', cursive;
  font-size: 30px;
  padding-right: 50%;
  color: #2c3e50;
  #logo-point{
    font-size: 40px;
    color: #42b983;
  }
}
#nav {
  padding: 10px;

    .tag {
        font-weight: bold;
        color: #2c3e50;
        padding-left: 20px;
        
        &.router-link-exact-active {
        color: #42b983;
        }
    }
}
</style>
