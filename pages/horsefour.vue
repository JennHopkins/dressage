<!--horsefour the Dressage Dancers Trainer page-->
<template>
<section class="container">
  <head>
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
 
  </head>
    <a href="top"></a>
  <h1 class="title">Meet Our Trainers</h1>
 <h3 class="subtitle">These are all the trainers we have currently on site.</h3>
  
<div class="center-about-links">
  <nuxt-link to="/" class="about-link">Home</nuxt-link>
  <nuxt-link to="/horsethree" class="about-link">Services</nuxt-link>
  <nuxt-link to="/horsefour" class="about-link">Trainers</nuxt-link>
</div>
 
  <br>
  <br>
  <br>
  <br>
  <br>
  <br>
  <div>

    <!--this is a link to the link to the link - comment left by mcjulie as a test --I think the user can click between the hrefs here to get to the trainer website, therefore #trainer is a link to #ihaveawebsite which is a link to #http://ihavewebsite.com-->
      <a href="#trainer" class="about-link">We are looking for a new trainer!</a>
    
    <!--link to go to website also here it should read #ihaveawebsite instead of #Dewitt which is the name of the link-->
      <!--<a href="#Dewitt" class="about-link"></a>-->
   </div>

  <!--div One-->
  <div class="train-page">
      <img src="@/assets/images/viviandressage.jpg" class="image-style-left">
      <section class="train-section-left-pic">
        <a name="Dean"><h2></h2></a>
          <p></p>
            <p style = "color:white;">future website for future trainer</p>
          <br>
          <br>
           <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
      </section>
    </div>

   <br>

   <!--div Two-->

   <!--<div class="train-page">
       <section class="train-section-right-pic">
  
  <!--I need to put a link loop in the website here-->
         <a name="ihaveawebsite"><h2></h2></a>
           <p></p>

  <!-- I need to put a website link here - will put the text "click here to contact trainer" between a's below -->
           <!--  <a href="http://ihaveawebsite.com"></a> -->
  
          <!-- took out <br>s to see if I can get footer to show up --> 
          
           <a href="#top" class="top-link">Back to Top</a>
           <br>
            <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
       </section>
       <img src="@/assets/images/whitehorsehead.jpg" alt="white horse head in bridle" class="image-style-right">
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
  height: 70%;
  width: 70%;
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
