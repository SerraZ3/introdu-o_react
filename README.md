# Introdução React

Esse material está sendo criando com intuito de facilitar o aprendizado dos membros da [Associação Empresa Junior de Computação da UESC (TecnoJr)](https://www.tecnojr.com.br/) e qualquer outro estudante da área de computação que tenha o desejo de aprender React

**Desenvolvido por:**
[Henrique A. Serra](https://github.com/SerraZ3/) :smile: :metal:

## Sumário

1. [Introdução](#introdução)
2. [Instalação](#instalação)
3. [Hello World](#hello-world)
4. [Estrutura diretório React (Em desenvolvimento)](#estrutura-diretório-react)
5. [Programando em React](#programando-em-react)

# Introdução

### O que é React

O React possui um [site oficial](https://pt-br.reactjs.org/), onde posse encontra a [documentação](https://pt-br.reactjs.org/docs/getting-started.html), [tutoriais](https://pt-br.reactjs.org/tutorial/tutorial.html), dentre outra coisas que poderão auxiliá-lo no desenvolvido de aplicativos.

React, segundo seus desenvolvedores, é um biblioteca JavaScript declarativa, eficiente e flexível para a criação de interfaces de usuário. Surgiu em 2011, pelo Facebook, e em 2013 seus códigos foram abertos ao público.

O React possui uma gama de módulos que estão disponíveis para download via npm ou outras plataformas. Os módulos auxiliam no desenvolvimento poupando tempo e trabalho.

O React possui uma versão para desenvolvimento híbrido pra mobile chamado [React-Native](https://facebook.github.io/react-native/). Ela está sendo muito utilizado por diversos aplicativos e a cada dia que passa cresce cada vez mais.

#### O que seria um JavaScript declarativo?

Uma linguagem declarativa é meio que o contrário de uma linguamge imperativa. Enquanto um linguagem imperativa foca em dar uma sequência de passos prevendo cada situação um linguagem declarativa se preocupa com o resultado final facilitando o que o programador deseja fazer.

Por exemplo, o botão de curtir do Facebook, quando clicado fica azul, quando clicado novamente fica cinza. Em uma linguagem imperativa, usando JavaScript, ficaria algo desse tipo:

```
if( usuario.curtiu() ) {
  if( botaoEstaAzul() ) {
      removeAzul();
      adicionaCinza();
  } else {
      removeCinza();
      adicionaAzul();
  }
}
```
Em um linguagem declarativa, usando React, ficaria algo assim:

```
if( this.state.curtido ) {
  return <curtidaAzul />;
} else {
  return <curtidaCinza />;
}
```

#### Por que uma biblioteca e não framework?

Bem, como de costume um framework é feito com seu padrão de projeto e não permite que o programador saia dessa padrão. Ele limita o programador ao que ele fornece, ele que dita o que deve ser feito.

A biblioteca possibilita, de forma flexivel e menos complexa, que o programador programe da melhor forma que achar.

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

Ele irá criar uma pasta padrão do React com todas suas configurações e arquivos base.

Para rodar o React basta entrar na pasta do seu nome_projeto:

```
cd nome_projeto
```

Em seguinda dar o seguinte comando:

```
npm start
```

Ele irá abrir o projeto por padrão no _localhost:3000/_. Caso precise instalar alguma dependencia dê o comando a seguir antes do comando anterior

```
npm install
```


## Programando em React

Primeiramente deve-se ter em mente que a estrutura utilizada pelo React é a do JSX. Ela é uma sintaxe semelhante ao XML, na qual você consegue escrever e compreender de uma forma melhor como será montado o seu component na UI (User Interface).

Utiliza-se componentes JSX para organizar a UI e o js para realizar a parte lógica. Exemplo de componente JSX:

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

Em um componente JSX sempre deve existir um componente que irá englobar os demais. No exemplo acima o <nav> engloba os demais. Se o código não possuisse um componente que englobasse os demais ele iria gerar erro. Exemplo de erro:

```
<h1>Exemplo de erro</h1>
<ul>
  <li>Não</li>
  <li>Faça</li>
  <li>Isso</li>
</ul>
```
