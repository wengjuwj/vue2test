<template>
  <div>
     <button @click="test" style="background:green;color:#fff">测试vue链接</button>
  </div>
</template>

<script>
import {login} from '@/api/test.js'
export default {
  data(){
    return{

    }
  },
  methods:{
    test(){
       login({}).then(response => {
          
        }).catch(error => {
          // reject(error)
        })
    }
  }

}
</script>

<style>

</style>