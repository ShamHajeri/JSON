<template>
    <div class="Tab-ElementValue">
        <span> {{ data.slice(0,25) }}{{ data.length>25?'...':'' }} </span>
    </div>
</template>
<script>

export default {
    name:'TabElementValue',
    data(){
        return{
            data:"bjcbaksjbjbsajkbjkasbkjcbsjbjsabkcbsabckjsabsa"
        }
    }
    
}
</script>
<style scoped>
.Tab-ElementValue{
    width: max-content;
    display: flex;
    border-radius: 4px;
    border: 2px gray solid;
    cursor: pointer;
}
span{
    padding: 10px 15px 10px 15px;
    color: #07701c;

}
</style>
