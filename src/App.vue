<template>
  <div id="app">
    <div class="top-nav">
      <ul class="container">
        <li>Dashboard</li>
        <li>My courses</li>
        <li>Calendar</li>
        <li>Badges</li>
        <li>Live Video sessions</li>
        <li>Bookmarks</li>
      </ul>
    </div>

    <div class="main-body">
      <button class="back-btn">Back</button>
      <h1>Your Bookmarked Courses</h1>
      <div class="courses-wrapper">
        <Course />
        <Course />
        <Course />
      </div>
    </div>
  </div>
</template>

<script>
import Course from "./course.component";
export default {
  name: "app",
  components: {
    Course
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      date: "3 month",
      likes: "5 likes",
      rating: "4.5",
      price: "$ 2000"
    };
  }
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html,
body {
  width: 100%;
  height: 100%;
}

#app {
  width: 100%;
  height: 100%;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  background-color: #f6f6f6;
}

.top-nav {
  width: 100%;
  height: 7%;
  background-color: #132144;
}
.top-nav ul {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-evenly;
  list-style: none;
  color: #ffffff;
}

.top-nav ul li {
  height: 100%;
  display: flex;
  align-items: center;
}

.back-btn {
  padding: 12px 20px;
  border-radius: 20px;
  background-color: #ffffff;
  border: none;
  box-shadow: 5px 3px 10px rgb(240, 239, 239);
}

.main-body {
  padding: 90px;
}

.main-body h1 {
  font-weight: 400;
  padding: 10px 0px 30px 0px;
}

.courses-wrapper {
  width: 60%;
  display: flex;
  justify-content: space-around;
}

.top-nav li:hover {
  color: #f28233;
  cursor: pointer;
  border-bottom: solid 3px #f28233;
}
</style>
