<template>
  <nav class="navbar navbar-expand-lg  bg-success">
    <div class="container justify-content-evenly">
      <router-link :class="{ active : activePath.posts }"  to="/" class="nav-link "><span class="material-icons-round">
        home
      </span>
      </router-link>

      

      <router-link :class="{ active : activePath.about }" to="/about" class="nav-link "><span class="material-icons-round">
          info
        </span>
      </router-link>

      <router-link :class="{ active : activePath.home }" to="/home" class="nav-link "><span class="material-icons-round">
        person
      </span>
      </router-link>





    </div>

  </nav>
</template>


<script>
export default {
  name: "NavComp",
  computed:{
    activePath(){
      if (this.$route.path === '/'){

        return {
        home:false,
        about:false,
        posts:true,
        }

      } else if (this.$route.path === '/about'){
        return {
        home:false,
        about:true,
        posts:false,
        }

      } else if (this.$route.path === '/home'){
        return {
        home:true,
        about:false,
        posts:false,
        }
      
      } else if (this.$route.path === '/createAcount'){
        return {
        home:true,
        about:false,
        posts:false,
        }

      }else{
        return {
        home:false,
        about:false,
        posts:false,
        }
      }
      
        
      }
    },

 
}
</script>

<style scoped>
.material-icons-round {
  color: white;
  font-size: 1.4em;
  background-color: rgba(128, 128, 128, 0.356);
  padding: 0.3em;
  border-radius: 50%;
  margin: 0.1em;
}

.active .material-icons-round {
  color: rgb(255, 255, 255);
  background-color: #65A386;
  border: 1px solid rgb(116, 116, 116);
}

.navbar {
  padding-bottom: 0;
  padding-top: 0;
}

.nav-link {
  padding: 0.2rem 1rem;
}
</style>


