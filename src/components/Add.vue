<style>
  .message{
    padding-bottom: 20px;
    font-weight: bold;
  }
</style>
<template>
    <div id="app">

            <input type="number" name="number1" v-on:input= "update_number1">
            <p>{{ number1 }}</p>
            <input type="number" name="number2" v-on:input= "update_number2">
            <p>{{ number2 }}</p>
            <hr>
            <p>{{ result() }}</p>

    </div>
</template>
<script>
// import { defineComponent } from '@vue/composition-api'

// export default defineComponent({
//     setup() {
        
//     },
// })

export default({
      name: 'MyAdd',
      data: ()=> {
        return{
            number1: 0,
        number2: 0,
            
        }
        
      },
      methods: {
        update_number1: function (event) {
          this.number1 = event.target.value;
        },
        update_number2: function (event) {
          this.number2 = event.target.value;
        },
        result: function () {
    
          return this.number1 + this.number2;
        },
    
      },
    });
</script>
