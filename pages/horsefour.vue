<!--horsefour the Dressage Dancers Trainer page-->
<template>
<section class="container">
  <head>
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
  </head>
    <a href="top"></a>
  <h1 class="title">Meet Our Trainer</h1>
    <h3 class="subtitle">We have an on-sight trainer affiliated with this barn. She can provide lessons to students of all skill levels.</h3>
  <div>
      <a href="#Dean" class="about-link">Dora Dean</a>
      <!--<a href="#Dewitt" class="about-link"></a>-->
   </div>

  <!--div One-->

  <div class="train-page">
      <img src="@/assets/images/doraProfile.jpg" class="image-style-left">
      <section class="train-section-left-pic">
        <a name="Dean"><h2>Dora Dean</h2></a>
          <p>Dora has been teaching and training dressage riders and horses since 2004. From beginning walk-trot all the way through Grand Prix, Dora can help you reach your dressage dreams.</p>
            <p>All those interested contact her: starlitedressage@hotmail.com.</p>
          <br>
          <br>
           <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
      </section>
    </div>

   <br>

   <!--div Two-->

   <!--<div class="train-page">
       <section class="train-section-right-pic">
         <a name="Dewitt"><h2></h2></a>
           <p>ou are interested in training with her,</p>
             <a href="http://debbiefornia-dewittdressage.com/contact.htm">Click here to contact her.</a>
           <br>
           <br>
           <a href="#top" class="top-link">Back to Top</a>
           <br>
            <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
       </section>
       <img src="@/assets/images/whitehorsehead.jpg" alt="white horse head in bridle" class="image-style-right">
     </div>-->

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
  height: 40%;
  width: 40%;
  margin-top: 20%;
  margin-left: 10%;
  margin-bottom: 10%;
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
  margin-top: 20%;
  margin-right: 1%;
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
