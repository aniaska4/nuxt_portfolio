<template lang="pug">
    section.skills
        .container
            .skills_name
                h1.title Skills
            section.skills_toUse
                .skills_about_toUse
                    h1 Technology I am using:
                .skills_pictures
                    .skills_picture(v-for="icon in icons")
                        i(:class="icon")
</template>
<script>
export default {
    name: "Skills",
    data(){
        return {
            icons: [
                "fab fa-html5 icon",
                "fab fa-js icon",
                "fab fa-css3-alt icon",
                "fab fa-gulp icon",
                "fab fa-github icon",
                "fab fa-npm icon",
                "fab fa-sass icon",
                "fab fa-vuejs icon",
                "icon"
            ],
        }
    }
}
</script>
<style scoped>

.skills { background-color: #aafcfc; height: 100%; min-height: 800px; }

.skills .skills_name { height: 20vh; padding-top: 20px; margin-left: 10px; width: 200px; }

.skills .skills_name h1 { width: 100%; text-transform: uppercase; border-bottom: 3px solid #aafcfc; color: rgba(59, 58, 58, 0.842); font-size: 30px; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .skills .skills_name h1 { font-size: 35px; } }

.skills .skills_name h1:hover { border-bottom: 3px solid red; transition: border-bottom 0.3s ease; }

.skills .skills_toUse { display: flex; flex-direction: column; align-items: center; }

.skills .skills_toUse .skills_about_toUse { height: 25vh; }

.skills .skills_toUse .skills_about_toUse h1 { text-align: center; font-size: 25px; color: rgba(59, 58, 58, 0.842); }

.skills .skills_toUse .skills_pictures { display: flex; flex-wrap: wrap; justify-content: space-around; width: 100%; }

.skills .skills_toUse .skills_pictures .skills_picture { height: 200px; width: 400px; text-align: center; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .skills .skills_toUse .skills_pictures .skills_picture { height: 200px; width: 200px; } }

.skills .skills_toUse .skills_pictures .skills_picture .icon { font-size: 5em; transition: transform 0.5s; }

.skills .skills_toTeach { display: flex; flex-direction: column; align-items: center; padding-top: 30px; }

.skills .skills_toTeach .skills_about_toTeach { height: 20vh; }

.skills .skills_toTeach .skills_about_toTeach h1 { text-align: center; font-size: 25px; color: rgba(59, 58, 58, 0.842); }

.skills .skills_toTeach .skills_pictures { display: flex; flex-wrap: wrap; justify-content: space-around; width: 100%; }

.skills .skills_toTeach .skills_pictures .skills_picture { height: 200px; width: 400px; text-align: center; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .skills .skills_toTeach .skills_pictures .skills_picture { height: 200px; width: 200px; } }

.skills .skills_toTeach .skills_pictures .skills_picture .icon { font-size: 5em; transition: transform 0.5s; }

</style>
