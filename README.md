# Entrega: Tabela de Multiplicação

## Visão Geral

Para começar, acesse [este link](https://classroom.github.com/a/5RDmDMXi) e clone o repositório em sua máquina.

Construa uma função que recebe um parâmetro _n_ do tipo inteiro que permita a geração de tabelas de diferentes tamanhos (por exemplo, 12x12, 16x16)

Escreva uma página HTML que use Javascript para desenhar uma tabela de multiplicação no console do navegador. A ideia chave aqui é usar dois loops aninhados _(um loop dentro de outro)_ para costruir um array aninhado _(bidimencional)_ que você vai utilizar para desenhar as linhas e colunas da tabela.

Imagine que você está construindo uma tabela para que professores do ensino fundamental a usem em sala de aula. Ela deve ficar mais ou menos assim, executando com o parâmetro n valendo 10:

![](https://i.snag.gy/xf0HnX.jpg)

### Início

Você pode usar o seguinte documento HTML como ponto de partida:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Multiplication Table</title>
  </head>

  <body>
    <h1>Multiplication Table</h1>
    <script>
      function tabelaMultiplicacao(n) {
        let x = [];
        for (let i = 0; i <= n; i++) {
          x[i] = [];

          for (let j = 0; j <= n; j++) {
            x[i][j] = i * j;
          }
        }
        console.table(x);
      }
    </script>
  </body>
</html>