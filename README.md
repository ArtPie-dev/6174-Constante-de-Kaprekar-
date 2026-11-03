# Constante de Kaprekar — 6174

![Linguagem C](https://img.shields.io/badge/Linguagem-C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![Matemática](https://img.shields.io/badge/Área-Matemática-blue?style=for-the-badge)
![Algoritmos](https://img.shields.io/badge/Área-Algoritmos-orange?style=for-the-badge)

## Sobre o projeto

Este projeto explora a **Constante de Kaprekar (6174)**, uma propriedade matemática descoberta pelo matemático indiano Dattatreya Ramchandra Kaprekar.

A atividade consiste em aplicar uma sequência de operações sobre um número de quatro algarismos, reorganizando seus dígitos em ordem crescente e decrescente e subtraindo o menor valor do maior. Ao repetir o procedimento, chega-se à constante 6174 para qualquer número elegível.

O objetivo acadêmico é praticar raciocínio lógico, manipulação de dígitos, operações aritméticas, validação de dados e estruturas de repetição.

## O que é a Constante de Kaprekar?

A constante 6174 é obtida por meio de uma rotina matemática:

1. Escolha um número de quatro algarismos que possua pelo menos dois dígitos diferentes.
2. Organize os algarismos em ordem decrescente.
3. Organize os mesmos algarismos em ordem crescente.
4. Subtraia o menor número do maior.
5. Repita o processo com o resultado, mantendo quatro algarismos e incluindo zeros à esquerda quando necessário.
6. Continue até alcançar 6174.

Para números elegíveis de quatro algarismos, a rotina chega a 6174 em no máximo sete iterações. Quando o resultado é 6174, o procedimento permanece nesse valor.

## Exemplo de funcionamento

Considere o número `3524`.

| Etapa | Ordem decrescente | Ordem crescente | Subtração |
|---|---:|---:|---:|
| 1 | 5432 | 2345 | 3087 |
| 2 | 8730 | 0378 | 8352 |
| 3 | 8532 | 2358 | 6174 |

A constante é alcançada na terceira iteração.

## Regra importante

A rotina não funciona da mesma maneira para números formados por quatro dígitos iguais, como `1111` ou `7777`.

Nesses casos, a subtração resulta em `0000`, e o processo não chega a 6174.

Por isso, a validação do número de entrada é importante para garantir que o algoritmo seja aplicado corretamente.

## Tecnologias e conceitos

- **Linguagem C:** implementação do algoritmo.
- **Operações aritméticas:** cálculo da diferença entre os números.
- **Manipulação de dígitos:** separação e reorganização dos algarismos.
- **Estruturas condicionais:** verificação das condições de entrada e término.
- **Estruturas de repetição:** execução sucessiva da rotina.
- **Validação de dados:** tratamento de números que não atendem aos requisitos.

## Como executar

### Pré-requisitos

- Compilador C, como o GCC; ou
- Ambiente de desenvolvimento compatível com C.

### 1. Clone o repositório

```bash
git clone https://github.com/ArtPie-dev/6174-Constante-de-Kaprekar-.git
```

### 2. Acesse a pasta

```bash
cd 6174-Constante-de-Kaprekar-
```

### 3. Localize o código-fonte

O repositório contém uma pasta chamada `6174`. Entre nela e identifique o arquivo `.c` que implementa o algoritmo.

### 4. Compile o programa

Substitua `main.c` pelo nome real do arquivo-fonte:

```bash
gcc main.c -o kaprekar
```

### 5. Execute

No Linux:

```bash
./kaprekar
```

No Windows:

```bash
kaprekar.exe
```

## Casos de teste sugeridos

| Entrada | Resultado esperado |
|---|---|
| `3524` | Alcança 6174 em três iterações |
| `2111` | Alcança 6174 após aplicar a rotina |
| `6174` | Permanece em 6174 |
| `1111` | Não alcança 6174; a diferença é zero |
| `0001` | Alcança 6174 em sete iterações |

As entradas devem ser tratadas de acordo com as regras de validação implementadas no código. `0001` representa um número de quatro algarismos com zero à esquerda.

## Demonstração

Adicione capturas reais do programa em execução, mostrando a entrada, as operações realizadas e o resultado final.

Sugestão de estrutura:

```text
evidencias/
├── exemplo-3524.png
├── resultado-6174.png
└── validacao-entrada.png
```

## Aprendizados

Este projeto permite compreender como um problema matemático pode ser transformado em um algoritmo, além de desenvolver habilidades de manipulação numérica, validação de dados e controle de repetição.

## Autor

**Arthur Pierre de Aguiar da Silva**

Estudante de Ciência da Computação.

## Licença

Consulte o arquivo `LICENSE` do repositório para verificar as condições de utilização e distribuição do código.
