<template>
  <div>
   <ToggleButton/>
   <ul>
     <li v-for="tweet in tweets" :key="tweet">{{ tweet }}</li>
   </ul>
  </div>
</template>

<script>
  import ToggleButton from '../components/ToggleButton.vue'
  export default {
    name: "TweetSelection",
    data: function(){
      return {
        tweets: [
          {
          postContent: "Hi I'm John and I'm posting on 04/10/2022",
          datePosted: "04/10/2022",
          authorName: "John"
          },
          {
          postContent: "Hi I'm Jane and I'm posting on 04/09/2022",
          datePosted: "04/09/2022",
          authorName: "Jane"
          },
          {
          postContent: "Hi I'm Jim and I'm posting on 04/08/2022",
          datePosted: "04/08/2022",
          authorName: "Jim"
          },
          {
          postContent: "Hi I'm James and I'm posting on 04/07/2022",
          datePosted: "04/07/2022",
          authorName: "James"
          }
        ]
      }
    },
    // data: function makeGrid(){

    // },
    components: {
      ToggleButton,
    },
    props: {
      authorName: String,
      datePosted: String,
      postContent: String
    },
    // methods:{
    //   makeGrid: function(){
    //     let toggleButton = document.getElementById('toggleButton');
    //     toggleButton.addEventListener('click', makeGrid);
    //     // makeGrid function needs to be made
    //   }
    // }
  }
</script>

<style scoped>
/* create a variable with a few tweets and extra info, then the actual bulk of the assignment is to add a toggle button to switch between grid and list, do it through class binding */
li{
  background-color: bisque;
  margin: 5px;
  padding: 5px;
}
</style>