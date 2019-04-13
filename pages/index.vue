<template>
  <section class="container">
    <header class="title">
      <h1>
        10_team_profile
      </h1>
    </header>
    <div class="top-image">
      <img class="member_image" src="~assets/images/topimage.jpg">
    </div>
    <div class="members">
      <h2>members</h2>
      <div class="cssgrid">
        <div class="member">
          <h3 class="name">スター</h3>
          <img class="member_image" src="~assets/images/star.jpg">
          <p></p>
        </div>
        <div class="member">
          <h3 class="name">かっちゃん</h3>
          <img class="member_image" src="~assets/images/kazumi.jpg">
          <p></p>
        </div>
        <div class="member">
          <h3 class="name">じゅん</h3>
          <img class="member_image" src="~assets/images/jun.jpg">
          <p></p>
        </div>
        <div class="member">
          <h3 class="name">もか</h3>
          <img class="member_image" src="~assets/images/moca.jpg">
          <p></p>
        </div>
        <div class="member">
          <h3 class="name">てんちゃん</h3>
          <img class="member_image" src="~assets/images/hiroko.jpg">
          <p></p>
        </div>
        <div class="member">
          <h3 class="name">たいが</h3>
          <img class="member_image" src="~assets/images/taiga.jpg">
          <p></p>
        </div>
      </div>
    </div>
    <div class="photos">
      <h2>photos</h2>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 30px;
  color: #35495e;
  letter-spacing: 1px;
  padding: 20px 0;
}

.top-image {
}

.top-image img {
  background-size: cover;
  width: 100%;
  height: 500px;
  object-fit: cover;
}

.members {
  padding-top: 30px;
}

.members h2 {
  padding: 20px;
}

.cssgrid {
  display: grid;
  grid-template-columns: repeat(3, minmax(100px, 1fr));
  grid-auto-rows: 1fr;
}

.member {
  padding: 10px;
}

.name {
  padding-bottom: 5px;
}

.member_image {
  width: 100%;
}

@media screen and (min-width: 736px) {
  .cssgrid {
    grid-gap: 28px;
  }
}

@media screen and (max-width: 735px) {
  .cssgrid {
    grid-gap: 3px;
  }
}

</style>
