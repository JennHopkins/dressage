<!--HERE IS THE CODE FROM BASEACCORDIAN.VUE-->
<template>
  <!--this component, the baseAccordian page, it is the Parent component, it will give a basic template and code for the toggles to hide or show content.-->
  <div class="wrapper">
    <div class="accordian" @click="toggleItem">
<!--service goes here-->
      <h2 class="type">
        <slot name="type"></slot>
      </h2>
    </div>
<!--price info goes here-->
    <div v-show="show" class="content">
      <slot name="content"></slot>
    </div>
  </div>
</template>

<script>
//data and method to toggle the hide or show state of content
export default {
  data: function() {
    return {
      show: false
    };
  },
  methods: {
    toggleItem: function() {
      this.show = !this.show;
    }
  }

};

</script>

<style scoped>
.wrapper {
  width: 200px;
  padding: 10px;
  display: block;
  text-align: left;
}
.accordion {
  display: flex;
  margin: 0;
}

.type {
  margin: 0;
  font-size: 100%;
  }
  
.content {
  width: 100%;
  border-bottom: 1px solid white;
  padding: 10px;
}
</style>
