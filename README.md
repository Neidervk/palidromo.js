// # palidromo.js
//Identificador de palidromos

let str = prompt("Por favor escribe tu frase") 
       
 str = str.toLowerCase().replace(/[\W_]/g, '');

  for(i = 0, len = str.length - 1; i < len/2; i++) {
    if(str[i] !== str[len-i]) {
      alert ("La frase ( " + str + " ) NO es un palidromo");
      break
    }
    else {
        alert ("Felicidades la frase ( " + str + " ) es un palidromo");
        break
    }
  }
