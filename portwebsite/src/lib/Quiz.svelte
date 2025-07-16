<script lang>
    let answers = []
function handleOnSubmit (){
    const correctAnswers = ['1', '2', '3']
    checkAnswers(correctAnswers, answers);
}

function checkAnswers(correctAnswers, answers){
    console.log(correctAnswers);
    console.log(answers);
    if (answers.length === correctAnswers.length && answers.every(val => correctAnswers.includes(val))){
        alert("You got them right!!!");
    }
    else{
        alert("Try again!;D")
    }
}

</script>

<form class="fun-facts" id="fun-facts" name="facts" on:submit|preventDefault={handleOnSubmit}>
    <h2 class="quiz-header">Fun Facts</h2>
    Which of these statements do you think are right about me? <br>Pick three.<br>
    <input class="qitems" type="checkbox" name="facts" bind:group={answers} value="1">I can read a 300-page book in one sitting.<br>
    <input class="qitems" type="checkbox" name="facts" bind:group={answers} value="2">I have 10 ear piercings (used to be 11).<br>
    <input class="qitems" type="checkbox" name="facts" bind:group={answers} value="3">I have a dog named Dollar.<br>
    <input class="qitems" type="checkbox" name="facts" bind:group={answers} value="4">I used to have a Leopard Gecko named Pax.<br>
    <input class="check-btn" type="submit" value="Check">
</form>

<style>
    .fun-facts{
    font-family: "Karla", serif;
    border-radius: 10px;
    background-color: #EEC3F3;
    padding: 1.5em;
    margin-bottom: 3em;
    font-size: 1.5em;
    }

    .quiz-header{
        text-align: center;
        font-family: "Montserrat", sans-serif;
        color: #1A1A1B;
        font-optical-sizing: auto;
        margin: 0.25em;
        padding: 0.25em;
    }

    input[type=submit]{
    padding: 0.5em;
    font-family: "Karla", sans-serif;
    font-size: 0.65em;
    color: #1A1A1B;
    border-radius: 1em;
    background-color: transparent;
    border: 2px solid #1A1A1B;
    transition-duration: 0.4s;
    margin-top: 1em;
    margin-left: 16em;
    }

    input[type=submit]:hover{
        color: #EEC3F3;
        border-radius: 1em;
        background-color: #1A1A1B;
        border: 2px solid #EEC3F3;
    }

    :root {
    --checkbox-border-color: #1A1A1B;
    --checkbox-checked-color: #1A1A1B;
    }

    input[type="checkbox"] {
    box-sizing: border-box;
    width: 15px;
    height: 15px;
    margin-top: 20px;
    padding: 0;
    border: 2px solid var(--checkbox-border-color);
    appearance: none;
    background-color: transparent;
    outline: none;
    transition: outline 0.1s;
    }

    input[type="checkbox"]:checked {
    background-size: cover;
    padding: 2px;
    background-image: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="20" height="20" viewBox="0 0 32 32" xml:space="preserve"><path style="fill: %23EEC3F3" d="M11.941,28.877l-11.941-11.942l5.695-5.696l6.246,6.246l14.364-14.364L32,8.818"/></svg>');
    background-color: #1A1A1B;
    }
</style>