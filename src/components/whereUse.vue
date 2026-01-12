<template>
    <div class="whereUse">
        <h2>Где можно использовать</h2>
        <div class="whereUse__card"
        v-for="(value) in whereUses">
            <div class="whereUse__text">
                <h3>{{ value.title_use }}</h3>
                <section>{{ value.text_use }}</section>
            </div>
            <hr>
            <div class="whereUse__buttons">
                <button 
                v-for="(button) in value.buttons_use"
                :key="button"
                >
                {{ button }}
                </button>
            </div>
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
            whereUses: [
                {
                    title_use: 'Учёба',
                    text_use: 'Помогает не пропускать дедлайны.',
                    buttons_use: [
                        'Домашка', 
                        'Экзамены', 
                        'Проекты', 
                        'Конспекты', 
                        'Курсы'
                    ]
                },
                {
                    title_use: 'Личные дела',
                    text_use: 'Упрощает бытовые и повседневные задачи.',
                    buttons_use: [
                        'Покупки', 
                        'Уборка', 
                        'Финансы', 
                        'Финансы', 
                        'Планы'
                    ]
                }
            ]
        }
    }
    }
</script>


<style>
    .whereUse {
        display: flex;
        flex-direction: column;
        gap: 32px;
        align-items: flex-start;
        margin: 24px;
        padding: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
        max-width: 508px;
        max-height: auto;
    }
    .whereUse h2 {
        font-size: 18px;
        font-weight: 400;
        color: #000000;
    }
    .whereUse__card {
        display: flex;
        flex-direction: column;
        gap: 16px;
    }
    .whereUse__text {
        display: flex;
        flex-direction: column;
        gap: 8px;
    }
    .whereUse__text h3 {
        font-size: 14px;
        font-weight: 400;
        color: #181818;
    }
    .whereUse__text section {
        font-size: 14px;
        font-weight: 300;
        color: #666666;
    }
    .whereUse__card hr {
        height: 2px;
        width: 460px;
        color: #E6E6E6;
    }
    .whereUse__buttons {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
    }
    .whereUse__buttons button {
        padding: 8px;
        border-radius: 100px;
        background-color: #FFFFFF;
        border: 1px solid #3C3C43;
        transition: background-color 0.3s;
    }
    .whereUse__buttons button:hover {
        cursor: pointer;
        background-color: #F5F5F5;
    }
    .whereUse__buttons button:active {
        background-color: #3C3C43;
    }
</style>