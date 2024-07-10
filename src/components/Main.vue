<template>
 
    <div>
       
        <v-sheet class="d-flex">
            <v-sheet class="ma-2 pa-2">Flex item</v-sheet>
            
            <v-card
            class="mx-auto w-100"
            color="surface-light"
            max-width="400"
        >
            <v-card-text>
            <v-text-field
                :loading="loading"
                append-inner-icon="mdi-magnify"
                density="compact"
                label="Search templates"
                variant="solo"
                hide-details
                single-line 
                @click:append-inner="onClick"
            ></v-text-field>
            </v-card-text>
        </v-card>
        <v-sheet class="ma-2 pa-2">Flex item</v-sheet>
        <v-sheet class="ma-2 pa-2">Flex item</v-sheet>
        </v-sheet>

      
        <v-sheet class="d-flex">
            <v-sheet class="ma-2 pa-2 me-auto">Flex item</v-sheet>
            <v-sheet class="ma-2 pa-2">Flex item</v-sheet>
            <v-sheet class="ma-2 pa-2 ">Flex item</v-sheet>
        </v-sheet>
       
            
        

    </div>

</template>


<style scoped>


</style>

<script>
  export default {
    data: () => ({
      loaded: false,
      loading: false,
    }),

    methods: {
      onClick () {
        this.loading = true

        setTimeout(() => {
          this.loading = false
          this.loaded = true
        }, 2000)
      },
    },
  }
</script>