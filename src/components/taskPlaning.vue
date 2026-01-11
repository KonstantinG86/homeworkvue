<template>
    <div class="task">
        <div class="task__text">
            <h3>
                Умное планирование задач
            </h3>
            <p>
                Держите фокус на главном и не теряйте сроки.
            </p>
        </div>
        <div class="task__button">
            <button>Начать работу</button>
        </div>
    </div>
</template>


<script>
  
</script>


<style>
    .task {
        display: flex;
        gap: 24px;
        align-items: center;
        flex-direction: column;
        max-width: 268px;
        max-height: 198px;
        padding: 24px;
        margin: 24px;
        border-radius: 12px;
        background-color: #FFFFFF;
    }
    .task__text {
        text-align: start;
        gap: 12px;
        display: flex;
        flex-direction: column;
    }
    .task__text h3 {
        font-size: 18px;
        font-weight: 400;
    }
    .task__text p {
        font-size: 14px;
        font-weight: 300;
        color: #666666;
    }
    .task__button {
        display: flex;
        width: 100%;
        justify-content: right;
    }
    .task__button button {
        background-color: #3C3C43;
        border-radius: 12px;
        border: none;
        padding: 8px 18px;
        color: #FFFFFF;
        transition: background-color 0.3s;
    }
    .task__button button:hover {
        cursor: pointer;
        background-color: #6a6a70;
    }
    .task__button button:active {
        background-color: #bdbdc9;
    }
</style>