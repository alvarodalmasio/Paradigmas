# Atividade: Derivação de um Código a partir da Gramática da Linguagem C#

## 1. Linguagem escolhida

A linguagem escolhida para a realização desta atividade foi a linguagem **C#**.

O C# é uma linguagem de programação que possui uma especificação formal, contendo regras que definem como os elementos da linguagem devem ser organizados para formar um código válido.

## 2. Fonte da gramática consultada

A fonte consultada foi a documentação oficial da Microsoft, que apresenta a especificação da linguagem C#, incluindo suas regras gramaticais.

Fonte:

https://learn.microsoft.com/pt-br/dotnet/csharp/language-reference/language-specification/grammar

A gramática do C# é apresentada utilizando uma notação formal baseada em regras de produção. Para esta atividade, foram utilizadas apenas algumas regras necessárias para demonstrar a derivação de um pequeno trecho de código.

## 3. Regras de produção selecionadas

As regras foram escolhidas para permitir a criação de uma instrução de atribuição com uma expressão de adição.

De forma simplificada, as regras utilizadas são:

```text
<instrucao> ::= <atribuicao> ";"

<atribuicao> ::= <identificador> "=" <expressao>

<expressao> ::= <numero>
              | <numero> "+" <numero>

<identificador> ::= "x"

<numero> ::= "1" | "2"
```

A regra `<instrucao>` representa uma instrução completa terminada com ponto e vírgula.

A regra `<atribuicao>` representa a atribuição de um valor a uma variável.

A regra `<expressao>` permite utilizar um número sozinho ou realizar uma operação de adição entre dois números.

A regra `<identificador>` representa o nome da variável utilizada no exemplo.

A regra `<numero>` representa os valores numéricos utilizados na expressão.

## 4. Código que será derivado

O código escolhido para ser derivado foi:

```csharp
x = 1 + 2;
```

Esse código foi escolhido por ser simples e permitir demonstrar uma atribuição e uma expressão aritmética.

## 5. Derivação passo a passo

A derivação começa pelo símbolo inicial:

```text
<instrucao>
```

Aplicando a primeira regra:

```text
<instrucao>
⇒ <atribuicao> ";"
```

Aplicando a regra de atribuição:

```text
⇒ <identificador> "=" <expressao> ";"
```

Substituindo o identificador:

```text
⇒ "x" "=" <expressao> ";"
```

Aplicando a regra da expressão com adição:

```text
⇒ "x" "=" <numero> "+" <numero> ";"
```

Substituindo o primeiro número:

```text
⇒ "x" "=" "1" "+" <numero> ";"
```

Substituindo o segundo número:

```text
⇒ "x" "=" "1" "+" "2" ";"
```

Portanto, o código final obtido pela derivação é:

```csharp
x = 1 + 2;
```

## 6. Identificação dos terminais e não terminais

Os símbolos não terminais são aqueles que representam estruturas da gramática e ainda podem ser substituídos por outras regras durante a derivação.

Os símbolos não terminais utilizados foram:

```text
<instrucao>
<atribuicao>
<identificador>
<expressao>
<numero>
```

Os símbolos terminais são aqueles que aparecem no código final e não precisam ser substituídos.

Os símbolos terminais utilizados foram:

```text
x
=
1
+
2
;
```

## Conclusão

A atividade demonstrou como uma gramática formal pode ser utilizada para gerar um trecho de código válido em C#.

O processo começou com o símbolo `<instrucao>`. Em seguida, foram aplicadas regras de produção para formar uma atribuição, definir o identificador, criar uma expressão de adição e substituir os números pelos valores finais.

Ao final da derivação, foi obtido o código:

```csharp
x = 1 + 2;
```

Dessa forma, foi possível identificar que os símbolos não terminais representam as estruturas que podem ser desenvolvidas durante a derivação, enquanto os símbolos terminais representam os elementos finais que aparecem no código gerado.
