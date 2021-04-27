# Aula #02 React

## Typescript

Uma das principais funções do TS é dar manutenção em código, nisso ele difere muito do JS, pois com ele conseguimos definir uma tipagem das propriedades de uma variável.
Nos ajuda tambem a não errar no projeto e termos mais segurança ao programar. 

## Dicas
- O projeto React puxa automaticamente os arquivos _app.tsx e o index.tsx e controi a interface no navegador. O que colocamos no _app.tsx é tudo o que fica "em volta" do projeto. Só não colocamos as fontes nele pois sempre que o arquivo é recarregado ele teria que recarregar as fontes novamente. Por isso criamos uma arquivo _document.tsx.
Esse arquivo _document.tsx também fica por volta do projeto todo, porém ele é carregado uma unica vez. Dentro dele importamos o HTML, Head, Main, NextScript do servidor do next.js, para contruirmos a interface conforme a documentação do next.js.

- No projeto React, tudo o que esta na pasta public pode ser acessado em qualquer arquivo sem precisar do diretório, apenas do nome do arquivo.


