
<script>
    import Landing from "./lib/Landing.svelte";
    import Nav from "./lib/Nav.svelte";
    import Links from "./lib/Links.svelte";
    import Card from "./lib/Card.svelte";
    import Quiz from "./lib/Quiz.svelte";
    import Teaser from "./lib/assets/Teaser (Autodesk & Ai).jpg";
    

    let name = "Shamika";
    let bio = "And I like to create with 💗, both software and artworks alike.";
    let cta = "Checkout my stuff. Let's work together.";
    let heroIcon = "/v2.png"

    let cardData = [
        {
            portImage: "/IMG_4038.PNG",
            title: '"Matilda"',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/178dmJJNy6o6zSwnzSb6FlX1ENb7n1DDk/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/art-piece1.PNG",
            title: '"Lucky Star Cafe Figurine"',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1pprhK8vDJWF_kB7c5LmfuUH4Lt0kTZHB/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/Screenshot 2024-07-09 162455.png",
            title: '"Nasaan na si Bruno?" Storybook',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1mlMsRdWA5DsjdeIm7qkVoFfpVuHX9gPs/view?usp=drive_link"
        },
        {
            portImage: {Teaser},
            title: 'Podcast Teaser',
            subtitle: "illustrator / layout artist",
            outLink: "https://drive.google.com/file/d/1R_HDnDcIs7H_fjqpav2O5FvtJOj6bSR_/view?usp=drive_link"
        },
         {
            portImage: "src/lib/assets/poster (1).jpg",
            title: 'Event Poster',
            subtitle: "illustrator / layout artist",
            outLink: "https://drive.google.com/file/d/1loxH7xUNGWA2igI3Y1RN0itDCp_RXn9p/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/Website Background (Procreate).PNG",
            title: 'Website Background',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1aNFUbgEpQOWpKu8uvN6jSxJIb_ssfTdZ/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/449641748_1174403883704236_4451601075784323482_n.jpg",
            title: '"Faura Hall"',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1dq0a430gN_zkMLGP6lMy9gXKxg5wRKgB/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/449493571_1191743911847098_3736706079504177442_n.jpg",
            title: '"Olive"',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1d9Ee__tEDDf9DIoVWZ_PXear0hNqHF-8/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/Podcast Cover (Procreate) (1).PNG",
            title: 'Podcast Cover',
            subtitle: "illustrator",
            outLink: "https://drive.google.com/file/d/1Z43hyr8wguwZb67pSj_yOSqpSPs9wF1j/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/302773533_585031313315254_4283950001366953607_n.jpg",
            title: 'ASHS ProgVar PubMat 1',
            subtitle: "illustrator / layout artist",
            outLink: "https://drive.google.com/drive/folders/1NP9v71_5CjtEWRCx9A19w8eRtfDH3cqN?usp=sharing"
        },
        {
            portImage: "src/lib/assets/Sign ups pub 5-01.png",
            title: 'ASHS ProgVar PubMat 2',
            subtitle: "illustrator / layout artist",
            outLink: "https://drive.google.com/file/d/1go4n1vVlgVu3UbHoh2Iw721EgBPdmjZf/view?usp=drive_link"
        },
        {
            portImage: "src/lib/assets/pvg.png",
            title: 'ASHS ProgVar Animatic',
            subtitle: "illustrator / animator",
            outLink: "https://drive.google.com/file/d/1-TmkBH2_Iuq3BbvoC216iGL32LLata3z/view?usp=drive_link"
        },
    ]
</script>


<div class="flex-container">
    <Nav />
    <Landing {name} {bio} {cta} {heroIcon} />
</div>
<div>
    <Links />
</div>
<h1 class="work-header" id="work-header">Some Works</h1>
<section id="works" class="works">
    {#each cardData as { portImage, title, subtitle, outLink }}
      <Card {portImage} {title} {subtitle} {outLink} />
    {/each}
</section>
<div class="quiz">
    <Quiz />
</div>

<style>
    .work-header{
    text-align: center;
    font-family: "Montserrat", sans-serif;
    color: #F2FFFF;
    font-optical-sizing: auto;
    font-weight: 700;
    font-style: normal;
    margin-top: 40px;
    margin-bottom: 40px;
    }
    .works{
    display: grid;
    grid-template-columns: repeat(3, 33.33333%);
    margin-left: 75px;
    margin-right: 75px;
    background-color: #1A1A1B;
    }
    .quiz{
    display:flex;
    flex-direction: column;
    align-items: center;
    }
</style>
