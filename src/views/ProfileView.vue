<template>
  <div class="profile-page">
    <v-row>
      <v-col cols="6" class="profile-style">
        <ProfileCard />
      </v-col>
      <v-col cols="6" class="profile-style">
        <ProfileDetail />
      </v-col>
    </v-row>
  </div>
</template>

<script>
import ProfileCard from '@/components/profile/ProfileCard.vue'
import ProfileDetail from '../components/profile-details/ProfileDetails.vue'

export default {
  name: 'Profile',

  components: {
    ProfileCard,
    ProfileDetail
  }
}
</script>

<style>
.profile-page {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #eeeeee;
}

.profile-style{
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>