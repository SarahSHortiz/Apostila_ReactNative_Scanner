
# Componentes Básicos do React Native


### View

o View dentro da estrutura do React Native exibe o conteúdo que está inserido ente sua tag. 

Quando comparamos seu uso, podemos dizer que ele opera semelhante a uma <**div**>, porém sua sintaxe é `<View><\View>`.Embora a tag seja escrita no corpo do código e necessário fazer sua importação. 

O View opera quase como um body também, pois todos os elementos para serem exibidos devem estar contidos nele.


import { View } from 'react.....';


import { Button } from 'react.....';


Function MinhaPrimeiraTela(){

  return(

     <View>

         <Button>

            Clique aqui!

         <\Button>

     </View>

  )

}



### Onde minhas importações ficam?

As importações quaisquer que sejam devem ficar alocadas na parte superior de seu código, e por quê?

A resposta é muito simples, para melhor organização e rapidez na visualização das tags importadas necessárias para formar seu projeto. Além de que, a estrutura da linguagem bem como de outras que necessitam de importações (quase todas) utilizam, já que estas importações estão relacionadas às bibliotecas necessárias para o desenvolvimento do seu projeto. 

por exemplo: 

`import { Button } from "react...";`

Esta importação puxa de uma biblioteca que precisa ser baixada ou que já é baixada através do NODE_MODULES com os componentes desejados. No caso queremos um botão, então o importamos, e escrevemos no nosso código a tag que pedimos.

`<Button>`

Outro exemplo de importações é a linguagem C com o #include <studio.h>.

### Text 

A tag Text atua como um **<p>** ou **<h1>** etc, no HTML convencional, atribuindo textos em seu código. A tag também necessita de importação e precisa obrigatoriamente estar dentro do componente pai, ou seja a <**View**>. 


import { Text } from "react.....";


import { View } from 'react.....';


import { Button } from 'react.....';


Function MinhaPrimeiraTela(){

  return(

     <View>

         <Text>

          Olá 👋 eu sou a Sarah e esse é meu primeiro          texto no meu código!

         <\Text>

         <Button>

            Clique aqui!

         <\Button>

     </View>

  )

}


### Image 


### StyleSheet Estilização em CSS e Estilização de Componentes


## O que são Props ou Propriedades? 

## O que é States? 

### Tipos de States

## Navegação em React Native






Navegação entre telas
Uso de Stack Navigator, Drawer Navigator, Tab Navigator
Gestos e Animações

Gestos de toque e arraste
Animações básicas e avançadas
Consumo de APIs

## Requisições HTTP com Fetch ou Axios
Manipulação de dados JSON
Persistência de Dados

Uso de AsyncStorage para armazenamento local
Integração com bancos de dados SQLite
Publicação de Aplicativos

## Preparação de aplicativos para publicação na App Store e Google Play Store
Gerenciamento de versões e lançamentos de aplicativos
Boas Práticas e Dicas de Desenvolvimento

## Organização de código
Melhores práticas de design de interfaces
Debugging e resolução de problemas comuns
