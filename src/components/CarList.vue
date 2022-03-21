<template>
    <div id="wrapper">
        <div class="cars">
            <div class="car" v-for="car in cars" :key="car.id">
                <div class="info">
                    <h1>{{car.car_make}} {{car.car_model}}</h1>
                    <p>{{car.car_model_year}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .wrapper {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .cars {
        margin-top: 20px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
    }

    .car {
        margin: 10px;
        margin-top: 50px;
        width: 160px;
    }

    .info {
        background: FireBrick;
        color: #000;
        padding: 50px 30px;
        height: 80px;
    }

    .info h1 {
        font-size: 16px;
    }

    .info p {
        margin: 0px;
        font-size: 10px;
    }

    .auto {
        margin-left: auto;
    }
</style>

<script>
    export default {
        name: 'CarList',
        props: {
            cars: Array
        }
    }
</script>