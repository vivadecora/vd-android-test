# Teste Android

Este teste é destinado para a vaga de desenvolvedor android. Não se preocupe: é um teste simples e não deve tomar muito do seu tempo.

Seu objetivo é desenvolver um aplicativo em Kotlin, contemplando  os objetivos principais listados abaixo:

## Objetivos principais:
* **Objetivo 1** - Exibir uma lista de filmes 
* **Objetivo 2** - A cada n filmes, exibir uma view customizada para promover filmes
* **Objetivo 3** - Ao clicar em um item dessa lista, mostrar a tela com os detalhes do filme

Os detalhes de cada objetivo estão listados abaixo:

## Objetivo 1
Exibir uma lista de filmes consultando a api versão **3** do **themoviesdatabase**. 
* **Passo 1:** Obtenha uma key para utilizar a api neste [link](https://developers.themoviedb.org/3/getting-started/introduction)
* **Passo 2:** Obter os filmes obtidos no endpoint /discover/movie:
```https://api.themoviedb.org/3/discover/movie?api_key=<your_api_key>```
* **Passo 3:** Exibir os filmes seguindo o layout proposto abaixo:

![alt text](http://url/to/img.png)

**A listagem deve ter paginação automática (scroll infinito) e cada request deve requisitar 25 itens**

## Objetivo 2
Queremos promover a visualização dos filmes da Marvel. Para isso devemos:
* Inserir um item (custom view) na lista de filmes. Este item irá se repetir a cada "n" filmes (exemplo: 4 filmes, item promocional, 4 filmes, item promocional...)
* O intervalo "n" pode ficar definido em uma variável com o valor inicial 4. Iremos testar esta funcionalidade com valores diferentes.
* Esse item deve ser exibido seguindo o layout sugerido abaixo:
![alt text](http://url/to/img.png)

Ao clicar neste item, devemos mostrar a lista de filmes com o termo sugerido. Deve ter o layout sugerido anteriormente no objetivo 1. Para isso você deve obter os filmes neste endpoint:
```https://api.themoviedb.org/3/search/movie?query=marvel&api_key=<your_api_key>```

Aqui também é esperado o scroll infinito, e 25 itens por requisição
Utilizamos o termo marvel como sugestão. Sinta-se a vontade para promover outros filmes.

## Objetivo 3
Criar uma tela que exibe o detalhe do item. Esta tela deve seguir o layout proposto abaixo. Sinta-se a vontade para adicionar novos recursos
![alt text](http://url/to/img.png)

Esta tela será exibida quando o item da lista for clicado, seja a lista do **objetivo 1** ou do **objetivo 2**.

## Plus:
* Clean Architecture
* Testes
* Tela com estados (loading, error, success)
* Seja criativo para surpreender-nos com o que desejar

## Entrega:
Faça seu teste em um repositório *privado* no Github, Gitlab ou Bitbucket. Ao término você receberá instruções para adicionar um colaborador para avaliar seu teste
