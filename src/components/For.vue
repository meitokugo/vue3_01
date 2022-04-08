<template>
  <div >
    <ul>
    <li v-for='name in names' :key='name.id'> 
          {{ name.text }}
        </li>
        </ul>
  </div>
</template>

<script>
export default {
  name: 'VFor',
    data(){
        return{
            names:[
                {text:'mike'},
                {text:'jack'},
                {text:'marry'}
            ]
        }
    }
}
</script>

