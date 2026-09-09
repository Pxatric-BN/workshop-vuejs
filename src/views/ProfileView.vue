<template>
  <div class="profile-page">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="4"
          lg="4"
          class="profile-style"
        >
          <ProfileCard />
        </v-col>

        <v-col
          cols="12"
          md="8"
          lg="8"
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

<style scoped>
.profile-page {
  min-height: 100vh;
  background: #eeeeee;
  padding: 40px 0;
}

.profile-style {
  display: flex;
  justify-content: center;
  align-items: flex-start;
}

.profile-content {
  display: flex;
  flex-direction: column;
  gap: 20px;
}
.profile-detail{
  margin-top: 20px
}

</style>

