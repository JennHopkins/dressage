<!--horsetwo page the Dressage Dancers About page-->
<template>
<section class="container">
  <head>
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
 
  </head>
  <a href="top"></a>
  <h1 class="title">About Us</h1>
  <h2 class="subtitle">Dressage Dancers is a barn owned and managed by Carol Hopkins.</h2>

  
<div class="center-about-links">
  <nuxt-link to="/" class="about-link">Home</nuxt-link>
  <nuxt-link to="/horsethree" class="about-link">Services</nuxt-link>
  <nuxt-link to="/horsefour" class="about-link">Trainers</nuxt-link>
</div>
 
  
  <!--div One general history-->
    <div class="about-section-one">
          <section class="about-text first">
           <h2 style="color: white;">History</h2>
             <p style="color:white;"> Carol started out teaching dressage riding and boarding horses 20 years ago in Kirkland before moving from Bridle Trails in Bellevue to the Equestrian area in Woodinville WA. Carol, a certified public school teacher, began teaching riding lessons in the year 2000.  Her background with horses started when she was 6 years old, riding ponies in the Michigan summers.  In 1970 she bought her first horse, and began riding lessons.</p>
              <br>
              <br>
             <a href="#history"><div class="arrow bounce">
            </div></a>
          </section>
          <!--carosel image here-->
                  <carousel />

             </div>



     <!--div two - Carol's horse history-->
           <div class="about-section-two">
                <img src="@/assets/images/carolONhorse.jpg" alt="Carol wears helmet and rides a horse" class="about-pic-two">
             <section>
               <div class="about-text third">
                <p style="color:white;">During the years between 1976 -1980. Carol competed on the Hunter/Jumper A Show circuit. In 1986 Carol switched to riding Dressage.   After many years of lessons, clinics with well known trainers Carol began competing in Dressage,  In her many years of competing she has received many awards and championships.</p>
                  <br>
               <p style="color:white;"> Presently, Carol manages her barn along with an inhouse barn assistant who takes excellent care of the boarding horses. </p>
                   <br>
                <p style="color:white;"> Trainers are welcome to teach in her arenas.</p>
              </div>
               <br>
               <br>
                 <a href="#top" class="top-link">Back to Top</a>
               <br>
               <br>
                 <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
              </section>

         </div>
           <br>

     <!--div Two-->
            <!--<div class="about-section-two">
               <img src="@/assets/images/barnandstable.jpg" alt="a barn and a stable" class="about-pic-two">
              <section class="about-section-right">
                 <h2>Barn Policies</h2>
                   <p>Bulls at rose garden cucumbers mice sunflower wheat in pig. Petting zoo at carrots alligators quack. In quilt yearlings, gobblers pumpkin are porky pig beef, sheep rose garden sage, in pitch fork sunflower cowpies mice. Mouse soybeans sweet corn hogs llamas or oink oink wind. Rooster celery pineapples fertilizer, a melon chirp pets in. Feed in a woof, a farmers market. Bulls at rose garden cucumbers mice sunflower whea.</p>

                   <br>
                   <br>
                    <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
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
import carousel from "@/components/carousel.vue";


export default {
  components: {
  'carousel': carousel,
    }
  }

</script>
<style media="screen">


.about-section-one {
  display: flex;
  flex-direction: row;
  align-items: flex-end;
  margin-bottom: 10%;
  margin-right: 1%;
}

.about-text {
  margin: 0 13% 15%;
  }


.about-section-two {
  display: flex;
  flex-direction: row;
  margin-bottom: 5%;
}


.about-pic-two {
  height: 30%;
  width: 30%;
  border-bottom-right-radius: 50%;
  border-top-right-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
  margin-bottom: 25%;
  }

.board-link {
  font-size: 100%;
  margin: 50% 0 20% 10%;
  }

.about-link {
  padding-right: 20px;
}

/*arrow down animation*/
.arrow {
  bottom: 0;
  left: 50%;
  margin-left:20px;
  width: 40px;
  height: 40px;
  background-image: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAxNi4wLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI+DQo8c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4IiB3aWR0aD0iNTEycHgiIGhlaWdodD0iNTEycHgiIHZpZXdCb3g9IjAgMCA1MTIgNTEyIiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAgMCA1MTIgNTEyIiB4bWw6c3BhY2U9InByZXNlcnZlIj4NCjxwYXRoIGZpbGw9IiNGRkZGRkYiIGQ9Ik0yOTMuNzUxLDQ1NS44NjhjLTIwLjE4MSwyMC4xNzktNTMuMTY1LDE5LjkxMy03My42NzMtMC41OTVsMCwwYy0yMC41MDgtMjAuNTA4LTIwLjc3My01My40OTMtMC41OTQtNzMuNjcyICBsMTg5Ljk5OS0xOTBjMjAuMTc4LTIwLjE3OCw1My4xNjQtMTkuOTEzLDczLjY3MiwwLjU5NWwwLDBjMjAuNTA4LDIwLjUwOSwyMC43NzIsNTMuNDkyLDAuNTk1LDczLjY3MUwyOTMuNzUxLDQ1NS44Njh6Ii8+DQo8cGF0aCBmaWxsPSIjRkZGRkZGIiBkPSJNMjIwLjI0OSw0NTUuODY4YzIwLjE4LDIwLjE3OSw1My4xNjQsMTkuOTEzLDczLjY3Mi0wLjU5NWwwLDBjMjAuNTA5LTIwLjUwOCwyMC43NzQtNTMuNDkzLDAuNTk2LTczLjY3MiAgbC0xOTAtMTkwYy0yMC4xNzgtMjAuMTc4LTUzLjE2NC0xOS45MTMtNzMuNjcxLDAuNTk1bDAsMGMtMjAuNTA4LDIwLjUwOS0yMC43NzIsNTMuNDkyLTAuNTk1LDczLjY3MUwyMjAuMjQ5LDQ1NS44Njh6Ii8+DQo8L3N2Zz4=);
  background-size: contain;
}

.bounce {
  animation: bounce 2s infinite;
}

@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}

@media only screen and (max-width: 650px) {
  .about-section-one {
    display: flex;
    flex-direction: column-reverse;
    align-items: flex-end;
    margin-bottom: 10%;
    margin-right: 1%;
  }

  .about-text {
    margin: 0 13% 15%;
    }

.about-pic-two {
  margin-bottom: 10%;
}

  .about-section-two {
    display: flex;
    flex-direction: column;
    margin-bottom: 5%;
  }

  .about-link {
   margin: 30px;
  }

.center-about-links {
  display: flex;
  flex-direction: row;
}

}

@media only screen and (max-width: 750px) {
  .about-section-one {
    display: flex;
    flex-direction: column-reverse;
      }
}
</style>
