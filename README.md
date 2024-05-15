# **Desafio Dio - Criando uma Homepage com React**



Projeto Completo para criar uma homepage com React usando TypeScript:

## Pré-Requisitos

Para este projeto, você precisará dos seguintes pré-requisitos:

- NodeJS 14 ou superior
- NPM 6 ou superior
- Typescript 4 ou superior
- React 17 ou superior
- Create React App



## Criar um Novo Projeto React

O primeiro passo é criar um novo projeto React. Para isso, você pode usar o Create React App:



```plaintext
npx create-react-app my-homepage
```

Este comando irá criar um novo diretório chamado `my-homepage` e instalar as dependências necessárias para o React.



## Configurar o TypeScript

Agora, você precisa configurar o TypeScript no seu projeto. Para isso, abra o arquivo `tsconfig.json` e adicione as seguintes linhas:

json



```json
{
  "compilerOptions": {
    "target": "es2017",
    "lib": ["dom", "es6"],
    "allowJs": true,
    "strict": true,
    "noImplicitAny": true,
    "strictNullChecks": true,
    "forceConsistentCasingInFileNames": true,
    "noUnusedLocals": true,
    "noUnusedParameters": true,
    "noImplicitReturns": true,
    "noFallthroughCasesInSwitch": true
  }
}
```

Estas linhas irão definir as opções de compilação do TypeScript para o seu projeto.



## Criar os Componentes

Agora, você pode começar a criar os componentes da sua homepage. Para isso, crie um novo arquivo chamado `App.tsx` e adicione o seguinte código:



```typescript
import React from "react";
import ReactDOM from "react-dom";

const App = () => {
  return (
    <div>
      <h1>Esta é a minha homepage</h1>
    </div>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));
```

Este código irá renderizar um simples componente `App` com uma `h1` que diz "Esta é a minha homepage".



## Criar a Rota Principal

Agora, você precisa criar a rota principal para a sua homepage. Para isso, abra o arquivo `App.tsx` e adicione o seguinte código:



```typescript
import React from "react";
import ReactDOM from "react-dom";
import { BrowserRouter, Route } from "react-router-dom";

const App = () => {
  return (
    <BrowserRouter>
      <Route path="/" component={App} />
    </BrowserRouter>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));
```

Este código irá criar uma rota principal para a página `App.tsx`.



## Executar o Projeto

Agora, você pode executar o seu projeto usando o seguinte comando:

```plaintext
npm start
```

Este comando irá iniciar o servidor de desenvolvimento do Create React App e você poderá visualizar a sua homepage no navegador.



## Conclusão

Este é apenas um projeto simples para criar uma homepage com React usando TypeScript. Você pode adicionar mais componentes e funcionalidades ao seu projeto conforme necessário.





## **OBSERVAÇÃO:**



### \# Primeiros passos com o aplicativo Create React

###### (Getting Started with Create React App)



#### npm start

Executa o aplicativo no modo de desenvolvimento.\
Abra [http://localhost:3000](http://localhost:3000) para visualizá-lo no navegador.

A página será recarregada se você fizer edições.\
Você também verá erros de lint no console.



### `npm test`

Inicia o executor de testes no modo de observação interativo.\
Consulte a seção sobre [execução de testes](https://facebook.github.io/create-react-app/docs/running-tests) para obter mais informações.



### `npm run build`

Cria o aplicativo para produção na pasta `build`.\
Ele agrupa corretamente o React no modo de produção e otimiza a construção para obter o melhor desempenho.

A compilação é reduzida e os nomes dos arquivos incluem os hashes.\
Seu aplicativo está pronto para ser implantado!

Consulte a seção sobre [implantação](https://facebook.github.io/create-react-app/docs/deployment) para obter mais informações.



### `npm run eject`

**Observação: esta é uma operação unidirecional. Depois de `ejetar`, você não pode voltar!**

Se você não estiver satisfeito com a ferramenta de construção e as opções de configuração, você pode `ejetar` a qualquer momento. Este comando removerá a dependência de compilação única do seu projeto.

Em vez disso, ele copiará todos os arquivos de configuração e as dependências transitivas (webpack, Babel, ESLint, etc) diretamente no seu projeto para que você tenha controle total sobre eles. Todos os comandos, exceto `eject`, ainda funcionarão, mas apontarão para os scripts copiados para que você possa ajustá-los. Neste ponto você está sozinho.

Você nunca precisa usar `ejetar`. O conjunto de recursos selecionados é adequado para implantações pequenas e médias e você não deve se sentir obrigado a usar esse recurso. No entanto, entendemos que esta ferramenta não seria útil se você não pudesse personalizá-la quando estiver pronto para isso.



## Saiba mais:

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
