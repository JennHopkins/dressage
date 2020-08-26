<!--horsefour the Dressage Dancers Trainer page-->
<template>
<section class="container">
  <head>
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
  </head>
    <a href="top"></a>
  <h1 class="title">Meet Our Trainers</h1>
    <h3 class="subtitle">We have on-sight trainers affliated with this barn. They can provide lessons to students of all skill levels.</h3>
    <div>
      <a href="#Dewitt" class="about-link">Debbie Fornia-Dewitt</a>
      <a href="#Doolittle" class="about-link">Vivian Doolittle</a>
  </div>

  <!--div One-->
    <div class="train-page">
        <img src="@/assets/images/whitehorsehead.jpg" alt="white horse head in bridle" class="image-style-left">
        <section class="train-section-left-pic">
          <a name="Dewitt"><h2>Debbie Fornia-Dewitt</h2></a>
            <p>Debbie Fornia-Dewitt offers the highest quality in dressage training, tailored toward each individual as well as each horse. She has been riding and training Dressage for over 30 years. Her experience with hundreds of horse-and-rider combinations as well as her own training with numerous international-level trainers supports her training system.</p> <br><p> If you are interested in training with her,</p>
              <a href="http://debbiefornia-dewittdressage.com/contact.htm">Click here to contact her.</a>
            <br>
            <br>
             <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
        </section>
      </div>

     <br>

   <!--div Two-->
            <div class="train-page viv">
              <section class="train-section-right-pic">
                <a name="Doolittle"> <h2>Vivian Doolittle</h2></a>
                   <p>I’ve been training and teaching professionally for over 35 years. I started my professional career as an assistant instructor at Sunnybrook Stables for the University of Washington Experimental College. I taught six Beginning Horsemanship group lessons a week, each with 5 to 7 riders </p>
                   <br>
                   <p>I have earned my USDF Bronze medal on a horse I trained myself. Subsequent to that, I did not show for 17 years after my divorce. I will be returning to the show ring in the 2021 season, competing my own and several clients’ horses. I have been trained all the way up the levels through the Grand Prix and I will be pursuing my silver and gold medals beginning in 2021.
</p>              <br>
                   <p>I believe that dressage is the language we invented to communicate with horses. We must teach them grammar and syntax before we can expect them to create great poetry. I specialize in adult beginning riders, but have also trained other professionals and all points in between. </p><br><p> If you are interested in training with her,</p>
                <div>
                  <p v-if="show"></p>
                <span v-if="show">
                  <p>{{contact}}</p>
                </span>
                <a @click="show = !show">Click here for her contact information</a>
                  </div>
                   <br>
                   <br>
                     <a href="#top" class="top-link">Back to Top</a>
                     <br>
                    <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
               </section>
               <img src="@/assets/images/viviandressage.jpg" alt="vivian in full dressage uniform competes on her horse" class="image-style-right">
            </div>

     <!--footer-->
       <div class="horse-box">
         <footer>

           <div class="horse-foot">
             <h3>We Are Located at:</h3>
             <p>21718 NE 161st St.</p>
             <p>Woodenville, WA 98077</p>
           </div>
           <div class="horse-foot">
               <div class="fb-layout">
             <h3>Connect</h3>
             <!--facebook stuff-->

        <i class="fab fa-facebook social-horse"></i>
        <a href="https://www.facebook.com/DressageDancers/"><button class="dressage-facebook">Facebook</button></a>
      </div>
           </div>
           <div class="horse-foot">
             <h3>Contact Us</h3>
             <p>Email: dressagedancers@gmail.com</p>
             <p>Phone: 425-889-6468</p>
           </div>

         </footer>
       </div>
</section>
</template>
<script type="text/javascript">
export default {
  data() {
    return {
      show: false,
      contact: 'Phone: 425-344-4660, Email: love2piaffe@gmail.com'
    }
  }
}
</script>
<style media="screen">

.train-page {
  display: flex;
  flex-direction: row;
  margin-bottom: 5%;
}

.image-style-left {
  height: 30%;
  width: 30%;
  border-bottom-right-radius: 50%;
  border-top-right-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
}

.image-style-right {
  height: 30%;
  width: 30%;
  margin-top: 10%;
  margin-bottom: 20%;
  border-bottom-left-radius: 50%;
  border-top-left-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
}

.train-section-left-pic {
  margin-top: 10%;
  margin-right: 10%;
  margin-left: 20%;
}

.train-section-right-pic {
  margin-top: 10%;
  margin-right: 25%;
  margin-left: 10%;
  margin-bottom: 10%;
}

.board-link {
  font-size: 100%;
  margin-top: 50%;
  margin-bottom: 20%;
}

.top-link {
  margin: 10%;
}

@media only screen and (max-width: 600px) {
  .train-page {
    display: flex;
    flex-direction: column;
  }

.about-link {
  margin: 1rem;
  text-align: center;
}

.viv {
display: flex;
flex-direction: column-reverse;
}

.image-style-right {
  width: 60%;
  height: 60%;
  margin-left: 40%;
}

.train-section-right-pic {
  margin-top: 10%;
  margin-right: 15%;
  margin-left: 10%;
 }
}
</style>
