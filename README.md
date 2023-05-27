# Sistema de Criptografia

Este repositório contém um programa em C que implementa um sistema de criptografia baseado nas regras especificadas no problema "PoliCripto" da Maratona de Programação InterFatecs 2022.

## Descrição do Problema

Um grupo político extremista deseja se comunicar de forma segura, evitando que suas conversas sejam interceptadas. No entanto, eles têm dificuldades com chaves públicas e privadas. Por isso, decidiram criar um código de comunicação que possa ser utilizado por qualquer pessoa, sem a necessidade de chaves.

O código é formado por duas sequências: uma composta apenas por caracteres minúsculos e outra por dígitos, além dos caracteres '+' e '-'. Os caracteres especiais não são permitidos na sequência de caracteres minúsculos.

Cada caractere na sequência de caracteres representa uma letra da mensagem original. O caractere 'w' exerce um papel especial e sempre representa um espaço na mensagem original. Assim, a sequência de caracteres pode ser inicialmente modificada para representar a mensagem decodificada corretamente.

Os números na sequência numérica indicam quantos caracteres acima ou abaixo cada caractere da sequência de caracteres deve ser modificado. Um número positivo N indica que o caractere em questão deve ser modificado pelo N-ésimo caractere após ele, seguindo a ordem alfabética. Um número negativo N indica que o caractere em questão deve ser modificado pelo N-ésimo caractere anterior a ele. O alfabeto é considerado circular, ou seja, após o 'z' vem o 'a' novamente e vice-versa.

A presença do caractere '-' na sequência numérica indica que todos os dígitos subsequentes são considerados negativos. Da mesma forma, a presença do caractere '+' indica que todos os dígitos subsequentes são considerados positivos. Caso não haja nenhum caractere '-', os números são considerados positivos por padrão.

## Solução

O programa desenvolvido neste repositório implementa a decodificação da mensagem criptografada usando as regras mencionadas acima. Ele recebe como entrada a mensagem codificada e a sequência numérica e retorna a mensagem original decodificada.

O programa é escrito em linguagem C e utiliza a biblioteca padrão `<stdio.h>` para entrada/saída e manipulação de strings, e a biblioteca `<stdlib.h>` para alocação de memória.

Ele lê a mensagem codificada e a sequência numérica fornecidas pelo usuário, remove o caractere de nova linha e realiza a decodificação de acordo com as regras especificadas. O caractere 'w' é tratado de forma especial, representando um espaço na mensagem decodificada. Os demais caracteres são modificados de acordo com os números da sequência numérica.

Por fim, a mensagem decodificada é impressa na tela.

## Como utilizar

1. Compile o programa em C utilizando um compilador de sua preferência.
2. Execute o programa compilado.
3. Digite a mensagem codificada quando solicitado.
4. Digite a sequência numérica quando solicitado.
5. Aguarde a exibição da mensagem decodificada.

## Contribuição

Sinta-se à vontade para contribuir com melhorias para este programa. Você pode criar um fork deste repositório, fazer as alterações desejadas e enviar um pull request.

## imagem do Exercício

![primeira imagem](file.jpeg)
