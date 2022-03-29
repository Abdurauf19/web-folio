import '../public/font'
<template >
  <div>
    <header-form/>
    <headerForm :cart="0"/>
    <header-content/>
    <headerAbout  :Num="'7+'" :Text="'Years of experience'" :About="'Working with Alex was interesting. He went above and beyond what I\'ve asking for and provided such an amazing design for my mobile application.'" />
  </div>

  <div v-for="(item, index) in datas" :key="index" >
    <main-portfolio :portfolioTitle="item.titlee" :portfolioText="item.textt"/>
  </div>

    <div v-for="(item, index) in data" :key="index">
        <mainPortfolioImg :text="item.text" :title="item.title" :img="item.img" :btn="item.btn" />
    </div>
    
    
  
</template>



<script>
import headerForm from '../componets/headerNav.vue';
import headerContent from '../componets/headerContent.vue';
import headerAbout from '../componets/headerAbout.vue';
import mainPortfolio from '../componets/mainPartfolio.vue';
import mainPortfolioImg from '../componets/_mainPortfolioImg.vue'
import mainServise from '../componets/mainServise.vue'



export default {
  name: "App",
  components: {
    headerForm,
    headerContent,
    headerAbout,
    mainPortfolio,
    mainPortfolioImg,
    mainServise,
  },
  
  data() {
    return {
        cart:0,
        // Main portfolio
       data: [
         {
           title:"Maize Website Design",
           text:"Vivamus mattis eu odio non aliquam. Vestibulum tristique congue laoreet. Nulla facilisi.",
           img: require('../photos/portfolioimg/portolio2.png')
         },
         {
           title:"Datadash Product Design",
           text:"Vivamus mattis eu odio non aliquam. Vestibulum tristique congue laoreet. Nulla facilisi.",
           img: require('../photos/portfolioimg/portolio1.png')
         },
         {
           title:"Joggr Website Design",
           text:"Vivamus mattis eu odio non aliquam. Vestibulum tristique congue laoreet. Nulla facilisi.",
           img: require('../photos/portfolioimg/portolio3.png')
         },
         {
           title:"Origin UI/UX Design",
           text:"Vivamus mattis eu odio non aliquam. Vestibulum tristique congue laoreet. Nulla facilisi.",
           img: require('../photos/portfolioimg/portolio4.png'),
           btn: "View All Project"
         },
         {
           title:"Otsuka Pharmaceutical",
           text:"Vivamus mattis eu odio non aliquam. Vestibulum tristique congue laoreet. Nulla facilisi.",
           img: require('../photos/portfolioimg/portolio5.png'), 
         },
       ], 
       datas :[
         {
           titlee:"Work",
           textt: "Bringing stellar results for every client."
         },
         
       ]   
    }
  },

  methods: {
    
    },

}

</script>


<style >

</style>

