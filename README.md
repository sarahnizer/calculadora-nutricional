<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Calculadora Nutricional</title>
</head>
<body>
  <div class="container">
    <h1>Calculadora Nutricional</h1>
    <form id="calcForm">
      <label for="age">Idade:</label>
      <input type="number" id="age" name="age" required>
      
      <label for="weight">Peso (kg):</label>
      <input type="number" id="weight" name="weight" required>
      
      <label for="height">Altura (cm):</label>
      <input type="number" id="height" name="height" required>
      
      <label for="goal">Objetivo:</label>
      <select name="goal" id="goal">
        <option value="maintain">Manter Peso</option>
        <option value="lose">Perder Peso</option>
        <option value="gain">Ganhar Peso</option>
      </select>
      
      <button type="button" onclick="calculateCalories()">Calcular</button>
    </form>
    
    <div id="result"></div>
  </div>
</body>
</html>
