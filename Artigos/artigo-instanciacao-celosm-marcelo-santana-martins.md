# Artigo
**autor**: Marcelo Santana Martins

**Prazo**: até dia 18 de Novembro de 2015

Explique, com teoria e código, nesse artigo como o JavaScript cria e instancia as variáveis, seguindo os seguintes tópicos.

## Hoisting

*Hoisting* é o procedimento executado pelo JavaScript de "mover" a declaração de uma váriavel para o topo de seu escopo, quando está não for feita de forma explícita.

```
var idade; //declarada no escopo global

function exibeIdade(){    
    console.log(idade);
    var number = 27; //declarada no escopo de exibeIdade()
}

idade = 21;
exibeIdade();
```

No exemplo acima, será exibido *undefined* no console. Isso ocorre pois, como existe a declaração da variável idade dentro do escopo de exibeIdade() e ela se encontra no final, o próprio compilador se encarrega de declará-la no topo do escopo.

Com isso, o código ficaria da seguinte forma:

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

Explique o que é, o porquê acontece e como usar. 
Cite situações que você usaria.












## Variável Global

Explique como se usa uma var Global dentro de uma função.









## Variável por parâmetro

Explique o que acontece dentro da função qnd um parâmetro é passado e também explique quando uma GLOBAL é passada por parâmetro.







## Instanciação usando uma IIFE

Explique como uma variável pode receber um valor de uma IIFE.
Explique como passar uma variável por parâmetro para a IIFE e acontece com ela dentro da função.







## Considerações

Quanto mais explicado melhor.

Lembre que isso fará parte do seu currículo como aluno e será disponilizado no sistema de vagas, ou seja, o contratante poderá ver todos seus projetos e trabalhos feitos nesse curso.

Boa sorte.

# Envio

1. Fork [esse repositório](https://github.com/Webschool-io/be-mean-instagram-artigos/) 
2. Nomeie seu artigo usando o seguinte padrão: artigo-instanciacao-githubuser-nome-completo.md
3. Adicione seu exercício aqui na Pasta Variables
4. Faça um Pull Requst enviando seu artigo.