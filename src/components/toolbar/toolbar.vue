<template>
<div>
  <v-app-bar
    app
    flat
    color="transparent"
    class="toolbar"
  >
    <v-container class="text-container">
      <div class="toolbar-logo">
        Workshop
      </div>

      <v-spacer />

      <div class="toolbar-menu">
        <v-btn
          text
          to="/profile"
          class="toolbar-btn"
        >
          Profile
        </v-btn>
        <v-btn
          text
          to="/grade"
          class="toolbar-btn"
        >
          Grade
        </v-btn>
      </div>

    </v-container>
  </v-app-bar>
<v-main>
      <router-view/>
    </v-main>

  </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.toolbar {
  background: rgba(255, 255, 255, 0.65);
}
.text-container {
  display: flex;
  align-items: center;
}
.toolbar-logo {
  font-size: 18px;
  font-weight: 600;
  color: #222;
  letter-spacing: -0.3px;
}
.toolbar-menu {
  display: flex;
  align-items: center;
  gap: 4px;
}
.toolbar-btn {
  text-transform: none;
  font-size: 14px;
  font-weight: 500;
  color: #555;
  border-radius: 10px;
}

.toolbar-btn:hover {
  background: rgba(0, 0, 0, 0.04) ;
}
</style>

