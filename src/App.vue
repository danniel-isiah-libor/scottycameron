<template>
  <v-app>
    <router-view />
    <SnackBar />
    <Dialog />
  </v-app>
</template>

<script>
import SnackBar from '@/components/App/SnackBar.vue'
import Dialog from '@/components/App/Dialog.vue'

export default {
  components: {
    SnackBar,
    Dialog
  }
}
</script>

<style>
html {
  overflow-y: auto !important;
  overflow-x: auto !important
}
button {
  -webkit-app-region: no-drag !important;
}
.titleBar {
  -webkit-user-select: none !important;
  -webkit-app-region: drag !important;
}

/* Let's get this party started */
::-webkit-scrollbar {
  width: 8px;
}

/* Track */
::-webkit-scrollbar-track {
  /* -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3); */
  -webkit-border-radius: 10px;
  border-radius: 10px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  -webkit-border-radius: 10px;
  border-radius: 10px;
  background: grey;
  /* -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.5); */
}
::-webkit-scrollbar-thumb:window-inactive {
  background: grey;
}
</style>
