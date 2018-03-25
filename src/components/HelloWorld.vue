<template>
  <div class="hello">
    
  </div>
</template>

<script>
import {Line} from 'vue-chartjs'

export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted(){
     this.renderChart({
          labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July'],
          datasets: [
            {
              label: 'Data One',
              backgroundColor: '#FC2525',
              data: [40, 39, 10, 40, 39, 80, 40]
            },{
              label: 'Data Two',
              backgroundColor: '#05CBE1',
              data: [60, 55, 32, 10, 2, 12, 53]
            }
          ]
        }, {responsive: true, maintainAspectRatio: false})

      }
   
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
