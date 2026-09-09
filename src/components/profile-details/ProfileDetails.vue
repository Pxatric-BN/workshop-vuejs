<template>
  <div>
    <v-card
      v-for="(item, index) in items"
      :key="index"
      class="profile-card mb-4"
      max-width="600"
      outlined
    >
      <v-list-item three-line>
        <v-list-item-content>
          <div class="text-overline mb-4 ">
            {{ item.title }}
          </div>

          <v-list-item-title class="text text-h5 mb-1">
            {{ item.name }}
          </v-list-item-title>
          <div class="about-card">
            <v-list-item-subtitle class="about-text">
                {{ item.description }}
            </v-list-item-subtitle>
          </div>
        </v-list-item-content>

        <v-list-item-avatar
          tile
          size="80"
          color="grey"
        >
          <v-img :src="item.imglink"></v-img>
        </v-list-item-avatar>
      </v-list-item>
    </v-card>
  </div>
</template>
<script>
export default {
    name: 'ProfileDetail',
    data() {
        return {
            value:'',
            items: [
                {
                    title: 'Hobby',
                    name: 'Terrarium',
                    description: 'Creating and taking care of small plants and terrariums is one of my favorite hobbies. I enjoy designing miniature landscapes, choosing different types of plants, and creating small natural environments inside glass containers. It is a relaxing activity that allows me to be creative while also learning about plants, balance, and patience. I especially enjoy watching the plants grow and maintaining each terrarium over time.',
                    imglink: 'https://res.klook.com/image/upload/w_750,h_469,c_fill,q_85/w_80,x_15,y_15,g_south_west,l_Klook_water_br_trans_yhcmh3/activities/wugjorsvc5dtm5vfl5ua.jpg'
                },
                {
                    title: 'Graduated',
                    name: 'Prince of Songkla University',
                    description: 'Graduated with a Bachelor of Science degree in Computer Science, with a strong interest in software development, web technologies, and building practical solutions through technology.',
                    imglink: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTHKhAJdNYhqmUz2PgcoFWhUBdKCKnBQ3EhmmvjTUI86EFALnOQD3IGEjQ&s=10'
                },
                {
                    title: 'Experience',
                    name: 'ERP Functional Implement and Consult',
                    description: 'Experience in ERP implementation, system analysis, and consulting, helping businesses improve their processes through effective technology solutions.',
                    imglink: 'https://ucarecdn.com/1bf45853-e215-41d8-97fd-c94ee47e5849/-/resize/1050/'
                }
            ]
        }
    },
}


</script>

<style scoped>
.profile-card {
  width: 100%;
  max-width: 400px;
  border-radius: 18px;
  overflow: visible;
  background: #ffffff;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.12) !important;
  margin: 4;
}
.text {
  font-size: 20px;
  font-weight: 700;
  color: #222222;
}

.about-text{
  font-size: 12px;
  line-height: 1.6;
  color: #777777;
}
.about-card {
  margin-top: 15px;
  border-radius: 12px;
  background: #f8f8f8;
}
</style>