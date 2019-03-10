# Introdução React

Essa material está sendo criando com intuito de facilitar o aprendizado dos membros da [Associação Empresa Junior de Computação da UESC (TecnoJr)](https://www.tecnojr.com.br/) e qualquer outro estudante da área de computação que tenha o desejo de aprender React

**Desenvolvido por:**
[Henrique A. Serra](https://github.com/SerraZ3/) :smile: :metal:

## Sumário

1. [Introdução (Em desenvolvimento)](#introdução)
2. [Instalação](#instalação)
3. [Hello World](#hello-world)
4. [Estrutura diretório React (Em desenvolvimento)](#estrutura-diretório-react)
5. [Programando em React](#programando-em-react)


## Instalação

### Instalando o NodeJs e npm

Para instalar o React é preciso instalar primeiro o NodeJs juntamente com o NPM (Node Package Manager - Gerenciador de Pacote Node), pois o React utiliza o NodeJs para rodar suas configurações.

Para instalar o NodeJs basta ir no site do [NodeJs](https://nodejs.org/) e baixar sua última versão LTS. Quando baixar o NodeJs o npm irá instalar automáticamente.

Verifique se o NodeJs e o npm foram instalador com os seguintes comandos:
```
node -v
```
```
npm -v
```

### Instalando React

Após realizar o passo anterior, basta abrir o terminal e instalar globalmente o creador de aplicativos React com o seguinte comando:
```
npm install -g create-react-app
```

## Hello World

Após realizar a etapa anterior, deve abrir o terminal e digitar o seguinte comando:

```
create-react-app nome_projeto
```

Nele irá criar uma pasta padrão do React com todas suas configurações base.

Para rodar o react basta entrar na pasta do seu nome_projeto

```
cd nome_projeto
```

Em seguinda da o seguinte comando:

```
npm start
```

Ele irá abrir o projeto por padrão no ~localhost:3000/~. Caso precise instalar alguma dependencia dê o comando a seguir antes do comando anterior

```
npm install
```


## Programando em React

Primeiramente deve-se ter em mente que a estrutura utilizada pelo React é a do JSX. Ela é uma sintaxe semelhante ao XML, na qual você consegue escrever e compreender de uma forma melhor como será montado o seu component na UI (User Interface).

Utiliza-se componentes JSX para organizar a UI e o js para realizar a parte lógica. Por exemplo:

```
const nav = (
  <nav>
    <ul>
      <li>
        <a href="#">Home</a>
      </li>
      <li>
        <a href="#">About</a>
      </li>
    </ul>
  </nav>
)
```

Nesse código é cria uma contante que recebe um componente JSX. Em um componente JSX sempre deve existir um componente que irá englobar os demais. No exemplo a cima o <nav> engloba os demais. Se o código não possuisse um componente que englobasse os demais iria gerar erro. Exemplo de erro:

```
<h1>Exemplo de erro</h1>
<ul>
  <li>Não</li>
  <li>Faça</li>
  <li>Isso</li>
</ul>
```
