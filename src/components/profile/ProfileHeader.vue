<template>
  <div class="profile-header">

    <img
      class="header-background"
      src="https://i.pinimg.com/736x/cf/e2/17/cfe2172e5036d70c43ab7179d4fa7954.jpg"
      alt="Profile banner"
    />

    <ProfileAvatar />

  </div>
</template>

<script>
import ProfileAvatar from './ProfileAvatar.vue'

export default {
  name: 'ProfileHeader',

  components: {
    ProfileAvatar
  }
}
</script>

<style scoped>
.profile-header {
  position: relative;
  height: 155px;
  padding: 10px;
}

.header-background {
  width: 100%;
  height: 115px;
  border-radius: 14px;

  object-fit: cover;
  object-position: center;
}
</style>