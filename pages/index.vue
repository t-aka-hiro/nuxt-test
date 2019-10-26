<template>
  <v-layout>
    <v-flex>
      <div class="text-center">
        <InputTask v-on:child-event="TaskAdded" />
        <taskView v-bind:tasks="tasks" v-on:child-event="TaskFinished" />
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
//  import Logo from '~/components/Logo.vue'
//  import VuetifyLogo from '~/components/VuetifyLogo.vue'
import TaskView from "~/components/TaskView.vue";
import InputTask from "~/components/InputTask.vue";

export default {
  components: {
    //  Logo,
    //  VuetifyLogo
    TaskView,
    InputTask
  }
};
</script>
