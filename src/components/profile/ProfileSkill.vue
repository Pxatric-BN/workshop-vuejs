<template>
  <v-card flat class="profile-skill">
    <v-card-text class="profile-skill-content">
      <div class="profile-skill-title">
        Skill
      </div>

      <div class="profile-skill-list">
        <v-chip
          v-for="(skill, index) in skills"
          :key="index"
          small
          outlined
          :color="skill.color"
        >
          {{ skill.name }}
        </v-chip>
      </div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'ProfileSkill',

  data() {
    return {
      skills: [
        {
          name: 'Python',
          color: '#5003C0'
        },
        {
          name: 'NodeJs',
          color: '#2A7C13'
        },
        {
          name: 'Odoo ERP',
          color: '#FF7F50'
        },
        {
          name: 'TypeScript',
          color: '#2E6FA0'
        },
        {
          name: 'Java',
          color: '#D10056'
        }
      ]
    }
  }
}
</script>

<style scoped>
.profile-skill {
  width: 100%;
  border-radius: 18px;
  overflow: visible;
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12) !important;
}

.profile-skill-content {
  padding: 18px 20px;
}

.profile-skill-title {
  margin-bottom: 10px;
  font-size: 13px;
  font-weight: 700;
  color: #333333;
}

.profile-skill-list {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

</style>

