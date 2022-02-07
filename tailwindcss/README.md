# UTILIZANDO  TAILWIND CSS NA PRÁTICA :: PRIMEIRO CONTATO

## PONTOS POSITIVOS
Basea-se na aplicação de utilidade, ou seja, utiliza classes pré-criadas para ir construindo o objeto do zero, dando maior liberdade de customização para o desenvolvedor. Exemplo de aplicação:
```
<div class="font-semilbold mt-4 mb-5 text-xl lg:text-xl">Exemplo</div>
```

## PONTOS NEGATIVOS
Por depender de classes de utilidade, torna o HTML extremamente poluído, sem contar que a nomenclatura das classes não é nem um pouco semântica, podendo tornar a manutenção posterior um completo caos.


## SOLUÇÃO 
O próprio framework dá uma solução alternativa, que é a utilização do *@apply*, onde pode-se criar uma classe totalmente semântica, seguindo a metodologia BEM (Block, Element, Modifier), sem precisar perder todos os recuros úteis que tem a oferecer. Exemplo:
~~~html
<div class="container">Exemplo</div>
~~~
~~~css
.container{ @apply font-semilbold mt-4 mb-5 text-xl lg:text-xl; }
~~~

** Utilizando o @apply dessa forma, é muito mais prático criar componentes, reutilizar estruturas de código, e a customização também se torna mais fácil.

