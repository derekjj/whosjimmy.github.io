<template lang="pug">
  .container-fluid
    .col-md-12.row
      .col-md-6(v-for="clock in clocks")
        appGallery(:cover="clock.images[0]" :images="clock.images" :info="[clock.name, clock.info, clock.description]")
    .row.text-center
      .col-lg-12
        | Click on an image, to view image gallery.
  </div>

</template>
<script>
  import Gallery from '~/components/Gallery.vue'
  export default {
  components: {
    appGallery: Gallery
  },
  data() {
    return  {
      clocks : [
      {
        name: 'E1 "Angela"',
        info: '7 Diameter X 16H ~ inches',
        description: 'First Edition Clock built from P3, 3 units made.',
        images: [
          "img/clocks/e1/may07all 210-1.jpg",
          "img/clocks/e1/may07all 220-1.jpg",
          "img/clocks/e1/may07all 202-1.jpg",
          "img/clocks/e1/may07all 057.jpg", 
          "img/clocks/e1/may07all 054.jpg",
          "img/clocks/e1/129-2911_IMG-1.jpg"
        ]
      },
      {       
        name: 'Prototype 7 "Robo-Retro"',
        info: '9L X 10D X 12H ~ inches',
        description: "I am building 4 beautiful re-creations of the prototype featured here called Robo-Retro. They will be set on an oiled walnut base, with a clear face and a clear acrylic cover with set and reset buttons on top. The wiring will be neat and channeled in raceways (not the birds nest on the prototype) This clock is part of my \"ode to the 20th century statement, using electro-mechanical components with technology from the 1950's or older. It's an elaborate way to tell time, buy perfectly accurate by using a syncronous motor syncronized to the line frequency. The counting relays are brand new but 40 years old and obsolete, neon lights and led's for the minutes and hours and operating on a 12 hour cycle. The cost for one of these art pieces is 25,000 us dollars and 6 month delivery, a 40% deposit will secure one in your name, there are NO modern electronics in this time piece, it operates on 120 volts 50 or 60 cycle and uses 6 watts of power. This clock is made by the same head, heart and hands that created all the work featured on this site, and movie props that I'm sure you have seen. jimmy claws",
        images: [
          "img/clocks/p7/vancouver2013a1 1841.JPG",
          "img/clocks/p7/IMG_0509.JPG",
          "img/clocks/p7/IMG_0511.JPG",
          "img/clocks/p7/IMG_0516.JPG",
          "img/clocks/p7/IMG_0519.JPG",
          "img/clocks/p7/IMG_0617.JPG"
        ]
      },
      {
        name: 'Prototype 4 "Little Jimmy"',
        info: '9L X 2D X 3H ~ inches',
        description: "This 12 hour clock is designed and crafted by \"Jimmy Claws\", 4 will be built because I only have 4 of the clock movements available, they will be numbered and signed 1 through 4. The body will be one-piece, carved in walnut, smoothed and oiled, the battery will be hidden under the base and will last a year. Accuracy of the movement is tunable by you, therefore it will keep one amused for some time! The movement will NOT be enclosed, so you can see the oscillating wheel and upon first viewing one may ask \"is that a clock\" The price for one of these limited time pieces is 2,500 us dollars and delivery is 100 days and counting down, a 40% deposit puts your name on one. jimmy claws",
        images: [
          "img/clocks/p4/hiatus 411.JPG",
          "img/clocks/p4/IMG_0650.JPG",
          "img/clocks/p4/IMG_0668.JPG",
          "img/clocks/p4/IMG_0700.JPG",
        ]
      },
      {  
        name: 'Prototype 5 "Sidewinder"',
        info: '7L X 3D X 3H ~ inches',
        description: "This clock is open production, meaning not limited, a product I will continue to offer. What will vary mostly will be the materials and the shapes of the bodies, my \"jimmy screw\" and pin/gear assemblies will be fairly constant. This began as p5,( please review the pictures in the p5 file in the clock gallery) and all will use a very common quartz movement, proven to be very accurate, and easy to replace .The pin gears are an old design I borrowed from a Dutch windmill. All of the screws used in \"jimmy clocks\" are machined on the Jimmy Mill, a 4 axis milling machine that Jimmy built, the same machine that made Wolverine's claws. The clear version shown is made from laminated polycarbonate and will NOT be used, instead acrylic will be used for the clear version, it's as clear as glass, assorted woods will also be offered and corian. The cost for these starts at 450 us dollars made in Corian, 550 in Walnut, 750 in acrylic and 1100 dollars crafted from Cocobolo, while I can get it! 4 weeks delivery Please make ordering arrangements through our e-mail for now, thanks jimmy claws",
        images: [
          "img/clocks/p5/IMG_9123.JPG",
          "img/clocks/p5/Dec.21 2010 365.JPG",
          "img/clocks/p5/Dec.21 2010 370.JPG",
          "img/clocks/p5/IMG_9159.JPG",
          "img/clocks/p5/IMG_9163.JPG"
        ]
      },
      ]
    }
  }
}
</script>

<style scoped>
  .hidden {
    visibility: hidden;
  }
  .row {
    margin-top: 10px;
  }
</style>

