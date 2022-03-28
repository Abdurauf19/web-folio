import '../public/font'
<template >
  <div>
    <header-form/>
    <headerForm :cart="0"/>
    <header-content/>
  </div>

    <headerAbout :About="'Working with Alex was interesting. He went above and beyond what I\'ve asking for and provided such an amazing design for my mobile application.'" />
    <!-- <headerAbout :Num ="'7+'"/>
    <headerAbout :Text ="'Years of experience'"/> -->
   <div  v-for="(item, ind) in data" :key="ind">
    <headerAboutCom :Num="item.num"/>
    <headerAboutCom :Text="item.text"/>
  </div>
  
</template>



<script>
import headerForm from '../componets/headerNav.vue';
import headerContent from '../componets/headerContent.vue';
import headerAbout from '../componets/headerAbout.vue';
import headerAboutCom from '../componets/headerAboutcom.vue';


export default {
  name: "App",
  components: {
    headerForm,
    headerContent,
    headerAbout,
    headerAboutCom,
  },
  
  data() {
    return {
        cart:0,
        data: [
          {
            num: '7+',
            text:'Years of experience',
          },
          {
            num:'50+',
            text:'Projects completed',
          },
          {
            num:'30+',
            text:'Happy clients',
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