<template>
    <div class="futers">
        <div class="futers__title">
            <h3>Основные возможности</h3>
        </div>
        <div class="futers__items">
            <div class="futers__items-item"
            v-for="(value) in data">
                <img :src='value.img' :alt='value.title'>
                <div class="futers__items-item-text">
                    <h3>{{ value.title }}</h3>
                    <p>{{ value.text }}</p>
                </div>
            </div>
        </div>    
    </div>
</template>


<script>
  export default {
    data: function() {
        return {
            data : [
                {
                    img : '/src/assets/icons/to_do_ico.svg',
                    title: 'Список задач',
                    text : 'Все дела в одном месте'
                },
                {
                    img : 'src/assets/icons/priority_ico.svg',
                    title: 'Приоритеты',
                    text : 'Видно, что важно сейчас'
                },
                {
                    img : 'src/assets/icons/reminder_ico.svg',
                    title: 'Напоминания',
                    text : 'Ничего не забывается'
                },
                {
                    img : 'src/assets/icons/history_ico.svg',
                    title: 'Итория',
                    text : 'Контроль выполненной работы'
                }
            ]
        }
    }
  }
</script>


<style>
    .futers {
        display: flex;
        flex-direction: column;
        gap: 24px;
        max-width: 350px;
        max-height: 350px;
        padding: 24px 32px;
        margin: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
    }
    .futers__title h3 {
        font-size: 18px;
        font-weight: 400;
    }
    .futers__items {
        display: flex;
        flex-wrap: wrap;
        gap: 24px;
    }
    .futers__items-item {
        display: flex;
        gap: 16px;
    }
    .futers__items-item img {
        width: 40px;
        height: 40px;
        border-radius: 12px;
        padding: 10px;
        background-color: #3C3C43;

    }
    .futers__items-item-text {
        display: flex;
        flex-direction: column;
        gap: 4px;
    }
    .futers__items-item-text h3 {
        font-size: 14px;
        font-weight: 500;
        color: #181818;
    }
    .futers__items-item-text p {
        font-size: 13px;
        font-weight: 300;
        color: #666666;
    }
</style>