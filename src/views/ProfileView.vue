<template>
  <div class="profile-page">
    <v-row>
      <v-col cols="6" class="profile-style">
        <ProfileCard />
      </v-col>
      <v-col cols="6">

      </v-col>
    </v-row>
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