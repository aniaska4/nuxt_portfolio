<template lang="pug">
    .name
        .container
            .main_title
                h2.title Anna Belka
            .small_title
                h3
                    span.front_name front 
                    span.end_name end 
                    span.front_name developer
</template>
<script>
export default {
    name: "Title"
}
</script>
<style scoped>
.name{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.name h2{
    /* opacity: 1;
    transition: opacity 2s ease 0s; */
    font-size: 5em;
}
.front_name{
font-size: 2em;
    color: red;
}
.end_name{
font-size: 2em;
    color: black;
}
.main_title{
    margin-bottom: 30px;
}
.small_title, .main_title{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center
}

</style>

