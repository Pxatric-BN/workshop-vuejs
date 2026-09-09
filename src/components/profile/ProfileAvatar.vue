<template>
  <div class="avatar-wrapper">

    <v-avatar
      size="105"
      class="profile-avatar"
    >
      <img
        src="@/assets/profile_picture.jpeg"
        alt="Profile"
      >
    </v-avatar>

  </div>
</template>

<script>
export default {
  name: 'ProfileAvatar'
}
</script>

<style>
.avatar-wrapper {
  position: absolute;
  left: 20px;
  bottom: -5px;
  z-index: 2;
}

.profile-avatar {
  border: 5px solid #ffffff;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}
</style>

