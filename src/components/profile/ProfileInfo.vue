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
              @click="dialog=true"
            >
             GET IN TOUCH
            </v-btn>
            <v-dialog
              v-model="dialog"
              max-width="400"
            >
              <v-card rounded="lg">
                <v-card-title class="text-h6">
                  Get in touch
                </v-card-title>

                <v-card-text>
                  <div>
                    <v-icon color="black" >
                      mdi-email-outline
                    </v-icon>

                    <div>
                      <div class="text-caption text-grey">
                        Email
                      </div>
                      <div>
                        chayanon.ban@one.th
                      </div>
                    </div>
                  </div>

                  <div>
                    <v-icon color="black" >
                      mdi-phone-outline
                    </v-icon>

                    <div>
                      <div class="text-caption text-grey">
                        Phone
                      </div>
                      <div>
                        061-741-1604
                      </div>
                    </div>
                  </div>
                </v-card-text>

                <v-card-actions>
                  <v-spacer />

                  <v-btn
                    variant="text"
                    color="error"
                    @click="dialog = false"
                  >
                    Close
                  </v-btn>
                </v-card-actions>
              </v-card>
            </v-dialog>
          </div>
        </v-col>
      </v-row>
  
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: 'ProfileInfo',
  data(){
    return {
      dialog: false
    }
  }
}
</script>

<style>
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
</style>

