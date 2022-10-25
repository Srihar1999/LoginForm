<style>
body{
    background-color:tomato;
}
  .message{
    padding-bottom: 20px;
    font-weight: bold;
  }
</style>
<template>
<center>
<table bgcolor="white" border="10px" width=30% >
<center>
<p style="color:red"><b>Random Number</b> <br><br> <table border="1px" width=30%><tr><center><td style="color:green"> {{randomNumber}}</td></center> </tr>  </table></p>
</center>
 <div class="message">
  <center>
  <button style="color:green" @click="random()">Random Number</button><br><br>
  <button><div @click="clear" class="btn">clear</div></button>
  </center>

<center>
<br>
<input type="number" name="input" v-model="input">
</center>
 <center>
    <br>
 <button v-on:click="getAdd()">add</button>
 <button v-on:click="getSub()">sub</button>
 <h1>{{count}}</h1>
 </center>
  </div>
  </table>
  </center>
</template>
<script>
export default {
    name:'MySri',
  data: ()=> {
    return {
        randomNumber:'',
        input:'1',
        count:0
    }
 
  },
  methods: {
     clear() {
      this.randomNumber = '';
      this.count='';
      this.input='';
    },
    random (){
        this.randomNumber = Math.floor(Math.random()*(100-1+1)+1);
    },
    getAdd(){
        this.count=parseInt(this.randomNumber)+parseInt(this.input)
    },
    getSub(){
        this.count=parseInt(this.randomNumber)-parseInt(this.input)
    }
  }
}
</script>

