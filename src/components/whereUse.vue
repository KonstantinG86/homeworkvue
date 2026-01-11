<template>
    <div class="whereUse">
        <div class="whereUse__text">
            <h3>{{ title_use }}</h3>
            <p>{{ text_use }}</p>
        </div>
        <div class="whereUse__buttons">
            <button 
            v-for="value in buttons_use"
            :key="value">
                {{ value }}
            </button>
        </div>
    </div>
</template>


<script>
    export default {
        name: 'whereUse',
        props: [
            'title_use',
            'text_use',
            'buttons_use'
        ],
        data() {
            return {
            }
        }
    }
</script>


<style>
    .whereUse {
        display: flex;
        flex-direction: column;
        gap: 32px;
        align-items: center;
        margin: 24px;
        padding: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
        max-width: 508px;
        max-height: auto;
    }
</style>