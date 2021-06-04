<template>
    <div>
        Parent component
        <button @click="showChild = !showChild">togglechild</button>
    <Child v-if="showChild" />
        </div>

</template>
<script>
import Child from './Child.vue'
export default{
    components:{Child},
    name:'parent',
    data(){
        return{
            showChild:true,
        }
    },
    beforeCreate(){
        console.log('parent beforeCreate()')
    },
    created(){
        console.log('parent Created()')
    },
    beforeMount(){
        console.log('parent beforeMount()')
    },
    mounted(){
        console.log('parent mounted()')
    },
    beforeUpdate(){
        console.log('parent beforeUpdate()')
    },
    updated(){
        console.log('parent updated()')
    },
    beforeDestroy(){
        console.log('parent beforeDestroy()')
    },
    destroyed(){
        console.log('parent destroyed()')
    },
}
</script>