<template>
    <div class="Tab-ElementKeyValue">
        <div class="TEKV-container">

            <div v-for="(value,key) in mockData"  :key="key">
                <span class="TEKV-key">{{ key }}</span>
                <span> : </span> 
                <span class="TEKV-value">" {{ value.slice(0, 25) }}{{ value.length>25?'...':"" }} "</span>
                </div>
        </div>

    </div>
</template>
<script>
import TabElementKeyVue from './TabElementKey.vue'
export default {
    name: 'TabElementValue',
    components: [
        TabElementKeyVue
    ],
    data(){
        return {
            mockData:{ bookName: "Book 11 dovnsdnndovnsdnnsodnvobdovnsdnnsodnvo bdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnn sodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvobdovnsdnnsodnvob", auother: "auother 1", number: "numbers", email: "email", png: './assert/1.jpg' }
        }
    }
    ,
}
</script>
<style scoped>
.Tab-ElementKeyValue {
    width: max-content;
    display: flex;
    border-radius: 4px;
    border: 2px gray solid;
    cursor: pointer;
}
.TEKV-container{
    display: block;
    min-width: 100px;
    max-width: 500px;
    padding: 20px;
    text-align: left;
}
span{
padding: 0px 4px 0px 4px;
}
.TEKV-key {
    color: #ff6b00;
}
.TEKV-value {
    color: #01a828;
}
</style>