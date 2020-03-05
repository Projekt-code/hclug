<template>
  <Layout>
    <section class="section">
    <div class="columns">
      <div class="column is-one-third">
        <figure class="image">
          <g-image alt="Logo" src="~/Logo.png" />
        </figure>
      </div>
      <div class="column is-two-thirds has-text-centered">
        <figure class="image">
          <g-image :alt="images[showID].text" :src="images[showID].src"/>
        </figure>
      </div>
    </div>
    </section>
    <section class="section has-background-white">
      <div class="columns">
        <div class="column">
          <h2 class="title has-text-centered">Join Us</h2>
          <p>Our meetings are the first and third Thursdays of each month. Check out our Meet Up or Slack Group for more details.</p>
        </div>

        <div class="column">
          <h2 class="title has-text-centered">About Us</h2>
          <p>We are a group of enthusiastic people ranging from students to professional experts willing to teach and foster the growth of Linux.</p>
        </div>
      </div>
      
    </section>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Hello, world! Err, I mean HCLUG"
  },
  data(){
    return {
      showID: 0,
      images: [
        {id: 0, src: "/images/term.gif",text: ""},
        {id: 1, src: "https://media.giphy.com/media/xUOxeZWKz8sD7SphGo/giphy.gif",text: "JS"},
        {id: 2, src: "https://media.giphy.com/media/mpF9fbOySV7aw/giphy.gif",text: "WATWWA"}      
      ]
    }
  },
  mounted(){
    setInterval(()=>{
      this.changeID();
    },3000)
  },
  methods:{
      changeID(){
        if(this.showID == 0){
          this.showID = Math.floor(Math.random() * 5)
        }else{
          this.showID = 0
        }
        
      }
    }
};
</script>
