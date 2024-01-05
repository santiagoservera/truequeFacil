<template>
    <div class="card-header">
        <div class="row">
          <div class="col-2 col-sm-1">
  
            <img class="avatar-img"
             :src="header.picture" 
             alt="avatar">
  
          </div>
          <div class="col-7 col-sm-9 text-center">
            <h5 class="card-header-title m-0">
              
              <router-link to="/profile">{{ header.name }}</router-link>
              
            </h5>
            <small class="text-muted card-header-subtitle">hace 10 minutos</small>
  
          </div>
         
  
  
        </div>
  
      </div>
</template>

<script>
export default {
    name:"CardHeader",
    props:["header"]
}
</script>

<style scoped>
.avatar-img{
    width: 40px;
    height: 40px;
    object-fit: cover;
    border-radius: 50%;
    
  }
  
  .card-header-title{
    line-height: 1;
    
    
  }
  
  .card-header-subtitle{
    font-size: 0.8em;
    
  }
  
  @media (min-width: 576px){
  
    .card-header .col-8{
      margin-left: 0.5em;
  
    }
  
  }
  
  .card-header{
    background-color: transparent;
    padding: 0.5rem 1rem;
    padding-bottom: 0;
    border-bottom: none;
  }
  
  .more-btn {
    border-radius: 50%;
    padding: 0.5em;
    margin: 0.3em;
  
  }
</style>