<template>
    <TanElementKey></TanElementKey>
    <TabElementKeyValue></TabElementKeyValue>
    <TabElementValue></TabElementValue>
</template>

<script>
import TanElementKey from '../components/tab-element/TabElementKey.vue'
import TabElementKeyValue from '../components/tab-element/TabElementKeyValue.vue';
import  TabElementValue from '../components/tab-element/TabElementValue.vue'
export default{

    name:'MainPage',
    components:{
        TanElementKey,
        TabElementKeyValue,
        TabElementValue
    }
}
</script>