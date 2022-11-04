<template>
    <header>
        <i class="fa-solid fa-bars"></i>
        <h1>{{ title }}</h1>
        <form>
            <input type="text" name="searcher" id="searcher" placeholder="Type a City">
            <button type="submit"><i class="fa-solid fa-magnifying-glass"></i></button>
        </form>
    </header>
</template>

<script>
export default {
  name: 'HeaderOne',
  props: {
    title: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700&display=swap');

header {
    background-image: url("../assets/sky_day.png");
    background-repeat: no-repeat;
    background-size: cover;
    padding: 2%;
    display: flex;
    flex-flow: row wrap;
    justify-content: flex-start;
    align-items: center;
}
i {
  flex: 1;
  order: 1;
  font-size: 2vw;
  visibility: visible;
}
h1 {
  flex: 6.5;
  order: 2;
  font-size: 3vw;
  font-family: 'Nanum Gothic';
}
form {
    flex: 1.2;
    order: 3;
    align-self: center;
    display: flex;
    flex-flow: row wrap;
    justify-content: center;
    align-items:stretch;
    background-color: #fff;
    padding: 0.5%;
    border-radius: 20px;
}
form input {
    flex: 1;
    border-radius: 20px;
    padding: 0.1%;
    border:none;
    font-family: 'Nanum Gothic';
    font-size: 1vw;
    color: #3687cd;
}
form input::placeholder {
    text-align:center; 
    font-family: 'Nanum Gothic';
    font-size: 1vw;
    color: #3687cd;
}
form input:focus {
    border:none;
}
form button {
    margin-left: 2%;
    background: none;
    border:none;    
}
form button i {
    color: #000;
    font-size: 1.5vw;
}
</style>