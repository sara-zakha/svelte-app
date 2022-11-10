<script>
    import About from "./components/About.svelte";
    import Banner from "./components/Banner.svelte";
    import Footer from "./components/Footer.svelte";
    import NavBar from "./components/NavBar.svelte";
    import Service from "./components/Service.svelte";
    import SocialMedia from "./components/SocialMedia.svelte";
    import Testimornial from "./components/Testimornial.svelte";
    import data from "./data/data";

    let HEADER = data.HEADER;
    let NAVBAR_DATA = data.NAVBAR_DATA;
    let BANNER_DATA = data.BANNER_DATA;
    let SERVICE_DATA = data.SERVICE_DATA;
    let ABOUT_DATA = data.ABOUT_DATA;
    let TESTIMONIAL_DATA = data.TESTIMONIAL_DATA;
    let SOCIAL_DATA = data.SOCIAL_DATA;
    let FOOTER_DATA = data.FOOTER_DATA;
</script>

<main>
    <NavBar {HEADER} {NAVBAR_DATA} />
    <Banner {BANNER_DATA} />
    <Service {SERVICE_DATA} />
    <About {ABOUT_DATA} />
    <Testimornial {TESTIMONIAL_DATA} />
    <SocialMedia {SOCIAL_DATA} />
    <Footer {HEADER}  {FOOTER_DATA} />
</main>

<style>
</style>
