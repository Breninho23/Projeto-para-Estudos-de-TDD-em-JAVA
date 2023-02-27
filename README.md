# Projeto-para-Estudos-de-TDD-em-JAVA

[![Express Logo](https://junit.org/junit4/images/junit5-banner.png)](https://junit.org/junit5/)

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=%20EM%DESENVOLVIMENTO&color=GREEN&style=for-the-badge)

O projeto em questão foi construido para fins de aprendizado em relação a Teste Automatizados em Java utilizando Junit.

## Classes

### Funcionario

A classe funcionario representa como o proprio nome diz um funcionario, possui apenas 3 campos, `nome`, `dataAdmissao` e `salario` .

### Desempenho

A classe Desempenho é um Enum utilizado para definir o percentual de reajuste do funcinario de acordo com o seu desempenho.

### ReajusteService

A classe ReajusteService é a classe que possui a lógica de calculo do bonus do funcionário com o método `concederReajuste` , nela é pego a porcentagem de reajuste do funcionário de acordo com o desempenho e é executado o método de reajustarSalario presente na classe funcionário.

### BonusService

A classe BonusService é uma classe que implementa um método com um Exception caso o funcionário tenha um salário maior que 1000 reias.

### BonusServiceTeste

A classe em questão possui uma anotação interessante para quem trabalha com junit, no caso a anotação `@BeforeEach` é utilizada para antes de ser executado um método com `@Test` ele executa o método anotado como `@BeforeEach`, no caso a anotação `@BeforeEach` nessa classe, é utilizada para inicializar valores ou classes.

Além disso ela importa a classe BonusService para poder executar os testes com 3 opções de valor para um funcionário.
