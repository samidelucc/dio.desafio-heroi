# Desafio DIO - Classificação de nível de herói

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://github.com/samidelucc/dio.desafio-heroi)
[![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/samidelucc)
[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rodriguest/)

-------

## Realizado em JavaScript, o desafio consiste em criar um programa para nomear um herói e classifica-lo de acordo com o nível de pontos de experiência (xp), seguindo a tabela abaixo

Experiência (XP) | Classificação
------------------|-------------
Menor que 1.000 | Ferro
entre 1.001 e 2.000 | Bronze
entre 2.001 e 5.000 | Prata
entre 5.001 e 7.000 | Ouro
entre 7.001 e 8.000 | Platina
entre 8.001 e 9.000 | Ascendente
entre 9.001 e 10.000| Imortal
maior ou igual a 10.001 | Radiante


 ### Para começar a resolução do desafio, foi criada uma função com o nome *classificador*, e o seu parâmetro *(xp)*, que posteriormente permitirá uma atribuição de valores quando a função for chamada

~~~ 
function classificador(xp) {
    (...)
}
~~~

### Depois, foi atribuído com a variável *let* o nome *classificacao*, que retornará mais a diante a classificação de xp, de acordo com a tabela vista anteriormente, além das estruturas de decisão e dos operadores

~~~    
let classificacao;
    if (xp < 1000) {
        classificacao = "Ferro";
    } else if (xp >= 1001 && xp <= 2000) {
        classificacao = "Bronze";
    } else if (xp >= 2001 && xp <= 5000) {
        classificacao = "Prata";
    } else if (xp >= 5001 && xp <= 7000) {
        classificacao = "Ouro";
        (...)
} else {
    classificacao = "XP inválido";
}   
~~~

* As estruturas de decisão *if, else if e else*, juntos a variável *xp* e dos operadores relacionais *maior (>=) e menor (<=)* e do operador lógico *&&*, irão imprimir a mensagem da classificação do herói quando forem chamados pela variável *classificacao*.

### em seguida, foi atribuído o retorno, para retornar com o valor da variável *classificacao*, como dito anteriormente.

~~~ 
    (...)
}
    return classificacao;
}
~~~

### Para o programa funcionar, foi criada com a variável *let* o nome *heroi*, com o valor "Batman". Junto a ela, foi criada outra variável com o nome *xp* de valor *7500* 

~~~
let heroi = "batman"
let xp = 7500
~~~

### Por fim, foi criado um *console* para imprimir a mensagem, informando o nome do herói, sua classificação em números e o seu nível, utilizando templates literais `` e *${}*, que retornam os valores da função *classificador(xp)* e das variáveis *heroi* e *XP*.

~~~
console.log(`A classificação para o herói ${heroi} é ${xp}, sendo o nível ${classificador(xp)}`);
~~~

`"A classificação para o herói Batman é 7500, sendo o nível Platina"`

* Como o valor atribuído a função para retornar a classificação da variável *xp* é 7500, a classificação a ser impressa será "Platina", que corresponde "*entre 7.001 e 8.000*"

com esta última linha, o programa fica completo e funcional, primeiro informando a classificação do herói de acordo com a tabela, e depois a sua informação completa, com o seu nome e nível.

> Para a realização do código, foram utilizados Variáveis, Operadores, Laços de repetição e Estruturas de Decisão na linguagem de programação JavaScript.
----
