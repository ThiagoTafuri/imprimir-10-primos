const n = parseFloat(prompt("Digite um número: "));
let contador = 0
let primos = 0
for(let i = n ; n > 1 ; i--){
    let ehprimo = true;
    for(let j = 2 ; j < i ; j++){
        if(i % j === 0){
            ehprimo = false;
            break;
        }

    }
    if(ehprimo){
        primos = i
        contador++
        console.log(primos)
    }
    if (contador == 10 || i == 2){
        break;
    }
}
