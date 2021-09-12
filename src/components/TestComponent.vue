
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    
    
    <div class="container">
      <div class="row">
        <div class="col-6">

          <ul class="list-group" 
          >
            <li class="list-group-item">This is an item</li>
            <li class="list-group-item">This is an item</li>
            <li class="list-group-item">This is an item</li>
          </ul>

        </div> <!--col-->
      </div> <!--row-->
    </div> <!--container-->
  </div> <!--hello-->
</template>
// everything in the browser goes inside the template



// all the code logic below in the script tag
<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },

  data() {
    return {
      name: 'Arjun Hadke'
    }
  }
}
</script>



// all the styles below
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
