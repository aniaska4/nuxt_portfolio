<template lang="pug">
    section.projects.scroll_section
        .container
            .projects_name
                h1 my projects
            .projects_pic_all
                .projects_pic(v-for="project in projects")
                    div(:class="project.class")
                        a(:href="project.href" target="blank")
                            img(:src="project.img")
                    .card.text-white.bg-secondary
                        .card-body
                            h5.card-title {{project.name}}
                            p.card-text {{project.describe}}
                        .card-footer
                            small(class="text-light") {{project.details}}
</template>
<script>
export default {
    data(){
        return{
            projects: [
                {
                    class: "lilando",
                    href: "https://github.com/aniaska4/Lilando",
                    img: "images/lilando.png",
                    name: "Lilando",
                    describe: "A small responsive website of a cosmetics company Lilando.",
                    details: "Webside made in HTML, CSS and JavaScript."
                },
                  {
                    class: "furryGame",
                    href: "https://github.com/aniaska4/Furry_Games",
                    img: "images/furryGame.png",
                    name: "Furry game",
                    describe: "Short game made in HTML and JavaScript.",
                    details: "Game was prepared in CodersLab course."
                },
                  {
                    class: "recipes",
                    href: "https://github.com/aniaska4/Recipe-dataset",
                    img: "images/recipes.png",
                    name: "Qlinarny Świat",
                    describe: "A small responsive website of page with culinary recipes.",
                    details: "Project made in React.js and firebase. Still in progress."
                },
                  {
                    class: "sitOnChair",
                    href: "https://aniaska4.github.io/Sit-On-Our-Chair/",
                    img: "images/sitOnChair.png",
                    name: "Sit on chair",
                    describe: "A PSD mockup converted into HTML, CSS and JavaScript website. No RWD.",
                    details: "Webside made in HTML, CSS and JavaScript."
                },
                  {
                    class: "toDo",
                    href: "https://github.com/aniaska4/ToDo_List_React",
                    img: "images/toDo.png",
                    name: "To-Do-List",
                    describe: "React to-do list app allowing to add and delete notes from the list.",
                    details: "App made in React.js."
                },
                  {
                    class: "sitOnChair",
                    href: "",
                    img: "image/workInProgress.jpg",
                    name: "Work in progress",
                    describe: "",
                    details: ""
                }
            ]
        }
    }
    
}
</script>
<style scoped>
.projects { height: 100%; margin-bottom: 20px; }

.projects .projects_name { height: 20vh; padding-top: 20px; margin-left: 10px; width: 400px; }

.projects .projects_name h1 { width: 100%; text-transform: uppercase; border-bottom: 3px solid white; color: rgba(59, 58, 58, 0.842); font-size: 30px; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .projects .projects_name h1 { font-size: 35px; width: 70%; } }

@media (min-width: 768px) and (max-width: 991px) { .projects .projects_name h1 { width: 60%; } }

.projects .projects_name h1:hover { border-bottom: 3px solid red; transition: border-bottom 0.3s ease; }

.projects .projects_pic_all { display: flex; flex-wrap: wrap; justify-content: space-around; width: 90%; }

.projects .projects_pic_all .projects_pic { width: 400px; height: 400px; border: 5px solid black; margin: 10px; box-shadow: none; }

.projects .projects_pic_all .projects_pic .card { display: flex; flex-direction: column; min-width: 0; word-wrap: break-word; background-clip: border-box; border: 1px solid rgba(0, 0, 0, 0.125); height: 35%; font-family: 'Open Sans', Arial, Helvetica, sans-serif; }

.projects .projects_pic_all .projects_pic .card .card-body { flex: 1 1 auto; display: flex; flex-direction: column; }

.projects .projects_pic_all .projects_pic .card .card-body .card-title { font-weight: 600; text-shadow: 2px 3px 0 black; line-height: 1.2; color: inherit; text-align: left; font-size: 20px; height: 50%; margin: 10px 10px 5px 15px; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .projects .projects_pic_all .projects_pic .card .card-body .card-title { font-weight: 500; font-size: 1em; text-shadow: 1px 1px 0 black; border-bottom: 2px solid black; } }

.projects .projects_pic_all .projects_pic .card .card-body .card-text { visibility: visible; transition: opacity 0.6s cubic-bezier(0.5, 0, 0, 1) 0s; text-align: left; height: 50%; font-size: 15px; margin: 10px 10px 5px 15px; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .projects .projects_pic_all .projects_pic .card .card-body .card-text { font-weight: 500; font-size: 0.8em; } }

.projects .projects_pic_all .projects_pic .card .card-footer { background-color: rgba(0, 0, 0, 0.3); border-top: 1px solid rgba(0, 0, 0, 0.125); display: flex; flex-direction: column; }

.projects .projects_pic_all .projects_pic .card .card-footer .text-light { font-size: 80%; color: #f8f9fa; text-align: left; margin: 10px 10px 10px 15px; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .projects .projects_pic_all .projects_pic .card .card-footer .text-light { font-weight: 400; font-size: 0.8em; } }

.projects .projects_pic_all .projects_pic .text-white { color: white; }

.projects .projects_pic_all .projects_pic .bg-secondary { background-color: gray; }

.projects .projects_pic_all .lilando, .projects .projects_pic_all .furryGame, .projects .projects_pic_all .recipes, .projects .projects_pic_all .toDo, .projects .projects_pic_all .sitOnChair { background-position: center; background-size: cover; background-repeat: no-repeat; height: 65%; }

.projects .projects_pic_all .lilando a, .projects .projects_pic_all .furryGame a, .projects .projects_pic_all .recipes a, .projects .projects_pic_all .toDo a, .projects .projects_pic_all .sitOnChair a { width: 100%; height: 100%; }

.projects .projects_pic_all .lilando a img, .projects .projects_pic_all .furryGame a img, .projects .projects_pic_all .recipes a img, .projects .projects_pic_all .toDo a img, .projects .projects_pic_all .sitOnChair a img { width: 100%; height: 100%; }


</style>