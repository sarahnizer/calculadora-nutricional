body{
  font-family: 'Roboto', sans-serif;
  background-image: url(https://danielsoutoortopedista.com.br/wp-content/uploads/2021/06/top-view-of-assortment-of-healthy-food-1024x683.jpg);
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
  margin: 20px;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.container{
  background-color: transparent;
  padding: 30px;
  box-shadow: 0 4px 12px rgba(0,0,0,1);
  width: 100%;
  max-width: 450px;
  border-radius: 15px;
 transition: transform 0.3s ease-in-out;
}

.container:hover{
  transform: scale(1.03);
}

h1{
  text-align: center;
  margin-bottom: 25px;
  font-size: 2.5em;
  color: white;
  text-shadow: 3px 3px 3px black;
}

form{
  display: flex;
  flex-direction: column;
}
 
label{
  margin-bottom: 8px;
  color: white;
  text-shadow: 2px 2px 2px black;
}

input, select, button{
  padding: 12px;
  margin-bottom: 10px;
  border: 1px solid black;
  border-radius: 8px;
  font-size: 1em;
  transition: border 0.3s ease, box-shadow 0.3s ease;
}

input:focus, select:focus{
  border-color: #eb3434;
  outline: none;
  box-shadow: 0 0 8px #87658f;
}

button{
  background-color: #eb3434;
  color: white;
  border: none;
  cursor: pointer;
  box-shadow: 1px 4px 6px grey;
  transition: background-color 0.3s ease, box-shadow 0.3s ease;
}

button:hover{
  background-color: #b34e3d;
  box-shadow: 1px 3px 6px black;
}

#result{
  margin-top: 25px;
  padding: 15px;
  background-color: #eb3434;
  border-radius: 8px;
  font-size: 1em;
  color: white;
  text-align: center;
}

