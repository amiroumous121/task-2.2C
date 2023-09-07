<template>
  <div id="app">
    <header>
      <h1>Weather Dashboard</h1>
    </header>
    <main>
      <section class="weather-info">
        <h2>Current Weather in [Location]</h2>
        <p>Temperature: {{ temperature }}°C</p>
        <p>Humidity: {{ humidity }}%</p>
        <p>Wind Speed: {{ windSpeed }} km/h</p>
      </section>
    </main>
    <footer>
      <p></p>
    </footer>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      temperature: 25,
      humidity: 60,
      windSpeed: 10,
    };
  },
};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

header,
footer {
  background-color: #4caf50;
  color: white;
  text-align: center;
  padding: 1em;
}

.weather-info {
  padding: 2em;
  text-align: center;
}
</style>
