<!--HERE IS ALL OF THE CODING FROM ACCORDIAN.VUE-->

<template>
  <!--this is the basic template for the faq accordion page which will fill the template on baseAccordian-->
  <div>
    <div v-for="accordian in accordians" :key="accordian.type">
      <accordianTemplate>
  <!--this is the slot the user will see and click on. This will call in the question text -->
  <template v-slot:type>{{ accordian.type }}</template>

<!--this is the slot that will only show when the user clicks on the title slot. This will call in the answer text-->
 <template v-slot:content>
   <div>{{ accordian.text }}</div>
 </template>

    
        
</accordianTemplate>
</div>
</div>
</template>


<script>
import accordianTemplate from "@/components/accordianTemplate";

//this is the data and array for the faq accordion page - this should populate the baseAccordian page

export default {
  components: {
    accordianTemplate
  },
  data() {
    return {
      accordians: [
// first slot
        {
          type: "Full Care Boarding",
          text: "$950 a month"
        },

//second slot
        {
          type: "Trailer Parking",
          text: "$50 a month"
        },
//third slot
        {
          type: "Lessons: with school horse",
          text: "$95 for 40 minutes (plan on approximately 15 minutes for tack up of horse). These are Carol's prices, see Trainer Page for other instructors' prices. Please note: Carol only takes on a small number of students"
        },
           ]
    };
  }
};

</script>

<style scoped>


}
</style>
