<script>
    export let BANNER_DATA;
    let { HEADING, DESCRIPTION, TUTORIAL_URL, WATCH_TUTORIAL } = BANNER_DATA;
</script>

<section class="main-bgcolor light-color" id="banner">
    <div class="container">
        <div class="row">
            <div class="col-md-6">
                <h1>{HEADING}</h1>
                <p>{DESCRIPTION}</p>
                <!-- svelte-ignore security-anchor-rel-noreferrer -->
                <a href={TUTORIAL_URL} target="_blank" class="light-color">
                    <i class="far fa-play-circle fa-2x watch-btn" />
                    {WATCH_TUTORIAL}
                </a>
            </div>
            <div class="col-md-6">
                <img src="images/home.png" alt="" class="img-fluid" />
            </div>
        </div>
    </div>
    <img src="images/wave1.png" alt="" class="wave-img" />
</section>

<style>
    section {
        padding-top: 5%;
    }

    h1 {
        font-size: 40px;
        font-weight: 600;
        margin-top: 100px;
        text-transform: uppercase;
    }
    .watch-btn {
        margin: auto 20px;
        position: relative;
        top: 8px;
    }

    section a {
        text-decoration: none;
    }

    .wave-img {
        width: 100%;
        height: auto;
    }
</style>
