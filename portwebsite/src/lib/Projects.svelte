<script>

</script>

<h1>Featured Projects</h1>
<div class="horizontal">
    <div class="rounded-box">
        <h2>Monty Hall Problem Data Scrollytelling</h2>
        <p>A scrollytelling piece with simulated data on my version of the Monty Hall Problem.</p>
        <p><span class="made-w">Made with: </span> React, React-scrollama, D3.js</p>
        <a href="https://monty-hall-problem-eta.vercel.app/"><button class="view-btn">View</button></a>
    </div>
    <div class="rounded-box">
        <h2>How to preprocess data? Part-1</h2>
        <p>A Jupyter notebook on data cleaning and collapsing from a messy Spotify dataset.</p>
        <p><span class="made-w">Made with: </span> Python, pandas, matplotlib</p>
        <a href="https://colab.research.google.com/drive/1iGpNZz_smmAMwYWoHK-4jezw15dBmk_E?usp=sharing"><button class="view-btn">View</button></a>
    </div>
    <div class="rounded-box">
        <h2>How to preprocess data? Part-2</h2>
        <p>A Jupyter notebook on exploratory data analysis and feature engineering as machine learning prep.</p>
        <p><span class="made-w">Made with: </span> Python, pandas, matplotlib</p>
        <a href="https://colab.research.google.com/drive/1AdB9Q6fZQk4_r6B-CyfLy8NeI1CP5_RR?usp=sharing"><button class="view-btn">View</button></a>
    </div>
    <div class="rounded-box">
        <h2>Custom Neural Network for Bank Loan Approval</h2>
        <p>A custom neural network with a novel layer and actovation function compared against a baseline model.</p>
        <p><span class="made-w">Made with: </span> Python, pandas, Pytorch, numpy, sklearn, matplotlib</p>
        <a href="https://colab.research.google.com/drive/19qW16J4r84APBSN1KG99duhZz_gXvVRs?usp=sharing"><button class="view-btn">View</button></a>
    </div>
    <div class="rounded-box">
        <h2>Retail Sales Data Prediction with ARIMA</h2>
        <p>A comparative analysis of ARIMA and XGBoost on predicting sales data.</p>
        <p><span class="made-w">Made with: </span> Python, pandas, numpy, sklearn, matplotlib</p>
        <a href="https://colab.research.google.com/drive/1SKljr89Xl5C-WFl_VPG4HwsqwSXtN-L3"><button class="view-btn">View</button></a>
    </div>
</div>

<style>
    .horizontal{
        padding-top: 2em;
        padding-bottom: 3em;
        width: 100%; /* Or a fixed width */
        overflow-x: scroll;
        overflow-y: hidden;
        white-space: nowrap;
        -webkit-overflow-scrolling: touch;
        &::-webkit-scrollbar {
        display: none;
        }

    }

    .horizontal > div{
        white-space: normal;
    }

    .rounded-box {
        border-radius: 25px; /* Adjust the value for more or less rounding */
        background-color: #2b262a; /* Example background color */
        padding: 20px;
        width: 240px;
        border: 2px solid #EEC3F3;
        color: white;
        max-width: 250px;
        margin-right: 3em;
        display: inline-block; /* Makes items sit in a single row */

    }
    h1{
        font-family: "Montserrat", sans-serif;
        color: white;
    }

    h2{
        margin-top: 0.25em;
        font-family: "Karla", sans-serif;
        font-weight: 800;
    }

    p{
        font-family: "Karla", serif;
    }

    .view-btn{
        padding: 0.75em;
        font-family: "Karla", sans-serif;
        font-size: 1em;
        color: #EEC3F3;
        border-radius: 1em;
        background-color: transparent;
        border: 2px solid #EEC3F3;
        transition-duration: 0.4s;
    }

    .view-btn:hover{
        color: #1A1A1B;
        border-radius: 1em;
        background-color: #EEC3F3;
        border: 2px solid #EEC3F3;
    } 

    .made-w{
        font-family: "Karla", sans-serif;
        font-weight: 700;
    }

</style>