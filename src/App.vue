<template>
  <div id="app">
    <!-- template部：コンポーネント名をHTMLタグとして記述 -->
    <NavigationBar />
    <!-- <MainPage /> -->
      <!--<MainPage /> に代わり、 URLに対応したコンポーネントを表示 -->
     <router-view></router-view>
  </div>
</template>

<script>
  // script部：コンポーネントの読み込み
import NavigationBar from '@/components/NavigationBar.vue'
// import MainPage from '@/components/MainPage.vue'

// script部：使用するコンポーネントの宣言
export default {
  name: 'App',
  components: {
    NavigationBar,
    // MainPage
  }
}
</script>

<style>
#app {
  height: 100vh;
}

 button.transparent {
    margin: 5px;
    background: transparent;
    border: none;
  }

 input.transparent {
    width: 100%;
    border: none;
  }
  input.transparent:focus {
    outline: none;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
</style>
