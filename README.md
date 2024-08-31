# ADS_Senac_PTI_WebStandards

# Nutricionista Landing Page

Este repositório contém o código-fonte de uma landing page para uma nutricionista. O projeto foi desenvolvido utilizando apenas HTML e CSS.

## Estrutura do Projeto

O projeto é organizado da seguinte forma:

├── public/ 
│   ├── assets/
│   │   ├── images/ 
│   │   │   ├── about-img.png
│   │   │   ├── header-img.png
│   │   │   ├── health-img.png
│   ├── css/ 
│   │   ├── fonts.css 
│   │   ├── global.css 
│
├── src/ 
│   ├── components/ 
│   ├── pages/  
│   │   ├── home/ 
│   │   │   ├── index.html 
│   │   │   ├── index.css 
│
├── netlify.toml
├── README.md

- **public/css**: Contém os arquivos CSS globais e de fontes.
- **src/pages/home**: Contém a página principal (`index.html`) e seu respectivo arquivo CSS (`index.css`).

## Deploy

O projeto está hospedado no [Netlify](https://pti-web-standards-guilherme-muller.netlify.app). Para fazer o deploy do projeto, o Netlify está configurado para considerar a raiz do projeto como o diretório de publicação, mas redireciona a página inicial para `src/pages/home/index.html`.

### Configuração do Netlify

No arquivo `netlify.toml`, a configuração para o deploy é:

```toml
[build]
  publish = "/"

[[redirects]]
  from = "/"
  to = "/src/pages/home/index.html"
  status = 200