<template>
  <v-container class="mt-5">
    <v-layout>
      <v-flex xs4>

        <Projects></Projects>

      </v-flex>
      <v-flex xs8 class="pl-4">
        <Panel title="Projects">
          <h1>TESTING</h1>
        </Panel>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import { mapGetters, mapState } from 'vuex';
import Projects from '../components/Projects.vue';
import router from '../router';

export default {
  components: {
    Projects,
  },
  mounted() {
    if (!this.isLoggedIn) {
      return router.push('/login');
    }
  },
  computed: {
    ...mapState('projects', [
      'currentProject',
    ]),
    ...mapGetters('authentication', [
      'isLoggedIn',
    ]),
  },
};
</script>

<style>

</style>
