# Expressões regulares

## Objetivo

Implemente em Python 3 um _matcher_ de expressões regulares. Dada uma expressão regular e uma palavra, sua implementação deve dizer **OK** ou **Not OK** quando a palavra dada "casa" com a expressão regular dada.

## Implementação 

Sua implementação deve ser organizada da seguinte forma.

1. Transformador de expressões regulares (ER) à autômatos finitos não-determinísticos com transições vazias (AFNe).  

   A função `erToAFNe : ER -> AFNe` deve receber uma expressão regular pré-fixadas e retornar um AFNe que reconheça palavras que "casam" com a expressão regular e somente estas. 
   
   Uma expressão regular pré-fixada é dada, por exemplo por `+(.(a, b), c)`, representando a ER `ab + c`.
   
   O transformador deve immplementar o algoritmo definido no livro-texto.

3. Transformador de AFNe à autômatos finitos não-determinísitcos (AFD).
4. Transformador de AFD à AFD mínimo.
5. Simiulador de AFD.
