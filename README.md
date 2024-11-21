## Configuração do aplicativo React

Passos realizados

1 - Na prompt de comando foi digitado os seguintes códigos:

npm install reactstrap react react-dom 
npm install --save bootstrap 
npm install react-popper @popperjs/core

2 - Em seguida, a pasta "src" que foi criada na aula-5 foi aberta no Visual Studio Code e no arquivo 'index.js' foi adicionado essa linha:

import 'bootstrap/dist/css/bootstrap.min.css'

3 - Após isso, no arquivo 'App.js' na mesma pasta "src" foi apagado a parte da header do html e adicionado esse bloco de código: 

<Navbar dark color="primary"> 
    <div className="container"> 
        <NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand> 
        <div>Aluno: Fulano de Tal</div> 
    </div> 
</Navbar>

Também foi alterado a o nome do aluno na div.
