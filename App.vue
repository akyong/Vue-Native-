<template>
  <view class="container">
      <AppNavigation/>
<!--    <HomeScreen v-if="activeScreen === 'homeScreen'"  :aaa="testingData" :navigate="navigate"/>-->
<!--    <HomeScreen   />-->
<!--    <Screen1  v-if="activeScreen === 'screen1'" :navigate="navigate" />-->
<!--    <button title="Go to Screen 1" :on-press="() => {navigate('screen1')}" />-->
  </view>
</template>

<script>
  import HomeScreen from "@/screens/HomeScreen"
  import Screen1 from "@/screens/Screen1"
  import Screen2 from "@/screens/Screen2"
  import { createStackNavigator, createAppContainer } from "react-navigation"


  const HomeStack = createStackNavigator(
          {
              Home: HomeScreen,
              Screen1: Screen1,
              Screen2: Screen2

          }
  )

  const AppNavigation = createAppContainer(HomeStack);

  export default {
    components: {
      HomeScreen, AppNavigation
    }
  }
</script>

<style>
  .container {
    background-color: white;
    flex: 1;
  }
  .text-color-primary {
    color: blue;
  }
</style>



