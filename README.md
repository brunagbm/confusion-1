# Aula 10 - React Components - props

# MenuComponent.js

### Imports utilizados

```js
import React, { useState } from 'react'; 
import { Card, CardImg, CardImgOverlay, CardText, CardBody, CardTitle } from 'reactstrap';
```

- O import de React traz o núcleo da biblioteca React, enquanto useState permite gerenciar o estado em componentes funcionais. Os componentes Card, CardImg, CardImgOverlay, CardText, CardBody, e CardTitle são importados da biblioteca reactstrap para criar e estilizar cartões de conteúdo de forma simples e responsiva.

### Componentes usados e suas funções

- `React`: importante para contruir interfaces do usuário ou para usar o JSX;
- `Card`: o card é o container para exibir textos, imagens ou links;
- `CarImg`: usado dentro de um card para exibir uma imagem dentro do cartão, ou seja o `Card`;
- `CardImgOverlay`: esse vai adicionar uma sobreposição de imagem dentro de um cartão, que seria a imagem dentro do `CardImg`;
- `CardText`: como o nome já diz, esse vai subir um texto dentro do corpo cartão;
- `CardBody`: é o corpo do cartão, onde vai ser colocado o conteúdo principal;
- `CardTitle`: aqui é colocado o título, que fica antes do body.

### Função do onDishSelect no projeto

- Nesse projeto ele é usado para a seleção de pratos, com interfaces interativas, como o menu do restaurante.
 
### Função do renderDish

- Tem a função de exibir as informações de um prato de forma estruturada.
 
### Função do props.dishes.map

-  É usada para iterar sobre a lista de pratos, ou seja, percorrer uma sequência de elementos e gera um novo componente ou elemento para cada prato.

# dishes.js

### Propriedades

- id, name, image, category, label, price, description, comments.

### Tipo de date utilizado

- ISO 8601: Ano/mês/data/hora/minutos/segundos

# App.js

### Função do oconst [dishes]

- Cria um estado dishes que armazena o array DISHES com os dados dos pratos.

### Funcionamento do <Menu dishes>

- envia o array dishes para o componente Menu, que exibe os pratos usando .map().
