## CSS Container

Usar containers no CSS é uma prática fundamental para estruturar e organizar o layout de uma página web. Eles são usados para envolver o conteúdo e definir o ponto de partida para o sistema de grid responsivo.

- Organização e Estruturação: Containers ajudam a dividir o conteúdo em seções, facilitando a organização do layout e tornando o código mais legível e fácil de manter.

- Responsividade: Containers permitem o controle do comportamento responsivo do layout. Usando técnicas como flexbox ou grid, você pode ajustar o tamanho, a ordem e a disposição dos elementos em diferentes tamanhos de tela.

- Controle de Estilo: Ao aplicar estilos diretamente aos containers, você pode controlar o espaçamento (margens e preenchimentos), alinhamento e outras propriedades CSS de todos os elementos contidos neles de forma centralizada.

- Isolamento de Estilos: Containers permitem que você isole estilos específicos de uma seção do site. Isso evita que estilos indesejados vazem para outras partes da página, mantendo a consistência visual.

- Flexibilidade no Layout: Containers fornecem flexibilidade para criar layouts complexos, como colunas e grids, e ajustar a disposição dos elementos de acordo com o design desejado.

- Centralização de Conteúdo: É comum usar containers para centralizar o conteúdo horizontalmente na página, proporcionando uma melhor experiência visual para o usuário.

### Container que eu utilizo

Abaixo estão os tamanhos de container que utilizo para diferentes resoluções de dispositivos. Esses tamanhos são ajustados para garantir uma experiência visual que eu considero ideal em diversos tamanhos de tela:

| Breakpoint | Largura Máxima | Largura do Container |
| ---------- | -------------- | -------------------- |
| small      | 768px          | 750px                |
| medium     | 992px          | 970px                |
| large      | 1200px         | 1170px               |
| huge       | 1440px         | 1366px               |

O CSS a seguir demonstra como aplicar os diferentes tamanhos de container usando media queries:

```css
.container {
  padding: 0 20px;
  margin: 0 auto;
}

@media (min-width: var(--breakpoint-small)) {
  .container {
    width: var(--container-small);
  }
}

@media (min-width: var(--breakpoint-medium)) {
  .container {
    width: var(--container-medium);
  }
}

@media (min-width: var(--breakpoint-large)) {
  .container {
    width: var(--container-large);
  }
}

@media (min-width: var(--breakpoint-huge)) {
  .container {
    width: var(--container-huge);
  }
}
```
