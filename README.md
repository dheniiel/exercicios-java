# Exercícios em Java

Exercícios básicos de Java feitos para praticar e aprender a linguagem: entrada de dados pelo console, manipulação de strings, operações matemáticas e os primeiros passos em orientação a objetos.

## Tecnologias

- Java 11
- Maven
- `java.util.Scanner` para leitura de dados do teclado

## Estrutura

```
Exercicios-em-Java/
├── exercicio_proposto/
│   └── src/main/java/
│       ├── exercicio_1/     Soma
│       ├── exercicio_2/     Cadastro
│       ├── exercicio_3/     CalculadoraIMC
│       ├── exercicio_4/     Conta, Banco
│       └── exercicioaula/   Aluno, Curso, Turma, Matricula, App
└── exercicios2/
    └── src/main/java/
        ├── lista1/          Maisculo, Email
        └── lista2/          Funcionario, Teste
```

## Exercícios

### `exercicio_proposto`

| Exercício | Classe | O que faz |
|---|---|---|
| 1 | `Soma` | Lê dois números inteiros e exibe a soma. |
| 2 | `Cadastro` | Lê nome, endereço e telefone e exibe os dados em uma linha. |
| 3 | `CalculadoraIMC` | Lê nome, peso e altura e calcula o IMC (peso / altura²). |
| 4 | `Banco` + `Conta` | Simula uma conta bancária com saldo e limite: realiza saque (usando o limite quando o saldo não basta) e depósito, informando o resultado de cada operação. |
| Aula | `App` + `Aluno`, `Curso`, `Turma`, `Matricula` | Modela um sistema escolar com classes relacionadas. O `App` cadastra 3 alunos e seus cursos em vetores e depois lista todos. |

### `exercicios2`

| Lista | Classe | O que faz |
|---|---|---|
| 1 | `Maisculo` | Lê um nome e o exibe em letras maiúsculas. |
| 1 | `Email` | Gera uma sugestão de e-mail a partir do nome: remove espaços, converte para minúsculas e adiciona `@gmail.com`. |
| 2 | `Teste` + `Funcionario` | Cadastra um funcionário (nome, função, salário), aplica um aumento e calcula o salário anual (12 meses). |

## Conceitos praticados

- Leitura de dados com `Scanner` (`nextLine`, `nextInt`, `nextDouble`, `nextFloat`)
- Operadores aritméticos e `Math.pow`
- Métodos de `String`: `toUpperCase`, `toLowerCase`, `trim`, `replaceAll`
- Estruturas condicionais (`if / else if / else`) e laços `for`
- Vetores de objetos
- Classes, atributos, construtores e métodos
- Encapsulamento com atributos `private` e getters
- Associação entre classes (`Turma` → `Curso`, `Matricula` → `Aluno` e `Turma`)

## Como executar

Pré-requisitos: JDK 11+ (Maven é opcional).

Abra o projeto (`exercicio_proposto` ou `exercicios2`) em uma IDE como NetBeans, IntelliJ ou VS Code e execute a classe que contém o método `main`.

Pelo terminal, a partir da pasta do projeto:

```bash
cd exercicio_proposto
javac -d target/classes src/main/java/exercicio_1/Soma.java
java -cp target/classes exercicio_1.Soma
```

Classes com `main`: `Soma`, `Cadastro`, `CalculadoraIMC`, `Banco`, `App`, `Maisculo`, `Email` e `Teste`.

Para compilar e rodar exercícios com mais de uma classe (como `Banco` ou `App`), compile o pacote inteiro:

```bash
javac -d target/classes src/main/java/exercicio_4/*.java
java -cp target/classes exercicio_4.Banco
```

## Autor

Dheniel — [@dheniiel](https://github.com/dheniiel)
