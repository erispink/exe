#CSS GRID

## GRID

-Bimensional
-Divisão de toda a página em linhas e colunas
-Colocar elementos onde quiser nessa divisão 

## GRID OU FLEXBOX
- Grid: Duas dimensões (colunas e linhas)
- Flexbox: Uma dimensão (ou coluna ou linha)
- Um complementa o trabalho do outro
Verodofcar quais navegadores ainda não estão aceitando o Grid

## PROPRIEDADES 

Vamos separar em 2 grupos:
'container' e 'item (s)' 

### CONTAINER 

- display: grid; - inicia o container como grid 
- grid-template-columns; - começa a fatiar as colunas, quanto elas possuem 
- grid-template-rows; - quantas linhas 
- grid-gap - espaçamentos
    -grid-row-gap
    -grid-column-gap
-grid-template-areas; - delimita areas 
... e mais 4 propriedades e **alinhamento**

## ITEM (s)

- grid-column - onde vai ficar o item na coluna 
    - grid-column-start
    - grid-column-end
-grid-row - onde fica na linha
    - grid-row-start
    - grid-row-end
- grid-area 
... e mais 2 propriedades e **alinhamento**

// SHORTHANDS
    grid-gap: 20px 50px
grid-row-gap: 20px;
grid-column-gap: 50px;

    grid-column: 1/3;
grid-column-start: 1;
grid-column-end: 3; 
    grid-row: 3/4;
grid-row-start: 3;
grid-row-end: 4;
//

// AREAS 

header {
  background: yellow;
  grid-area: header;
}

container {
grid-template-areas: "header ."
    "main a"
    ". f"
} * o ponto é caso eu queira um espaço vazio 

------------------------------------------------

#GRID: ALINHAMENTO

1.justify-content 
2.align-content
3.justify-items
4.align-items
5.justify-self
6. align-self 

Separando em 2 grupos 
1. justify e align
2. content, itens e self

# JUSTIFY E ALIGN
Sabendo que o grid é bidimensional, nós temos o eixo x e o eixo y.
O EIXO X é o posicionamento horizontal da esquerda para a direita.
O EIXO Y é o posicionamento vertical de cima para baixo.  

# CONTENT, ITENS E SELF
Juntando o justify ou align, com esses elementos content, itens e self, nós observamos nossas propriedades 

---
## CONTENT
'justify-content' e 'align-content' nos permitem alinhar o proprio grid, relativo ao espaço fora do grid. 
O uso dess propriedades raras pois só é aplicado caso o grid seja menor que a área definida.

VALORES 
1. start
2. end
3. center
4. stretch
5. space-between
6. space-around
7. space-evenly 