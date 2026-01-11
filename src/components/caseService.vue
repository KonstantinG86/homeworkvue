<template>
    <div class="service">
        <img src="/src/assets/img/to_do.jpg">
        <div class="service__content">
            <div class="service__content-text">
                <h3>Сервис для повседневных дел</h3>
                <span>Простая организация времени</span>
            </div>
            <p class="service__content-text-p">Подходит для учебы, работы и личных проектов.</p>
            <hr>
            <div class="service__content-categories">
                <h3>Категории</h3>
                <div class="service__content-categories-buttons">
                    <button>Учеба</button>
                    <button>Работа</button>
                    <button>Дом</button>
                    <button>Здоровье</button>
                </div>
            </div>
            <button class="service__content-create-button">Создать список</button>
        </div>
    </div>
</template>


<script>

</script>


<style>
    .service {
        display: flex;
        flex-direction: column;
        margin: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
        max-width: 342px;
        max-height: auto;
        overflow: hidden;
    }
    .service__content {
        display: flex;
        flex-direction: column;
        padding: 24px;
        gap: 16px;
    }
    .service__content-text {
        display: flex;
        flex-direction: column;
        gap: 4px;
    }
    .service__content-text h3 {
        font-size: 18px;
        font-weight: 400;
    }
    .service__content-text span {
        font-size: 14px;
        font-weight: 300;
        color: #181818;
    }
    .service__content-text-p {
        font-size: 14px;
        font-weight: 300;
        color: #666666;
    }
    hr {
        height: 1px;
        color: #C4C4C4;
    }
    .service__content-categories {
        display: flex;
        flex-direction: column;
        gap: 8px;
    }
    .service__content-categories h3 {
        font-size: 14px;
        font-weight: 300;
    }
    .service__content-categories-buttons {
        display: flex;
        flex-wrap: wrap;
        gap: 8px;
    }
    .service__content-categories-buttons button {
        padding: 8px;
        border-radius: 100px;
        background-color: #FFFFFF;
        border: 1px solid #3C3C43;
        transition: background-color 0.3s;
    }
    .service__content-categories-buttons button:hover {
        cursor: pointer;
        background-color: #F5F5F5;
    }
    .service__content-categories-buttons button:active {
        background-color: #3C3C43;
    }
    .service__content-create-button {
        background-color: #3C3C43;
        border-radius: 12px;
        border: none;
        width: 134px;
        font-size: 12px;
        font-weight: 300;
        padding: 8px 18px;
        color: #FFFFFF;
        transition: background-color 0.3s;
    }
    .service__content-create-button:hover {
        cursor: pointer;
        background-color: #6a6a70;
    }
    .service__content-create-button:active {
        background-color: #bdbdc9;
    }
</style>