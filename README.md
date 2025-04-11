# Prova-Bi-1

# Ex 1:
function somar (a,b) {// O nome da função é "Somar"
// parametros
return a + b; //
}
console.log ("Função soma: ", somar)

# Ex 2: 
Alternativa: E

# Ex 3:
// 1. Crie uma função chamada registrarPedido que receba cliente, prato, mesa e idade
function registrarPedido (cliente, prato, mesa, idade){
    return {
        cliente: cliente,
        prato: prato,
        mesa: mesa,
        idade: idade
    };
}

// 2. Crie um array vazio chamado pedidos
let pedidos = [];

// 3. Adicione 3 pedidos ao array usando a função criada
pedidos.push({cliente: "Ana", prato: "Hambúrguer",mesa: 1, idade: 10});
pedidos.push ({cliente: "Bruno",prato: "Lasanha",mesa: 2,idade: 17});
pedidos.push ({cliente: "Carlos",prato: "Feijoada",mesa: 3,idade: 65});


// 4. Crie uma função chamada classificarIngresso que retorna o tipo com base na idade

function  classificarIngresso (idade) {
    if (idade < 12) {
      return "Infantil";
    } else if (idade >= 12 && idade <= 17) {
      return "Adolescente";
    } else if (idade >= 18 && idade <= 59) {
      return "Adulto";
    } else {
      return "Sênior";
    }
  }

// 5. Atendimento dos pedidos (sem laço de repetição)
let pedido1 = pedidos.shift(1);
let tipo1 = classificarIngresso(pedido1.idade);
let valor1 = 29.9;
console.log("Cliente atendido:", pedido1.cliente);
console.log("Tipo de ingresso:", tipo1);
console.log("Valor da conta: R$", valor1.toFixed(2));
console.log("_________________________");

let pedido2 = pedidos.shift(2);
let tipo2 = classificarIngresso(pedido2.idade);
let valor2 = 31.9;
console.log("Cliente atendido:", pedido2.cliente);
console.log("Tipo de ingresso:", tipo2);
console.log("Valor da conta: R$", valor2.toFixed(2));
console.log("_________________________");

let pedido3 = pedidos.shift(3);
let tipo3 = classificarIngresso(pedido3.idade);
let valor3 = 29.9;
console.log("Cliente atendido:", pedido3.cliente);
console.log("Tipo de ingresso:", tipo3);
console.log("Valor da conta: R$", valor3.toFixed(2));
console.log("_________________________");

// 6. Exiba a quantidade de pedidos restantes
console.log("Pedidos restantes:", pedidos.length);

# Ex 4:
Alternativa: C

# Ex 5:
Alternativa: E
