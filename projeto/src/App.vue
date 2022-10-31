<template>
  <div id="app" class="d-flex flex-column">  
    <Navbar />
    <div class="container flex-grow-1 mt-5 mb-5 py-2">
      <div class="row">
        <div class="col-md-4 col-sm-12 mx-auto">
          <div class="card">
            <div class="card-header">
              <h3 class="text-success">
                Faça o upload o arquivo aqui
              </h3>
            </div>
            <div class="card-body">
              <form>
                <SingleUploader label="Upload" />
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Layouts/Navbar.vue';
import SingleUploader from './components/Uploader/SingleUploader.vue'
import Footer from './components/Layouts/Footer.vue';

export default {
  name: "App",
  components:{
    Navbar,
    SingleUploader,
    Footer,
  }
}
</script>