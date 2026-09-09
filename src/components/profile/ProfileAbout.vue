<template>
  <v-card flat class="profile-about">
    <v-card-text class="profile-about-content">
      <div class="profile-about-title">
        About
      </div>

      <div class="profile-about-text">
        Hi, I'm Chayanon (Guy), a Software Engineer at INET Hatyai.
        I'm passionate about software development, learning new
        technologies, and building impactful applications.
      </div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'ProfileAbout'
}
</script>

<style>
.profile-about {
  width: 100%;
  border-radius: 18px;
  overflow: visible;
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12) !important;
}

.profile-about-content {
  padding: 18px 20px;
}

.profile-about-title {
  margin-bottom: 6px;
  font-size: 13px;
  font-weight: 700;
  color: #333333;
}

.profile-about-text {
  font-size: 12px;
  line-height: 1.7;
  color: #777777;
}
</style>

