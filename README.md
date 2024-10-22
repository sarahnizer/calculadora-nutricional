function calculateCalories() {
  const age = parseInt(document.getElementById('age').value);
  const weight = parseFloat(document.getElementById('weight').value);
  const height = parseInt(document.getElementById('height').value);
  const goal = document.getElementById('goal').value;
  
  let result = document.getElementById('result');
  
  let BMR = 10 * weight + 6.25 * height - 5 * age +5;
  
  let calories;
  let protein, carbs, fats;
  let mealSuggestions = "";
  let sleepRecommendation = "Recomenda-se dormir entre 7-9 horas por noite para otimizar a recuperação e o bem-estar";
  
  if (goal === "maintain") {
    calories = BMR * 1.55;
    protein = weight * 1.8;
    carbs = weight * 4;
    fats = weight * 1;
    
    mealSuggestions = `<p><strong> Sugestão de Cardápio para manter massa</strong></p>
    <ul>
      <li>Café da manhã: Iogurte grego, amêndoas ou nozes, granola integral e frutas frescas.</li>
     <li>Almoço: Peito de frango grelhado, mix de verduras e batata doce assada.</li>
    <li>Lanche: Banana com aveia.</li>
    <li>Jantar: Salmão, quinoa e aspargos.</li>
    </ul>`   
    ;
  } else if (goal === "gain"){
    calories = BMR * 1.2;
    protein = weight * 2;
    carbs = weight * 2;
    fats = weight * 0.7;
    
     mealSuggestions = `<p><strong> Sugestão de Cardápio para ganhar massa</strong></p>
    <ul>
      <li>Café da manhã: Iogurte natural com frutas. </li>
     <li>Almoço: Salada de Frango Grelhado com Misto de Verduras e Vegetais. </li>
    <li>Lanche: Frutas com pasta de amendoim. </li>
    <li>Jantar: Peito de frango com batata doce e salada. </li>
    </ul>`    
     ;
  } else if (goal === "lose") {
    calories = BMR * 1.75;
    protein = weight * 2;
    carbs = weight * 5;
    fats = weight * 1;
    
     mealSuggestions = `<p><strong> Sugestão de Cardápio para perder peso</strong></p>
    <ul>
      <li>Café da manhã: Frutas frescas com iogurte natural. </li>
     <li>Almoço: Frango assado, arroz com brócolis e purê de batata. </li>
    <li>Lanche: chips de batata doce. </li>
    <li>Jantar: berinjela no forno com tomate-cereja e queijo. </li>
    </ul>`    
    ;
 }
 result.innerHTML =`
 <p> Sua necessidade calórica diária estimada é de ${calories.toFixed(2)} calorias.</p>
 
 <p> Para atingir seu objetivo, você deve ingerir: </p>
 <ul>
    <li>${protein.toFixed(2)}g de proteínas por dia. </li>
    <li>${protein.toFixed(2)}g de carboidratos  por dia. </li>
    <li>${protein.toFixed(2)}g de gorduras por dia. </li>
 </ul>
 
 
 ${mealSuggestions}
 <p>${sleepRecommendation}</p>
 <p><strong>Hidratação:</strong> tente beber cerca de ${(weight * 0.035).toFixed(2)} litros de água por dia</p>
 
 `
 }

