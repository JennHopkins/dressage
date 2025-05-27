<!--horsethree the Dressage Dancers Services page-->
<template>
<section class="container">
  <head>
     <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
  
  </head>
  <a href="top"></a>
  <h1 class="title">Our Services</h1>
  <h2 class="subtitle">Here's what we can do for you</h2>
  <!--div One-->
    <div class="board-page board-part">
        <img src="@/assets/images/barnandstable.jpg" alt="a barn and a stable" class="services-pic-one">
        <section class="board-section-left-pic">
          <h2>Horse Boarding</h2>
          <p>Boarding is provided for a reasonable fee. All horses, have individual paddocks (12 x 12) with covered padded stalls. Stalls have attached mud-free paddocks Horses, are fed 2 times a day (in hay nets that provide hay all day and night). Stalls and paddocks are cleaned twice a day. There are 2 full size dressage arenas, one covered (with lights for night riding) and one outside sand arena.</p>
          <p>We take pride in being a small and drama-free barn.</p>
          <p>We provide:</p>
          <ul>
            <li>Full care horse board</li>
            <li>Bedding for horses upon request</li>
            <li>Individual paddocks</li>
            <li>Tack room</li>
            <li>Cross ties for grooming, visits with farrier, etc.</li>
            <li>Hot and cold water wash rack</li>
            <li>Friendly atmosphere!</li>
          </ul>
          <p>Contact us if you'd like a barn tour!</p>

          <!--link "click here to go to prices"-->
             <a href="#horse-prices">Click here to go to prices</a>
          <br>
          <br>
        <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
        <br>
        <br>
  <a href="#trailer"><div class="arrow bounce">
        </div></a>
        </section>

      </div>

     <br>

   <!--div Two-->
            <div class="trailer-part">
              <section class="board-section-right-pic">
                <a name="trailer"> <h2>Trailer Parking</h2></a>
                 <p>Trailer parking space is available for a modest fee. Space is limited, so contact us if interested.</p>
                           <!--link "click here to go to prices"-->
                   <a href="#horse-prices">Click here to go to prices</a>
                   <br>
                   <br>
                  <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>

                  <br>
                  <br>
                  <br>
                  <br>
                  <a name="horse-prices"><h1>Our Service Prices</h1></a>
                  <p>Click on each service to find its price.</p>
                  <br/>
                  <accordian class="price-text"/>
                    <nuxt-link to="/horsefour" class="board-link">To Trainer Page</nuxt-link>
                    <br>
                    <br>
                    <a href="#volunteer"><div class="arrow bounce">
                    </div></a>
             </section>


             <img src="@/assets/images/trailerparking.jpg" alt="a trailer parked in the barn lot beside a boat" class="services-pic-two">
         </div>

      <!--div Three-->
       <div class="board-page">
           <img src="@/assets/images/ladieshorseinties.jpg" alt="a barn and a stable" class="services-pic-three">
         <section class="board-section-left-pic">
           <a name="volunteer"><h2>Volunteer Opportunities</h2></a>
             <p>For those who want to get the horse experience or just who enjoy working with horses, you can volunteer to work with the barn, arena or pasture areas. Contact us if interested.</p>
             <br>
             <br>
            <a href="#top">Back to Top</a>
            <nuxt-link to="/" class="board-link">Back to Home</nuxt-link>
         </section>

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
import accordian from '@/components/accordian';
export default {
  components: {
    'accordian': accordian
  },
  data() {
    return {
      show: false
    }
  }
};
</script>
<style media="screen">

.main-board-body {
  /*border: solid 10px magenta;*/
  display: flex;
  flex-direction: column;
}

.board-page {
  display: flex;
  flex-direction: row;
  margin-bottom: 5%;
}

.trailer-part {
  display: flex;
  flex-direction: row;
  margin-bottom: 5%;
}

.services-pic-one {
  height: 30%;
  width: 30%;
  border-bottom-right-radius: 50%;
  border-top-right-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
  }

.services-pic-two {
  height: 30%;
  width: 30%;
  border-bottom-left-radius: 50%;
  border-top-left-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
  margin-left: 10%;
}

.services-pic-three {
  height: 30%;
  width: 30%;
  border-bottom-right-radius: 50%;
  border-top-right-radius: 50%;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.5);
}

.board-section-left-pic {
  margin-top: 10%;
  margin-right: 10%;
  margin-left: 20%;
  margin-bottom: 20%
}

.board-section-right-pic {
  margin-top: 10%;
  margin-right: 5%;
  margin-left: 10%;
}

.board-link {
  font-size: 100%;
  margin-top: 50%;
  margin-bottom: 20%;
}

.price-text {
  cursor: pointer;
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

/*
@media only screen and (max-width: 360px) {
  .trailer-part {
    display: flex;
    flex-direction: column-reverse;
    width: 200%;
        }

}
*/

@media only screen and (max-width: 650px) {
  .board-page {
    display: flex;
    flex-direction: column;
    margin-bottom: 5%;
  }

  .trailer-part {
    display: flex;
    flex-direction: column-reverse;
            }

        .services-pic-two {
          margin-left: 50%;
      }

    .services-pic-three {
        height: 70%;
        width: 60%;
      }
}

@media only screen and (max-width: 768px) {
  .board-part {
    display: flex;
    flex-direction: column;
  }
  .arrow {
    display: none;
  }

  .trailer-part {
    display: flex;
    flex-direction: column-reverse;
      }

  .services-pic-two {
    margin-left: 50%;
}

.board-section-right-pic {
  margin-top: 10%;
  margin-right: 30%;
  margin-left: 30%;
}

}

</style>
