<template>
  <div class="course-card-component">
    <div class="course-img">
      <img
        src="https://images.unsplash.com/photo-1542744094-24638eff58bb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1351&q=80"
        alt="courses"
      />
    </div>
    <div class="course-contents">
      <div class="course-title">
        <h3>Certification course on Health care and quality management</h3>
        <div class="bookmark-logo"></div>
      </div>
      <div class="course-description">
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aspernatur magnam beatae labore doloribus. Amet ipsam enim esse sed autem omnis..</p>
      </div>
      <div class="like-btn">
        <div class="date btn-default">
          <p>{{date}}</p>
        </div>

        <div class="likes btn-default">
          <p>{{likes}}</p>
        </div>
      </div>
      <div class="rating-price">
        <div class="rating">
          <p>{{rating}}</p>
        </div>
        <div class="price">
          <p>{{price}}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      date: "3 month",
      likes: "5 likes",
      rating: "4.5",
      price: "$ 20000"
    };
  }
};
</script>

<style scoped>
.course-card-component {
  width: 30%;
  height: 80%;
  background-color: #ffffff;
  border-radius: 5px;
  padding: 10px;
}

.course-contents {
  width: 100%;
  height: 85%;
  padding: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.course-img img {
  width: 100%;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;
  background-position: center;
}

.course-title {
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-bottom: 10px;
}

.course-title h3 {
  width: 90%;
  font-weight: 400;
  font-size: 16px;
}

.course-title .bookmark-logo {
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background-color: #f28233;
}

.course-description {
  width: 90%;
  font-weight: 300;
  font-size: 12px;
  margin-bottom: 10px;
}

.like-btn {
  display: flex;
  justify-content: flex-start;
}

.rating-price {
  display: flex;
  justify-content: space-between;
  margin-top: 10px;
}

.btn-default {
  padding: 8px 20px;
  font-size: 12px;
  margin-right: 5px;
  border-radius: 20px;
  background-color: #f6f6ff;
}
</style>