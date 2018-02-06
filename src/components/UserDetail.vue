<template>
    <div class="component">
        <h3>Name</h3>
        <p>Many Details</p>
        <p>{{Name.email}}</p>
        
        

        <div></div>
       
        
        
    </div>  
</template>

<script>
export default{
    props:['Name']
    

}
          
      

    
</script>

<style scoped>
    div {
        background-color: lightcoral;
    }
</style>
