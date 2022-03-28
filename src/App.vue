import '../public/font'
<template >
  <div>
    <header-form/>
    <headerForm :cart="0"/>
    <header-content/>
  </div>
    <div>
    <headerAbout :Num="'7+'" :Text="'Years of experience'" :About="'Working with Alex was interesting. He went above and beyond what I\'ve asking for and provided such an amazing design for my mobile application.'" />
    </div>
    
   <!-- <div v-for="(item, ind) in data" :key="ind">
    <headerAbout :Text="item.text" :Num="item.num"/>
  </div> -->
  
</template>



<script>
import headerForm from '../componets/headerNav.vue';
import headerContent from '../componets/headerContent.vue';
import headerAbout from '../componets/headerAbout.vue';
// import headerCom from '../componets/headerAbout.vue'
// import headerAboutCom from '../componets/headerAboutcom.vue';


export default {
  name: "App",
  components: {
    headerForm,
    headerContent,
    headerAbout,
    // headerAboutCom,
  },
  
  data() {
    return {
        cart:0,
        // data: [
        //   {
        //     num: '7+',
        //     text:'Years of experience',
        //   },
        //   {
        //     num:'50+',
        //     text:'Projects completed',
        //   },
        //   {
        //     num:'30+',
        //     text:'Happy clients',
        //   },
        // ]
    }
  },
  methods: {
   
  },

}

</script>



<style >

    
</style>