<template>
    <footer>
        <p>{{ author }} &copy; , 2022</p>
        <article>
            <i class="fa-brands fa-github"></i>
            <i class="fa-brands fa-linkedin"></i>
        </article>
    </footer>
</template>

<script>
export default {
  name: 'FooterOne',
  props: {
    author: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700&display=swap');

footer {
    background-image: url("../assets/ground.png");
    background-repeat: no-repeat;
    background-size: cover;
    padding: 2%;
    display: flex;
    flex-flow: row wrap;
    justify-content: space-between;
    align-items: center;
}
footer p{
    font-family: 'Nanum Gothic';
    color: #efeecc;
    font-size: 1vw;
}

footer article {
    display:flex; 
    flex-flow: row wrap;
    justify-content: space-around;
    align-items: center;
}
footer article i{
    flex: 2;
    margin: 0 1vw;
    font-size: 1.5vw;
    color: #efeecc;
    text-shadow: 0px 0px 10px #dad4a2;
    cursor: pointer;
    transition: .5s all ease-in;
}
footer article i:first-of-type:hover{
    color: #000;
}

footer article i:last-of-type:hover{
    color: #0077b5;
}

</style>