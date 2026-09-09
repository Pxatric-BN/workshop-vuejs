<template>
  <div class="profile-page">

    <ProfileCard />

  </div>
</template>

<script>
import ProfileCard from '@/components/profile/ProfileCard.vue'

export default {
  name: 'Profile',

  components: {
    ProfileCard
  }
}
</script>

<style scoped>
.profile-page {
  min-height: 100vh;

  display: flex;
  justify-content: center;
  align-items: center;

  background: #eeeeee;
}
</style>