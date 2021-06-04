<template>
<div>Child-component</div>
</template>
<script>
export default{
    name:'Child',
    beforeCreate(){
        console.log('child beforeCreate()')
    },
    created(){
        console.log('child created()')
    },
    beforeMount(){
        console.log('child beforeMount()')
    },
    mounted(){
        console.log('child mounted()')
    },
    beforeUpdate(){
        console.log('child beforeUpdate()')
    },
    updated(){
        console.log('child updated()')
    },
    beforeDestroy(){
        console.log('child before()')
    },
    destroyed(){
        console.log('child destroyed()')
    }
}
</script>