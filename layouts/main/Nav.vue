<template lang="pug">
    header
        .nav
            nav.main_nav
                .container                    
                    ul
                        li.scroll(v-for="nav in navigation") {{nav}}
            //- nav(role="navigation" class="navigation")
            //-     #menuToggle
            //-         input(type="checkbox")
            //-         span
            //-         ul#menu
            //-             li(v-for="nav in navigation")
            //-                 a.scroll_dropdown( href="#") {{nav}}
        
</template>
<<script>
export default {
    name: "Nav",
    data(){
        return {
            navigation: [
                "about me", "my skills", "my projects", "contact me"
            ]
        }
    }
}
</script>
<style scoped>
header {
    height: 80px;
}
.scroll_show { opacity: 1; transition: opacity 2s ease; }

.title { opacity: 0; }

.nav .main_nav { position: fixed; background-color: rgba(223, 215, 215, 0.774); width: 100%; }

.nav .main_nav ul { list-style-type: none; display: flex; justify-content: left; color: rgba(59, 58, 58, 0.842); font-weight: 600; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .nav .main_nav ul { display: none; } }

.nav .main_nav ul li { margin: 10px; text-transform: uppercase; border-bottom: 2px solid rgba(234, 224, 224, 0.774); transition: border-bottom 0.3s linear; cursor: pointer; }

.nav .main_nav ul li:hover { border-bottom: 2px solid red; }

.nav #menuToggle { display: none; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .nav #menuToggle { display: block; position: relative; top: 50px; left: 50px; z-index: 1; -webkit-user-select: none; user-select: none; }
  .nav #menuToggle input { display: block; width: 40px; height: 32px; position: absolute; top: -7px; left: -5px; cursor: pointer; opacity: 0; z-index: 2; -webkit-touch-callout: none; }
  .nav #menuToggle span { display: block; width: 33px; height: 4px; margin-bottom: 5px; position: relative; background: #cdcdcd; border-radius: 3px; z-index: 1; transform-origin: 4px 0px; transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), background 0.5s cubic-bezier(0.77, 0.2, 0.05, 1), opacity 0.55s ease; } }

.nav #menuToggle #menuToggle span:first-child { transform-origin: 0% 0%; }

.nav #menuToggle span:nth-last-child(2) { transform-origin: 0% 100%; }

.nav #menuToggle input:checked ~ span { opacity: 1; transform: rotate(45deg) translate(-2px, -1px); background: #232323; }

.nav #menuToggle input:checked ~ span:nth-last-child(3) { opacity: 0; transform: rotate(0deg) scale(0.2, 0.2); }

.nav #menuToggle input:checked ~ span:nth-last-child(2) { transform: rotate(-45deg) translate(0, -1px); }

.nav #menu { position: absolute; width: 35vw; margin: -100px 0 0 -50px; padding-left: 50px; padding-top: 100px; padding-bottom: 20px; background-color: rgba(5, 5, 5, 0.26); list-style-type: none; -webkit-font-smoothing: antialiased; transform-origin: 0% 0%; transform: translate(-100%, 0); transition: transform 0.5s cubic-bezier(0.77, 0.2, 0.05, 1); }

.nav #menu li { padding: 10px 0; font-size: 22px; }

.nav #menuToggle input:checked ~ ul { transform: none; }

.nav .name { display: flex; flex-direction: column; justify-content: center; align-items: center; height: 100vh; }

.nav .name h2 { font-size: 5em; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .nav .name h2 { font-size: 2em; } }

.nav .name h3 { font-size: 2em; color: red; }

@media (min-width: 321px) and (max-width: 576px), (max-width: 320px) { .nav .name h3 { font-size: 2em; } }

.nav a { text-decoration: none; color: #232323; transition: color 0.3s ease; }

.nav a:hover { color: tomato; }
</style>
