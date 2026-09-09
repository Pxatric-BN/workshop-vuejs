<template>
  <v-card
    flat
    class="info-card"
  >
    <v-card-text>
      <v-row
        align="center"
        justify="space-between"
        no-gutters
      >
        <v-col cols="auto">
          <div class="name">
            Chayanon Banyen
          </div>

          <div class="username">
            @INET Hatyai
          </div>
        </v-col>

        <v-col cols="auto">
          <div class="actions">
            <v-btn
              outlined
              small
              class="getintouch-button"
            >
             GET IN TOUCH
            </v-btn>
          </div>
        </v-col>
      </v-row>
      <v-card
        flat
        class="about-card"
      >
        <v-card-text class="about-content">

          <div class="about-title">
            About
          </div>

          <div class="about-text">
            Hi, I'm Chayanon (Guy), a Software Engineer
            at INET Hatyai. I'm passionate about software
            development, learning new technologies, and
            building impactful applications.
          </div>

        </v-card-text>
      </v-card>

    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'ProfileInfo'
}
</script>

<style scoped>
.info-card {
  background: #ffffff;
}

.name {
  font-size: 20px;
  font-weight: 700;
  color: #222222;
}

.username {
  margin-top: 2px;
  font-size: 13px;
  color: #999999;
}

.actions {
  display: flex;
  align-items: center;
  gap: 4px;
}

.getintouch-button {
  min-width: 75px;
  height: 30px;
  border-radius: 8px;
  text-transform: none;
  font-size: 12px ;
  background-color: #222222;
  color: #ffffff;
}

.about-card {
  margin-top: 15px;
  border-radius: 12px;
  background: #f8f8f8;
}

.about-content {
  padding: 12px;
}

.about-title {
  margin-bottom: 5px;
  font-size: 13px;
  font-weight: 700;
  color: #333333;
}

.about-text {
  font-size: 12px;
  line-height: 1.6;
  color: #777777;
}
</style>

