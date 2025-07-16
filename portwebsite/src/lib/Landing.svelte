<script>
    export let name;
    export let bio;
    export let cta;
    export let heroIcon;
</script>

<div class="landing-container">
    <div class="hero-text">
        <h1 class="montserrat-intro">I'm {name}.</h1>
        <svg class="svg-box" viewBox="0 0 417 24" fill="none">
            <path class="open-path" d="M1.89008 6.78844C2.85183 6.78844 3.81359 6.78844 21.861 6.78844C39.9084 6.78844 75.0123 6.78844 94.5388 6.30757C131.053 5.40835 161.133 2.91232 173.796 2.17642C176.73 2.00593 179.61 1.45512 205.621 1.2074C231.632 0.959682 280.681 0.959682 306.911 1.20012C333.14 1.44055 335.064 1.92142 350.481 2.16914C394.746 2.88037 421.592 3.37861 414.816 4.83582C406.298 6.66783 393.949 4.36951 365.709 2.91231C344.704 1.82844 310.058 2.41686 290.539 2.89774C258.812 3.67936 240.463 7.25478 221.512 8.72655C207.13 9.84348 196.718 13.579 180.703 14.7958C176.729 15.0977 173.898 16.9597 171.45 18.1838C202.124 21.3604 274.896 21.8413 259.231 22.5699C245.971 22.8177 221.927 22.8177 197.155 22.8177" stroke="#EEC3F3" stroke-width="2" stroke-linecap="round" pathLength="1"/>
        </svg>
            <p class="about">{bio} <br> {cta}</p>
            <a href="mailto:shamanne.sawalha@gmail.com"><button class="contact-btn">Contact Me</button></a>
    </div>
    <img class="hero-icon" src={heroIcon} alt="me when i work">
</div>

<style>
   .landing-container{
    background-color: #1A1A1B;
    display: inline;
    }

    .hero-text{
        display: inline;
        float: left;
        position: absolute;
        z-index: 1;
        margin-left: 9em;
    }

    .hero-icon{
        padding: 2em;
        width: 50%;
        float: right;
    }

    .svg-box{
        margin-top: 0;
        padding-left: 12em;
        padding-bottom: 1em;
    }

    .open-path{
        stroke-dasharray: 1;
        stroke-dashoffset: 1;
        animation: dash 2s linear forwards;
    }

    @keyframes dash{
        to{
            stroke-dashoffset: 0;
        }
    }

    .montserrat-intro {
        font-family: "Montserrat", sans-serif;
        font-optical-sizing: auto;
        font-weight: 764;
        font-style: normal;
        font-size: 6em;
        color: #F2FFFF;
        padding-top: 1em;
        padding-right: 0;
        margin-bottom: 0px;
        margin-right: 0;
        padding-bottom: 0;
        }

    .about {
        font-family: "Karla", sans-serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
        font-size: 1.25em;
        margin-top: 0;
        color: #F2FFFF;
    }

    .contact-btn{
        padding: 0.75em;
        font-family: "Karla", sans-serif;
        font-size: 1em;
        color: #EEC3F3;
        border-radius: 1em;
        background-color: transparent;
        border: 2px solid #EEC3F3;
        transition-duration: 0.4s;
    }

    .contact-btn:hover{
        color: #1A1A1B;
        border-radius: 1em;
        background-color: #EEC3F3;
        border: 2px solid #EEC3F3;
    } 
</style>