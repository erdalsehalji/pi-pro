<template>

  <div id="app">

  
      <div class="bg-white">
        <div class="container">
          <div class="row">
            <div class="col">
              <nav class="navbar navbar-expand-lg navbar-light mb-2">
                <router-link class="navbar-brand" to="/"></router-link>
              </router-link>
              <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
            
              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <form class="form-inline my-2 my-lg-0 mr-auto ml-5">
                  <input v-model="searchTerm" class="form-control mr-sm-2" type="search" placeholder="Trazi nesto" aria-label="Search">
                </form>
                <router-link v-if="!authenticated" class="btn btn-info my-2 my-sm-0 mr-2" to="/login">Login</router-link>
                <span v-if="authenticated">
                  {{ userName }}
                  <a @click="logout" class="btn btn-info my-2 my-sm-0 mr-2" href="#">Logout</a>
                </span>
                <router-link class="btn btn-outline my-2 my-sm-0 mr-2" to="/signup">Signup</router-link>
            </div>
          </nav>
        </div>
      </div>
    </div>
    </div>

      <div class="container">
 
        <router-view/>
        

        

    </div>

    <div id="footer" class="text-center mt-5">Ovo je footer. (c) 2019 mi svi skupa.</div>
  </div>
</template>

<script type="text/javascript">


export default {
  data () {
    return store;
  },

  methods: {
    logout() {
      store.authenticated = false
    }
  }
}
</script>

<style lang="scss">
body {
  background-color: rgba(var(--b3f,250,250,250),1)
}

.bg-white {
  background-color: lightcoral;
  border-bottom: lightcoral;
  margin-bottom: 20px;
  padding: 10px;
}

nav.navbar {
  background-color: white;
}
</style>
