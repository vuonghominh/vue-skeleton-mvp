<template>
  <v-container fluid>
    <v-layout row wrap>
      <v-flex xs12 text-xs-center mt-5 mb-3>
        <h1 class="display-2 font-weight-bold">{{ $t('about.TITLE') }}</h1>
      </v-flex>
      <v-flex xs12 text-xs-center mb-2>{{ $t('about.DESCRIPTION') }}</v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  metaInfo() {
    return {
      title: this.$store.getters.appTitle,
      titleTemplate: this.$t('about.TITLE') + ' - %s'
    }
  }
}
</script>
