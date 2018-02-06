<template>
    <div class="component">
        <h1>The User </h1>
       
       


         
  


            
        <div>
        
  </div>
        
        
        
        <div class="row">
            <div class="col-xs-12 col-sm-6">
                <app-user-detail></app-user-detail>
            </div>
            <div class="col-xs-12 col-sm-6">
                <app-user-edit 
                ></app-user-edit>
            </div>
        </div>
    </div>
</template>

<script>
    import UserDetail from './UserDetail.vue';
    import UserEdit from './UserEdit.vue';

    import axios from 'axios';

    export default {


            components: {
            appUserDetail: UserDetail,
            appUserEdit: UserEdit
        },
 

    data() {
       return {
           url:String,
            posts: [],
            errors: []
    }
  },
  methods:{
    id(arg) {
        this.url= `https://jsonplaceholder.typicode.com/comments/?id=${arg}`;
        console.log(this.url)./UserDetail.vue';
    import UserEdit from './UserEdit.vue';

        axios.get( this.url)
        .then(response => {

        this.posts = response.data
        console.log(this.posts)
        })
        .catch(e => {
        this.errors.push(e)
        })
            }
    }

 
    }


   
      
    
</script>

<style scoped>
    div {
        background-color: lightblue;
    }
</style>
