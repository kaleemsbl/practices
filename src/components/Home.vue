<template>
<div>
    <h1 v-if="show">This is the first component</h1>
    <h2>{{ kaleem }}</h2>
    </div>
    <button v-on:click="hello">toggle</button>
</template>
<script>
export default{
    name: 'Home',
    props:{
        kaleem: String
    },
    data()
        {
             return{show:false}
        },
        methods:{
            hello(){
            this.show=!this.show
        }
        }

}
</script>

<style scoped>
button {
  margin: 25px 5px 20px 20px;
}

</style>
