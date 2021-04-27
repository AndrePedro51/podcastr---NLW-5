# Aula #01 React

Antigamente os app web eram desenvolvidos de forma que o back-end retornasse o código html inteiro para o browser, sobrecarregando assim o carregamento da pagina e a busca no servidor, além disso vieram o mobile, que não entendia o html retornado do servidor. Para resolver esses problemas foi criado o SSR.

## SSR
Server-side redering. Nesse formato ao invés do servidor montar o html, isso ficou por conta do browser, a unica coisa que o servidor retorna é um JSON, que é entendido em qualquer dispositivo.

## SSG
Static Site Generator. Normalmente para você acessar um site, você sempre faz uma requisição para o back-end retornar os dados solicitados. Em um site que têm muitas visitar por dia isso não é performático, gerando assim uma sobrecarga no servidor. Com o SSR isso mudou, pois nesse sistema você não faz a requisição direto no servidor e sim no Next.js. Esse por sua vez disponibiliza o mesmo código para todos sempre que algue fizer essa requisição, não fazendo a busca no back-end, por isso é estática. A atualização do back-end será feita apenas no momento em que programarmos o Next.js para atualizar, podendo ser uma vez ao dia, a cada 6 horas, etc.

## SPA
O SPA significa Single Page Application. A principal funcionalidade e vantegem desse tipo de aplicação é você alterar os dados visualizados no app sem precisar carregar todo o conteudo, ou seja, uma aplicação de uma única página.


## Ferramentas necessárias para construir um app em React
- Node.js
- Yarn

## Comandos úteis
- npx create-react-app [nome do arquivo] // criar um app em React.
- npx create-next-app [nome do arquivo] // criar um app em Next.js.
- code. //comando para abrir o VS Code no aquivo.
- yarn start // inicia a visualização do projeto
- yarn add typescript @types/react @types/node -D // instalar os pacotes do typescript
- yarn add date-fns // instalar o frameworks date fns que formata as datas de muitas formas possíveis
- yarn add json-server -D // instala uma fake API para podermos usar os dados de um "back-end" falso.
- yarn add axios // instala um framework para fazer requisições HTTP

## Diferença entre React e React com Next
- React
    O React sozinho reproduz os arquivos de interface em JS, fazendo uma requisição para o back-end da aplicação e retornando os dados em JSON. Todo esse procedimento so é efetivado depois que alguém entra na nossa página e faz essa requisição, antes disso nossa página fica "em branco". Desse modo os algoritimos de busca do Google ou de qualquer outro site não encontra a página. É nisso que o Next.js nos ajuda.
- Next.js
    O Next.js veio para resolver esses problemas no React. Ele usa o modelo de SSR porém ao invés de ser carregado quando alguém entre na aplicação e faz a requisição ele ja faz isso automaticamente, respondendo para o browser o codigo HTML.
### Exemplo de como funciona o SSR com o Next.js

![NLW](https://i.imgur.com/49IFcZf.png)