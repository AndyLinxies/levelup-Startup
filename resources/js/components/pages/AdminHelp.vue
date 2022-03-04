<template>
  <div>
    <div class="flex">
      <SideBar />
      <!-- ? Content -->
      <v-container>
        <v-row>
          <v-col>
            <h1 class="text-h4">Demander de l'aide a un membre de Molengeek</h1>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <!-- Body -->
            <FormAdminHelp/>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>
<script>
// import axios from 'axios'
import SideBar from '../SideBar.vue'
import FormAdminHelp from '../FormAdminHelp.vue'
import axios from 'axios'
// import { mapFields } from "vuex-map-fields";

export default {
  name: "AdminHelp",
  data: () => ({
    helps:[]
  }),
  components: {
    SideBar,
    FormAdminHelp
},
  methods: {
    // getHelps() {
    //         axios
    //             .get("/api/v1/helps", {
    //                 headers: { Authorization: "Bearer " + this.token },
    //             })
    //             .then((response) => {
    //                 this.notifications = response.data.data;
    //             });
    //     },
  },
  mounted () {
  },
  // computed: {
  //       ...mapFields(["token", "notifications"]),
  // }

};
</script>
<style></style>
