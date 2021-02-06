<!--THIS IS THE CODING FROM CAROUSEL.VUE-->
<template>
  <section class="container" >

  <div>
      <transition-group name="fade" tag="div">
        <div v-for="i in [currentIndex]" :key="i">
          <img :src="currentImg" class="horse-carousel"/>
        </div>
      </transition-group>

    </div>

  </section>
</template>

<script>
export default {
  name: "carousel",
  data() {
    return {
      images: [

             //title="carol and horse"
             require("../assets/images/carolandhorse.jpg"),
             //title="dora rides canter pirouette in competition"
             require("../assets/images/carolandhorse.jpg"),
             //title="barn, arena and chairs"
             require("../assets/images/barnchairs.jpg"),
             //title="two students in helmets brush a horse in cross ties to ready for riding"
             require("../assets/images/studentsbrushhorse.jpg"),
             //title="dora rides passage in competition"
             require("../assets/images/dora2"),
             //title="an outdoor arena next to a pasture area"
             require("../assets/images/arenapasture.jpg"),
             //title="a saddled horse runs through the arena"
             require("../assets/images/saddledhorse.jpg"),
             //title="an outdoor horse paddock"
             require("../assets/images/paddock.jpg"),
             //title="Debbie Dewitt dressage trainer in the arena on her horse"
             require("../assets/images/debbie.jpg"),
             //title="Vivian Doolittle on her horse"
             require("../assets/images/vivian.jpg")
        ],
        timer: null,
        currentIndex: 0
      };
    },

    mounted: function() {
      this.startSlide();
    },

    methods: {
      startSlide: function() {
        this.timer = setInterval(this.next, 4000);
      },

      next: function() {
        this.currentIndex += 1;
      },
      prev: function() {
        this.currentIndex -= 1;
      }
},
      computed: {
      currentImg: function() {
        return this.images[Math.abs(this.currentIndex) % this.images.length];
      }
    }
 };

</script>

<style lang="css" scoped>



  .fade-leave-active {
    transition: all 0.9s ease;
    overflow: hidden;
   display: block;
   margin-left: auto;
   margin-right: auto;
    position: absolute;
    width:40%;
    opacity: 1;
  }


  .fade-leave-to {
    visibility: hidden;
    width:40%;
    opacity: 0;
  }

  .horse-carousel {
  width: 400px;
  height: 400px;
  background-postion: 50% 50%;
  background-size: cover;
  border-radius: 50%;
  margin-bottom: 30%;
  }

@media only screen and (max-width: 650px) {
  .horse-carousel {
    width: 300px;
    height: 300px;
    background-size: 5%;
    background-position: 10% 10%;

  }
}

@media only screen and (max-width: 750px) {
  .horse-carousel {
    margin-top: 10%;
  }
}

</style>
