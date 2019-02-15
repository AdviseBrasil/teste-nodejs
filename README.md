# Advise - Teste prático para back-end 

## Pré-requisitos

- JavaScript
- NodeJS
- MySQL ou MSSQL
- REST

## Desafio
Você deverá desenvolver uma API REST para gerenciar produtos e categorias de produtos. Dessa forma, deverá existir rotas para o CRUD tanto das categorias quanto dos produtos.
Além disso, deverá haver uma rota para calcular o valor das parcelas do produto seguindo a seguinte tabela:

| Categoria   | %   |
|-------------|-----|
| Informática | 5   |
| Automotivo  | 2.5 |
| Móveis      | 1   |

Lembrando que os juros são mensais, portanto, deverá ser utilizado a seguinte formula para calcular o valor da parcela:

~~~~
pv * i / (1 - Math.pow(1 + i, -n))
~~~~

- pv = valor do produto
- i  = porcentagem do juros dividido por 100. (Ex. 10% = 10 / 100 = 0.1)
- n  = número de parcelas

### O que esperamos 
1. Uso de validadores na rota.
2. Testes unitários.
3. Documentação.


### O que nos impressionaria
- Alguma metodologia para definição e organização do seu código.
- Conteinerização da aplicação.

### O que não gostaríamos
- Saber que não foi você quem fez seu teste.
- Ver commits gigantes, sem mensagens ou com mensagens sem sentido.

## O que avaliaremos de seu teste
1. Funcionamento e método de resolução do problema.
2. Organização do código.
3. Performance do código.
4. Documentação da API.
5. Arquitetura do projeto.
6. Semântica, estrutura, legibilidade, manutenibilidade, escalabilidade do seu código e suas tomadas de decisões.
7. Históricos de commits do git.

### Dúvidas
Mande um e-mail para nós.

### Observação
Não esqueça de nos mandar o dump do banco utilizado.

* As tabelas deverão ter no minimo os seguintes campos:
    * Produtos

        | Campo      | Obrigatório |
        |------------|-------------|
        | id         |             |
        | nome       | sim         |
        | descricao  | sim         |
        | valor      | sim         |
        | idCategoria| sim         |

    * Categoria

        | Campo      | Obrigatório |
        |------------|-------------|
        | id         |             |
        | nome       | sim         |