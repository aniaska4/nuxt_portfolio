<template lang="pug">
    section.about
        .container
            .about.scroll_section
                .about_title
                    h1.title about me
            .about_all_sectiones
                section.about_section_one
                    .about_picture
                article.about_section_two
                    .about_describe
                        h2 Hello Stranger! My name is Ania. I'm a passionate programmer.
                        p I am beginner Front-End Developer, seeking work in developing in an interesting company.
                            |I am strongly motivated and interested in challenges offered by the area of programming.
                            |I am a postgraduate of the Faculty of Management at the Warsaw University .
                            |I worked for several years at the governmental institutions where I was responsible for the
                            |implementation of EU projects.
                            |For the last three years I have been a happy mother of two children. During my free time
                            |I am improving my skills in the front-development.
                            |Over time I will post here my projects.
</template>
<script>
export default {
    
}
</script>
<style scoped>
.about { height: 100%; }

.about .about_title { height: 5vh; margin-bottom: 30px; width: 200px; }

.about .about_title h1 { width: 100%; text-transform: uppercase; border-bottom: 3px solid white; color: rgba(59, 58, 58, 0.842); font-size: 30px; opacity: 0; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_title h1 { font-size: 35px; width: 100%; } }

@media (min-width: 768px) and (max-width: 991px) { .about .about_title h1 { width: 80%; } }

.about .about_title h1:hover { border-bottom: 3px solid red; transition: border-bottom 0.3s ease; }

.about .about_all_sectiones { display: flex; flex-direction: row; }

@media (min-width: 768px) and (max-width: 991px), (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones { display: flex; flex-direction: column; align-items: center; } }

.about .about_all_sectiones .about_section_one { width: 50%; height: 80vh; margin-left: 20px; }

@media (min-width: 768px) and (max-width: 991px) { .about .about_all_sectiones .about_section_one { display: flex; flex-direction: column; align-items: center; width: 100%; } }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones .about_section_one { display: flex; flex-direction: column; align-items: center; width: 90%; } }

.about .about_all_sectiones .about_section_one .about_picture { background-image: url("/images/me.jpg"); background-position: center; background-size: cover; background-repeat: no-repeat; height: 65%; width: 100%; height: 70vh; }

.about .about_all_sectiones .about_section_one .about_picture a { width: 100%; height: 100%; }

.about .about_all_sectiones .about_section_one .about_picture a img { width: 100%; height: 100%; }

@media (min-width: 992px) and (max-width: 1201px) { .about .about_all_sectiones .about_section_one .about_picture { width: 90%; height: 60vh; } }

@media (min-width: 768px) and (max-width: 991px) { .about .about_all_sectiones .about_section_one .about_picture { width: 60%; height: 70vh; } }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones .about_section_one .about_picture { width: 80%; height: 70vh; } }

.about .about_all_sectiones .about_section_two { color: rgba(59, 58, 58, 0.842); margin-right: 20px; width: 50%; }

@media (min-width: 1202px) and (max-width: 1599px) { .about .about_all_sectiones .about_section_two { width: 50%; } }

@media (min-width: 992px) and (max-width: 1201px) { .about .about_all_sectiones .about_section_two { width: 50%; display: flex; flex-direction: column; align-items: center; } }

@media (min-width: 768px) and (max-width: 991px), (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones .about_section_two { width: 80%; display: flex; flex-direction: column; align-items: center; } }

.about .about_all_sectiones .about_section_two .about_describe { display: flex; flex-direction: column; align-items: center; width: 100%; margin-left: 20px; }

.about .about_all_sectiones .about_section_two .about_describe h1 { text-align: left; font-size: 40px; padding-bottom: 20px; }

@media (min-width: 992px) and (max-width: 1201px) { .about .about_all_sectiones .about_section_two .about_describe h1 { font-size: 30px; } }

@media (min-width: 768px) and (max-width: 991px), (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones .about_section_two .about_describe h1 { font-size: 30px; padding-left: 20px; width: 100%; } }

.about .about_all_sectiones .about_section_two .about_describe h1:after { display: block; content: ""; width: 150px; height: 40px; border-bottom: 3px solid red; }

.about .about_all_sectiones .about_section_two .about_describe p { text-align: left; line-height: 1.8; letter-spacing: 1.2px; }

@media (min-width: 577px) and (max-width: 767px), (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .about .about_all_sectiones .about_section_two .about_describe p { padding-left: 10px; } }

</style>
