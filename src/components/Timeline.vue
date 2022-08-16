<template>
    <v-timeline>
    <v-timeline-item
      v-for="(year, i) in years" :key="i" :color="year.color" small >
      <template v-slot:opposite>
        <span
          :class="`headline font-weight-light`"
          v-text="year.year"
        ></span>
      </template>
      <div class="py-4">
        <h2 :class="`headline font-weight-bold mb-4 `">
          Tourism Research Institute
        </h2>
        <div>
          I.T Support  
        </div>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
export default {
    data: () => ({
      years: [
        {
          color: 'black',
          year: ' Present',
        },
       
      ],
    }),
}
</script>