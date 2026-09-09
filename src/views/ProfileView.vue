<template>
  <div class="profile-page">
    <v-container>
      <v-row class="profile-row">
        <v-col
          cols="4"
          class="profile-style"
        >
          <ProfileCard />
        </v-col>

        <v-col
          cols="8"
          class="profile-content-col"
        >
          <div class="profile-content">
            <ProfileAbout />
            <ProfileSkill />
          </div>
        </v-col>
      </v-row> 
      <div class="profile-detail">
          <ProfileDetail />
      </div> 
    </v-container>
  </div>
</template>

<script>
import ProfileCard from '@/components/profile/ProfileCard.vue'
import ProfileAbout from '@/components/profile/ProfileAbout.vue'
import ProfileSkill from '@/components/profile/ProfileSkill.vue'
import ProfileDetail from '@/components/profile-details/ProfileDetails.vue'

export default {
  name: 'Profile',

  components: {
    ProfileCard,
    ProfileAbout,
    ProfileSkill,
    ProfileDetail
  }
}
</script>

<style>
.profile-page {
  min-height: 100vh;
  background: #eeeeee;
  padding: 40px 0;
}

.profile-row {
  display: flex;
  align-items: stretch;
}

.profile-style {
  display: flex;
  align-items: stretch;
}

.profile-style > * {
  width: 100%;
}

.profile-content-col {
  display: flex;
}

.profile-content {
  display: flex;
  flex-direction: column;
  gap: 20px;
  width: 100%;
  height: 100%;
}

.profile-content > * {
  flex: 1;
}

.profile-detail {
  margin-top: 20px;
}

</style>

