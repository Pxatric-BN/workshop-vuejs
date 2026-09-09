<template>
  <v-card class="profile-card">
    <ProfileHeader />
    <ProfileInfo />
  </v-card>
</template>

<script>
import ProfileHeader from './ProfileHeader.vue'
import ProfileInfo from './ProfileInfo.vue'

export default {
  name: 'ProfileCard',

  components: {
    ProfileHeader,
    ProfileInfo
  }
}
</script>

<style scoped>
.profile-card {
  width: 350px;
  border-radius: 18px;
  overflow: visible;
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12) !important;
}
</style>