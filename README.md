## 🎬 VidFlow 🎬

Este projeto é um clone da interface do YouTube, construído com HTML, CSS e JavaScript, com um back-end que fornece dados de vídeos. 

## 💻 Tecnologias Utilizadas:

- HTML
- CSS
- JavaScript

## 📂 Arquitetura do Projeto

### 📁 backend/

Contém os dados dos vídeos.

- `videos.json`: Provavelmente um arquivo JSON contendo informações sobre os vídeos exibidos na interface.

### 📁 css/

Estilos CSS da aplicação.

- `estilos.css`:  Estilos gerais da aplicação.
- `flexbox.css`: Estilos específicos para o layout com Flexbox.
- `reset.css`: Arquivo de reset de estilos para garantir consistência entre navegadores.

### 📁 img/

Imagens utilizadas na interface.

- `arrow_forward_ios.png`: Imagem de seta para navegação.
- `Favicon.png`: Ícone (favicon) do site.
- `sidebar/`: Imagens utilizadas na barra lateral.
  - Diversos ícones representando seções do YouTube como "Início", "Explorar", "Inscrições", etc.
- `topbar/`: Imagens da barra superior.
  - Ícones de "Apps", "Notificações", "Pesquisa", etc.
- `videos/`: Imagens relacionadas aos vídeos. 
  - `Ellipse 11.png`:  Possivelmente um placeholder para miniaturas de vídeo. 
- `VidFlow--Logo-light-mode.png`: Logo do projeto em modo claro.

### 📄 Arquivos da raiz

- `.git/`: Diretório do sistema de controle de versão Git.
- `.gitattributes`: Define atributos para arquivos no Git.
- `index.html`: Arquivo principal da interface, estrutura em HTML.
- `LICENSE`: Licença do projeto (especifica os termos de uso).
- `package-lock.json`, `package.json` 📦: Gerenciamento de dependências (npm).
- `README.md` 📄: Este arquivo, a documentação do projeto.
- `script.js`:  Lógica da aplicação, escrita em JavaScript. 


## Descrição do Projeto

Este projeto está presente no curso "JavaScript: consumindo e tratando dados de uma API" da plataforma alura

### Desenvolvimento

De começo foi disponibilizado um figma com o modelo final esperado e os modelos CSS prontos, durante o curso foi desenvolvido a estrutura HTML e JS em que se tem uma navegação e uma aba lateral e uma amostragem dos videos presentes no backend

### Funcionalidades

Com o consumo da API com o uso de responses o site é capaz de mostrar os iframes dos videos, junto com o icone do canal e o titulo do video, na barra de pesquisa é possivel pesquisar pelo video e nos botões de categoria os videos são filtrados

## Como usar

Como a API utilizada é uma API Fake feita localmente na maquina é necessário a instalação de nodeJS e a utilização dos seguintes comandos

### Instalação do JSON Server
``` bash
npm install -g json-server@0.17.4
```

### Criação do Servidor JSON
``` bash
json-server --watch backend/videos.json
```

O endereço retornado como padrão será *http://localhost:3000/videos*, em caso de um outro endereço o mesmo deve ser alterado no carquivo script.js 

```javascript
const busca = await fetch('endereço__retornado')
```
