<template>
    <div class="Tab-ElementKey">
        <div class="Tab-Content">
            <span>
                member
            </span>
            <span>
                (2)
            </span>
        </div>
        <button @click='toggleBtn' v-if=true>
           {{ eyeHide?`&#x26D2;`:` &#128065;`  }}
        </button>
    </div>
</template>
<script>
export default {
    name: 'TanElementKey',
    data() {
        return {
            eyeHide: false
        }

    },
    methods: {
        toggleBtn() {
            this.eyeHide = !this.eyeHide
        }
    }
}

</script>
<style scoped>
.Tab-ElementKey {
    width: max-content;
    display: flex;
    border-radius: 4px;
    border: 2px gray solid;
    cursor: pointer;
}

.Tab-Content {
    display: inline;
    padding: 8px;

}

span {
    padding: 2px 6px 2px 6px;
    color: #ff6b00;
}

button {
    width: 28px;
    height: auto;
    border: none;
    background-color: #dddfe1;
    ;
}
</style>