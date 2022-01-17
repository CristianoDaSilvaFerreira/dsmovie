<div align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/CristianoDaSilvaFerreira/dsmovie?style=for-the-badge" height="24"> 
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/CristianoDaSilvaFerreira/dsmovie?style=for-the-badge" height="24"> 
  <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" height="24">
  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/CristianoDasilvaFerreira/dsmovie?style=for-the-badge" height="24"> 
  <img alt="GitHub release (latest by date including pre-releases" src="https://img.shields.io/github/v/release/CristianoDaSilvaFerreira/dsmovie?include_prereleases&style=for-the-badge" height="24"> 
  <br/>
  <img alt="Badges TypeScript" src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" height="24"> 
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" height="24"> 
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" height="24"> 
  <img alt="React.JS" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" height="24"> 
</div>


# ![DevSuperior logo](https://raw.githubusercontent.com/devsuperior/bds-assets/main/ds/devsuperior-logo-small.png) Semana Spring React - treinamento gratuito
*Crie um app inédito para seu portfólio com as tecnologias mais demandadas do mercado*

# DSMovie

![01](https://user-images.githubusercontent.com/68359459/149702464-bb109ee8-73d6-4e1f-966a-3086ac27823d.png)

![02](https://user-images.githubusercontent.com/68359459/149702495-36fddc29-f0a5-41be-be64-783db255fa90.png)

## Realização
[DevSuperior - Escola de programação](https://devsuperior.com.br)

## Objetivos do projeto para esta aula
- Criar projetos backend e frontend
- Salvar os projeto no Github em monorepo
- Montar o visual estático do front end

## Checklist

### Passo: preparação

#### Dica: extensões do VS Code

#### Conferir Node (16 LTS) e Yarn

[Guia de instalação das ferramentas](https://github.com/devsuperior/sds-dsmovie/tree/main/_instalacao)

```bash
node -v
yarn -v
```
Caso precise instalar o Yarn, faça o comando:

```
npm install --global yarn
```

#### Design Figma
*Caso um dos links esteja cheio foi colocando outros para acesso*

[design link 1](https://www.figma.com/file/hpQuzpGHq2MmrI87xnfMoT/DSMovie1)

[design link 2](https://www.figma.com/file/svCMhNqgpAZuN86w9IHJ4v/DSMovie2)

[design link 3](https://www.figma.com/file/gEZYKqJJs2gEhIB6k9ksGB/DSMovie3)

[design link 4](https://www.figma.com/file/hyovBMIxwrn2Bb5MZLrxHL/DSMovie4)

### Passo: criar projeto ReactJS

- ATENÇÃO: esta será a estrutura de pastas que vamos criar:

![DevSuperior no Instagram](https://raw.githubusercontent.com/devsuperior/bds-assets/main/sds/pastas-dsmovie.png)

```
yarn create react-app frontend --template typescript
```
OU:
```
npx create-react-app frontend --template typescript
```

IMPORTANTE: deletar subpasta .git
- *Lembrete: ver extensões e arquivos ocultos*

### Passo: criar projeto Spring Boot

- Criar projeto Spring Boot no `Spring Initializr` com as seguintes dependências:
  - Web
  - JPA
  - H2
  - Postgres
  - Security

- Ajuste no arquivo pom.xml:

```xml
<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version>
</plugin>
```

  - Botão direito no projeto -> Maven -> Update project (force update)
  
  ### Passo: "limpar" o projeto ReactJS

- Deletar arquivos não usados
  
  
  ### Passo: adicionar Bootstrap e CSS ao projeto
- Bootstrap
```
yarn add bootstrap@5.1.3
```


 ### Passo: Componente Navbar

ATENÇÃO: no arquivo tsconfig.json: `"baseUrl": "./src"` (reinicie o app)

- Instalar React Router DOM

```
yarn add react-router-dom@6.2.1 @types/react-router-dom@5.3.2
```
