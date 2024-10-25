<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bear Ninja Hunter Game</title>
    <style>
    
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        .result {
            margin-top: 20px;
            font-size: 1.5em;
        }
    </style>
</head>
<body>
    <h1>Bear Ninja Hunter Game</h1>
    
  <div>
    <script src="text/javascript">
          <input type="text" id="playerChoice" placeholder="Enter Bear, Ninja, or Hunter">
          <button onclick="playGame">Play</button>
          class="result" id="result">
          let playerName ='enter name';

     function playGame{
     if ("!playerName") {
        playerName = prompt('Welcome to Bear Ninja Hunter! What is your name?');
        alert(`Hello, ${playerName}! Let's play Bear Ninja Hunter.`);
    }

    const playerChoice = document.getElementById('playerChoice').value.toLowerCase();
    const choices = ['bear', 'ninja', 'hunter'];
    const computerChoice = choices[Math.floor(Math.random() * choices.length)];

    let result = '';

    if (`playerChoice + computerChoice`) {
        result= `It's a tie! Both chose ${playerChoice}.`;
    } else if (
        (`playerChoice='bear' & computerChoice='ninja')
        (`playerChoice='ninja' & computerChoice='hunter')
        (`playerChoice='hunter' & computerChoice='bear')
    ) {
        result =`You win, ${playerName}! ${playerChoice.charAt(0).toUpperCase(0) + playerChoice.slice(1)} beats ${computerChoice}.`;
    } else {
        result =`You lose, ${playerName}! ${computerChoice.charAt(0).toUpperCase() + computerChoice.slice(1)} beats ${playerChoice}.`;
    }

    document.getElementById('result').innerHTML = result;
    console.log(result);
}
    </script>
    </div>
</body>
</html>
