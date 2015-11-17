# Artigo
**autor**: Marcelo Santana Martins

**Prazo**: at� dia 18 de Novembro de 2015

Explique, com teoria e c�digo, nesse artigo como o JavaScript cria e instancia as vari�veis, seguindo os seguintes t�picos.

## Hoisting

*Hoisting* � o procedimento executado pelo JavaScript de "mover" a declara��o de uma v�riavel para o topo de seu escopo, quando est� n�o for feita de forma expl�cita.

```
var idade; //declarada no escopo global

function exibeIdade(){    
    console.log(idade);
    var number = 27; //declarada no escopo de exibeIdade()
}

idade = 21;
exibeIdade();
```

No exemplo acima, ser� exibido *undefined* no console. Isso ocorre pois, como existe a declara��o da vari�vel idade dentro do escopo de exibeIdade() e ela se encontra no final, o pr�prio compilador se encarrega de declar�-la no topo do escopo.

Com isso, o c�digo ficaria da seguinte forma:

```
var idade;

function exibeIdade(){
    *var number; //hoisting de number*
    console.log(idade);
    number = 27;
}

idade = 21;
exibeIdade();
```


## Closure

Explique o que �, o porqu� acontece e como usar. 
Cite situa��es que voc� usaria.












## Vari�vel Global

Explique como se usa uma var Global dentro de uma fun��o.









## Vari�vel por par�metro

Explique o que acontece dentro da fun��o qnd um par�metro � passado e tamb�m explique quando uma GLOBAL � passada por par�metro.







## Instancia��o usando uma IIFE

Explique como uma vari�vel pode receber um valor de uma IIFE.
Explique como passar uma vari�vel por par�metro para a IIFE e acontece com ela dentro da fun��o.







## Considera��es

Quanto mais explicado melhor.

Lembre que isso far� parte do seu curr�culo como aluno e ser� disponilizado no sistema de vagas, ou seja, o contratante poder� ver todos seus projetos e trabalhos feitos nesse curso.

Boa sorte.

# Envio

1. Fork [esse reposit�rio](https://github.com/Webschool-io/be-mean-instagram-artigos/) 
2. Nomeie seu artigo usando o seguinte padr�o: artigo-instanciacao-githubuser-nome-completo.md
3. Adicione seu exerc�cio aqui na Pasta Variables
4. Fa�a um Pull Requst enviando seu artigo.