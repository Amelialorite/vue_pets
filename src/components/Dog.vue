<template>
  <v-card class="dog-card">
    <v-img :src="dog" height="150px"></v-img>
    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn icon @click="$emit('remove');"> <v-icon>delete</v-icon> </v-btn>
    </v-card-actions>
  </v-card>
</template>
<script>
export default {
  props: {
    dog: {
      type: String
    }
  }
};
</script>
