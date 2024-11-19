<template>
    <div>

    </div>
</template>

<script setup>
import axios from 'axios';
import { useRoute } from 'vue-router';

const route = useRoute();

const getWeatherData = async() => {
    try {
        const weatherData = await axios.get(
        `https://api.openweathermap.org/data/2.5/onecall?lat=${route.query.lat}&lon=${route.query.lng}&exclude={part}&appid=ffb4dfa520bea4a7eb096da1e21ceea0&units=imperial`
        );
    } catch(err) {

    }
};
</script>