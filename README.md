
#Stylus Workflow

##Stylus, Jeet e Rupture

Esse projeto foi desenvolvido para um trabalho de faculdade.
O projeto foi desenvolvido utilizando o pré-processador Stylus, o sistema de grids modular Jeet 
e o Rupture, que é uma forma mais simples de desenvolver o responsivo (media-queries).

###Instalação:

1. Tenha instalado o NodeJs (https://nodejs.org/en/)
2. Abra o Terminal/cmd e clone o projeto localmente
  * `git init`
  * `git clone https://github.com/bkullmanns/stylus-workflow.git`
  
####Prossiga no terminal com os seguintes comandos:
3. `cd stylus-workflow`
4. `npm install` ou `npm i`
5. `npm run watch` 

##Uma explicação prática e rápida de como funciona: 

O **Stylus** funciona em uma camada acima do CSS. Pré processadores foram criados pra poder desenvolver 
o CSS com algumas funcionalidades que o CSS por si só não possui. 
Mas por que eu escolhi o Stylus pra aprender sobre pré processadores?
Porque o Stylus possui 3 benefícios sobre o LESS e o SASS: 
  1. Sintaxe flexível: Você pode desenvolver tanto utilizando chaves, dois pontos e ponto e vírgula quanto sem nada disso.
  Você tem essa opção.
  2. Mais fácil de instalar e menos coisas pra ter instalado no PC
    * O Stylus utiliza o NPM apenas. Para usar o SASS precisa ter o Ruby instalado. 
  "Mas é uma coisa só, que diferença faz?" A diferença é que a maioria das outras tecnologias que você utiliza
  usa o NPM. Se não precisa instalar o Ruby pra mais nada, é só uma coisa a mais pra você instalar e ter no PC.
  3. Mais funcionalidades.

O **Jeet** é um sistema de grids extremamente simples, fácil de aprender, leve e modular, ou seja,
você faz o seu grid. Você alinha cada elemento conforme a sua necessidade.
O Jeet inicialmente foi desenvolvido como plugin apenas para o Sylus, mas hoje ele possui uma versão para SASS também.

Exemplos utilizados no projeto:
  * `stack()` = empilha os elementos em blocos, usado no responsivo.
  * `center(tamanho-em-px)` alinha o elemento ao centro com relação ao elemento pai.

O **Rupture*** é um plugin para Stylus com o intuíto de ter uma forma mais simples e divertida de criar o responsivo.
É uma sintaxe mais simples que a sintaxe das MediaQueries.

Exemplos usados no projeto:
  * `+desktop()` 
  * `+between(minimo-px, maximo-px)` equivalente a `@media only screen and (min-width: minimo-px) and (max-width: maximo-px)`
  * `+below(maximo-px)`equivalente a `@media only screend (max-width: maximo-px)``

###Instalação inicial do projeto (processo que fiz para criar o projeto)

1. Instalação do NodeJs
  * Pelo link https://nodejs.org/en/
  
2. No terminal, usar o comando `npm init`
  * Esse comando cria o arquivo `package.json`, que é responsável pela gerência das dependências (plugins - Rupture, Jeet) 
  e onde é criado o script `watch`, que compila o arquivo `.styl`.
  
3. Instalação do Stylus
  *No terminal usar o comando: `npm install stylu --save`
  O `--save` é o comando para que o NPM liste o plugin instalado nas dependências do `package.json`. 
  Por que isso é útil? Nos arquivos aqui listados não possui a pasta node_modules, onde ficam as dependências. Essa pasta, contendo 
  os plugins instalados é criada a partir das dependências listadas no arquivo `package.json`.
  pelo comando `npm i`, como instruído a fazer no início desse documento. Isso é útil para não precisar subir a pasta node_modules 
  sempre, já que é uma pasta com vários arquivos (mais pesada do projeto, nesse caso).
  
4. Instalação do Jeet
  * O comando `npm install jeet --save`
  
5. Instalação do Rupture
  * O comando `npm install rupture --save`
  
Essa é uma forma diferente, simples de aprender (e usar) e divertida de desenvolver.

Materiais consultados pra desenvolver esse projeto: 

Stylus: https://www.youtube.com/watch?v=eJahtnmywMI&list=PLLnpHn493BHFWQGA1PcyQZWAfR96a4CkH

http://schempy.com/2015/04/03/responsive_layout_with_stylus_jeet_and_rupture/

https://github.com/jenius/rupture (documentação)

http://jeet.gs/ (documentação e videos)



  






  




