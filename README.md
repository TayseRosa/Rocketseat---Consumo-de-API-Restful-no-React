<h1 align="center">Ignite - Trilha ReactNative - Chapter II </h1>

# Índice
- [Índice](#índice)
- [🛠 Projeto Rocketseat Ignite - Trilha React Native - goFinance](#-projeto-rocketseat-ignite---trilha-react-native---gofinance)
  - [Iniciando o projeto](#iniciando-o-projeto)
- [🚀 Tecnologias utilizadas neste projeto](#-tecnologias-utilizadas-neste-projeto)
- [📥 Como usar](#-como-usar)
- [🚀 Developer](#-developer)
- [📞 Contate a Dev](#-contate-a-dev)
  
---
# 🛠 Projeto Rocketseat Ignite - Trilha React Native - goFinance

<img src="" width="100%" height="auto" />

## Iniciando o projeto

- [x] npm create vite@latest
- [x] npm install
- [x] cd [nomeProjeto]
- [x] Deixar apenas os arquivos dentro da pasta src:
  - [x] src/App.tsx
  - [x] src/main.tsx
  - [x] src/vite-env.d.ts

- [x] No arquivo src/App.tsx (maneira BÁSICA de fazer o consumo de API):

```
import { useEffect, useState } from "react"

type Repository = {
  full_name: string;
  description: string;
}

function App() {

  const [ repositories, setRepositories ] = useState<Repository[]>([])

  useEffect(()=>{
    fetch('https://api.github.com/users/tayserosa/repos')
    .then(response => response.json())
    .then(data => {
      setRepositories(data);
    })
  })

  return (
    <ul>
      {repositories.map(repo => {
        return(
          <li key={repo.full_name}>
            <strong> { repo.full_name } </strong>
            <p>{ repo.description } </p>
          </li>
        )
      })}
    </ul>
  )
}

export default App
 ```




# 🚀 Tecnologias utilizadas neste projeto
O projeto foi desenvolvido utilizando as seguintes tecnologias:

- [x] JAVASCRIPT
- [x] REACT JS
- [x] TYPESCRIPT

# 📥 Como usar
```js

    //Clonar o repositório
    $ git clone 

    //Entrar no diretório
    $ cd 

    //Instalar dependências
    $ yarn install 

    //Startar o projeto
    $ expo start
    

``` 

# 🚀 Developer

<a href="https://www.tayserosa.dev">
 <img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/u/31596454?v=4" width="100px;" alt="Tayse Rosa" style="border-radius:50%"/>
 <br />
 <sub><b>Tayse Rosa</b></sub></a> <a href="https://www.tayserosa.dev" title="Tayse Rosa">🚀</a>


Feito com ❤️ por Tayse Rosa 🚀

<hr />

# 📞 Contate a Dev

👋🏽 Entre em contato!


<a href="https://www.linkedin.com/in/tayse-rosa-3b683151/" target="_blank">
<img src="https://img.shields.io/static/v1?label=LinkedIn&message=Tayse Rosa&color=blue&style=for-the-badge&logo=linkedin"/>
</a>
<br/>
<br/>

<a href="https://github.com/TayseRosa/" target="_blank">
<img src="https://img.shields.io/static/v1?label=GitHub&message=Tayse Rosa&color=black&style=for-the-badge&logo=github"/>
</a>
<br/>
<br/>

<a href="https://api.whatsapp.com/send?phone=5551982368077" target="_blank">
<img src="https://img.shields.io/static/v1?label=whatsapp&message=Tayse Rosa&color=green&style=for-the-badge&logo=whatsapp"/>
</a>
<br/>
<br/>


<a href="https://www.tayserosa.dev" target="_blank">
<img src="https://img.shields.io/static/v1?label=Portfólio&message=Tayse Rosa&color=pink&style=for-the-badge&logo=portfolio"/>
</a>
<br/>
<br/>

<h5> Créditos: Rocketseat </h5>
