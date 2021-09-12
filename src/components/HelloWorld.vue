
<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    

    <div class="container">
      <div class="row">
        <div class="col-6">

          <ul class="list-group" :id="dynamicId"
          >
            <li class="list-group-item" :class="dynaclass">This is an item</li>
            <li class="list-group-item">This is an item</li>
            <li class="list-group-item">This is an item</li>
          </ul>
              <br />
              <br />

          <h2> {{ theNumber }} </h2>  
          <button class="btn btn-primary" @click="increment">
            Increment
          </button>

          <button class="btn btn-danger" @click="decrement">
            Decrement
          </button>

          <br />
          <button class="btn btn-success" @click="incrementbyten">
            Increment + 10
          </button>
          <button class="btn btn-danger" @click="decrementbyten">
            Increment - 10
          </button>
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
      name: "arjun hadke",
      dynamicId: 'this-just-changed',
      dynaclass: 'the-dynamic-class',
      theNumber: 0,

      author: {
        name: 'John Doe',
        books: [
          'Vue 2 - Advanced Guide',
          'Vue 3 - Basic Guide',
          'Vue 4 - The Mystery'
        ]
      }
    }
  },

  created() {
    console.log('created');
  },

  methods: {
    

    // decrement() {
    //   this.theNumber--;
    // },

    incrementbyten() {
      this.theNumber = this.theNumber + 10;
    },

    decrementbyten() {
      this.theNumber = this.theNumber - 10;
    }

    
  },

  computed: {
      // eslint-disable-next-line vue/return-in-computed-property
      compfunction() {
        console.log("hello there");
      },

      decrement() {
        return this.theNumber--;
      },
  }

  
}
</script>



// all the styles below
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
