<template>

<button @click.left="AlertL" @click.right="AlertR">左边 | 右边</button>
    <p>左右键不同弹窗</p>

</template>

<script>
export default {
    name:'choose',
        data(){
            return{

                }
            },
            methods:{
        AlertL:function(){
            alert("you click left ")
        },
        AlertR:function(){
            alert("you click right")
        }
            }
}
</script>

