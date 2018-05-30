<template>
<v-container fluid fill-height bg-image>
  <v-layout column>
<v-layout column wrap   >

  <v-flex xs12 >

  <img class="portal-image"
                  
                  src="~/assets/images/support/portal.png"
                  alt=""
                  height="150"
                  width="300"
                >   
 </v-flex>

</v-layout>

 

 
  
 

   <v-layout justify-space-around   > 
    <v-flex xs2>  
    
     <router-link to="/support">  <ServiceCard class=""
     :subject="'Support'"> 
       
       <img slot="hp-image"
                  
                  src="~/assets/images/support.png"
                  alt=""
                >   
<li slot="link1">log a call</li>
<li slot="link2">ask for help </li>

       
       
       </ServiceCard></router-link>

       </v-flex>


<v-flex xs2> 

    <nuxt-link to="/requests">    <ServiceCard class=""
      :subject="'requests'">

      <img slot="hp-image"
                  
                  src="~/assets/images/requests.png"
                  alt=""
                >   

      <li slot="link1">new user </li>
<li slot="link2">changes</li>

      
     
      
       </ServiceCard></nuxt-link>

</v-flex>

<v-flex xs2> 

     <nuxt-link to="/forms">  <ServiceCard class=""
      :subject="'Forms/Templates'">

        
       <img slot="hp-image"
                  
                  src="~/assets/images/forms.png"
                  alt=""
                > 
      
      
      
       </ServiceCard></nuxt-link>
</v-flex>

<v-flex xs2> 
    <nuxt-link to="/policies">   <ServiceCard class=""
      :subject="'Policies/Procedures'"
       :listItem1="'option 1'"
      :listItem2="'option 2'"
      :listItem3="'...more'">
      
        <img slot="hp-image"
                  
                  src="~/assets/images/policies.png"
                  alt=""
                > 
      
      </ServiceCard></nuxt-link>

</v-flex>
<v-flex xs2> 
    <nuxt-link to="/maps">    <ServiceCard class=""
      :subject="'Maps'">
       
       <img slot="hp-image"
                  
                  src="~/assets/images/maps2.png"
                  alt=""
                > 
        <li class="text-faded" slot="link1">training </li>
<li slot="link2">productivity</li>

      
       </ServiceCard></nuxt-link>

     </v-flex>  
      </v-layout>
 
 </v-layout>
    </v-container>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import ServiceCard from '~/components/ServiceCard.vue'

export default {
   layout: 'support',
  components: {
    Logo,
    VuetifyLogo,
    ServiceCard
  },

  data() {

    return {

      


    }

  }
}
</script>


<style  scoped>

.bg-image{

background: url(~/assets/images/bg.jpeg) ;
   background-repeat: no-repeat;
    background-size: cover;

}



a{text-decoration:none;
  color: rgba(255, 255, 255, 0.9);

}

  a:hover  {
  
    background-color: rgba(255, 255, 255, 0.5);
  
  }
  
   a:hover > .panel-heading{

     color: rgba(145, 101, 126);
   }


.text-faded {
  color: rgba(255, 255, 255, 0.9);
}

li:before {
  content: "✓";
  padding-right: 10px;
  text-align: left;
}


.portal-image{

  margin-top: 120px;
  margin-left:10px;
}


</style>



