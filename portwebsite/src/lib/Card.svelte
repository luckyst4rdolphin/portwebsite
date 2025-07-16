<script>
    export let portImage;
    export let title;
    export let subtitle;
    export let outLink;
</script>

<a class="zoom-img" target="_top" href={outLink}>
            <div class="overlay">
                <p class="cap">{title}</p>
                <p class="sub">{subtitle}</p>
            </div>
            <img class="portfolio-img" src={portImage} alt="">
</a>

<style>
    .portfolio-img{
    clip-path: polygon(0 0, 100% 0, 100% 80%, 0 80%);
    height: 420px;
    width: 400px;
    object-fit: cover;
    margin: 0 auto;
    }

    .zoom-img {
        object-fit: cover;
        height: 420px;
        width: 400px;
        margin: 0 auto;
    }

    .overlay {
        position: absolute;
        background: linear-gradient(to bottom, rgba(255,0,0,0), #EEC3F3);
        height: 336px;
        width: 400px;
        transition: all .5s ease;
        opacity: 0;
        z-index: 5;
    }

    .overlay:hover {
        opacity: 1;
    }

    .cap {
        font-family: "Karla", sans-serif;
        font-optical-sizing: auto;
        font-weight: 700;
        font-style: normal;
        font-size: 20px;
        text-align: center;
        color: #1A1A1B;
        margin-top: 250px;
    }

    .sub {
        font-family: "Karla", serif;
        font-style: italic;
        text-align: center;
        color: #1A1A1B;
        margin-top: -15px;
    }
</style>