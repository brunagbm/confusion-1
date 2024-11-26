# React Components

## Importação de funcionalidades:

```js
import React, { useState } from 'react'
import { Media } from 'reactstrap'
```
- React = usado para criar as telas do app;
- useState = uma ferramenta do react que ajuda a guardar informações;
- Media = ele vai organizar textos e imagens.

## Primeiro bloco de código (Menu):

```js
const Menu = () => 
  const [dishes] = useState
            {
                id: 0,
                name: 'Uthappizza',
                image: 'assets/images/uthappizza.png',
                category: 'mains',
                label: 'Hot',
                price: '4.99',
                description: 
        'A unique combination of Indian Uthappam (pancake) and Italian pizza, ' + 
        'topped with Cerignola olives, ripe vine cherry tomatoes, Vidalia onion, ' + 
        'Guntur chillies and Buffalo Paneer.'
        },
```

- De ínicio há uma definição de um componente funcional chamado `Menu`, nela tem uma lista com atribuições sobres os pratos do menu.

## Segundo bloco de código (menu):

```js
const menu = dishes.map((dish) => {
        return (
            <div key={dish.id} className="col-12 mt-5">
                <Media tag="li">
                    <Media left middle>
                        <Media object src={dish.image} alt={dish.name} />
                    </Media>
                    <Media body className="ml-5">
                        <Media heading>{dish.name}</Media>
                        <p>{dish.description}</p>
                    </Media>
                </Media>
            </div>
        );
    });
```

- Essa faz a parte visual do menu, onde `dishes.map` pega pega cada prato da lista e cria uma parte visual.
Dentro da `<div>` contém as imagens, nome e descrição.

## Terceiro bloco de código 

```js
return (
        <div className="container">
            <div className="row">
                <Media list>
                    {menu}
                </Media>
            </div>
        </div>
    );
```

- Aqui o menu é mostrado na tela.

## Exportando

```js
export default Menu
```
- Usado para outras partes do app usarem o que foi criado.

```js
import Menu from 'components/MenuComponent'
```
- Onde o componente `Menu` e o arquivo `MenuComponent.js` é importado.
