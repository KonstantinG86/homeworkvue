<template>
    <div class="cart">
        <div class="cart__number">
            {{ index }}
        </div>
        <div class="cart__text">
            <h3>{{ title }}</h3>
            <p>{{ text }}</p>
        </div>
    </div>
</template>


<script>
    export default {
        name: 'cardsList',
        props: [
            'index',
            'title',
            'text'
        ],
        data() {
            return {
            }
        }
    }
</script>


<style>
    .cart {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: 24px;
        padding: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
        max-width: 268px;
        max-height: 170px;
        gap: 16px;
    }
    .cart__number {
        font-size: 18px;
        font-weight: 400;
        color: #3C3C43;
        background-color: #DEDEDE;
        border-radius: 50%;
        width: 32px;
        height: 32px;
        padding: 4px 10px;
        text-align: center;
    }
    .cart__text {
        display: flex;
        flex-direction: column;
        gap: 8px;
    }

</style>