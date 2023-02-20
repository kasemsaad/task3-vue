
<template>
  <Nav-Bar1></Nav-Bar1>
  <Head1></Head1>
  <section class="pt-4">
  <div class="container px-lg-5"> 
       <div class="row gx-lg-5">
  <Section1 v-for="person in box" :person="person"></Section1>
</div>
    </div>
</section>
  <Footer1></Footer1>
</template>

<script>
import NavBar1 from "./components/NavBar1.vue";
import Head1 from "./components/Head1.vue";
import Section1 from "./components/Section1.vue";
import Footer1 from "./components/Footer1.vue";

export default {
  data() {
        return {
          box:[
                 { title:"Fresh new layout",
                   urlimg:            "bi bi-collection"       ,
                  disc:"With Bootstrap 5, we've created a fresh new layout for this template!",
},
{ title:"Free to download",
                   urlimg:            "bi bi-cloud-download"       ,
                  disc:"As always, Start Bootstrap has a powerful collectin of free templates.",
}, { title:"Jumbotron hero header",
                   urlimg:            "bi bi-card-heading"       ,
                  disc:"The heroic part of this template is the jumbotron hero header!",
}, { title:"Feature boxes",
                   urlimg:            "bi bi-bootstrap"       ,
                  disc:"We've created some custom feature boxes using Bootstrap icons!",
}, { title:"Simple clean code",
                   urlimg:            "bi bi-code"       ,
                  disc:"We keep our dependencies up to date and squash bugs as they come!",
}, { title:"A name you trust",
                   urlimg:            "i bi-patch-check"       ,
                  disc:"Start Bootstrap has been the leader in free Bootstrap templates since 2013!",
},
          ]
        }

  },
  components: {
    NavBar1,Head1,Section1,Footer1,
  },
};
</script>

