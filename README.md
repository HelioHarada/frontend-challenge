# Frontend Challenge

Você deverá desenvolver um componente em `Vue.js` para a listagem de produtos.

Leia as instruções abaixo e fique à vontade para solicitar esclarecimentos, se necessário.

## Entrega do projeto:

O projeto deve ser entregue através do Github e se optar por criar um projeto privado, por favor, forneça a permissão de acesso para o usuário: `shoppub`.

Seu arquivo `README` deve conter a descrição sobre o design de código utilizado, além das instruções sobre como utilizar o seu componente.

## Pré-requisitos:

Para acessar o design do componente [challenge.xd](https://github.com/shoppub/frontend-challenge/blob/master/challenge.xd), você deverá instalar o programa [Adobe XD](https://www.adobe.com/br/products/xd.html).

## Instruções:

O arquivo [settings.json](https://github.com/shoppub/frontend-challenge/blob/master/settings.json) possui todas as configurações gerais da loja, incluindo as configurações de layout.

Abaixo temos a descrição de cada campo:

- **title**: Título da loja (`str`)
- **layout**: Configurações de layouts da loja
- - **product**: Configurações de layout referente aos componentes de produtos
- - - **list**: Configurações de layout de listagem dos produtos
- - - - **attribute_widget_type**: Tipo do widget de atributos dos produtos. As opções são: 1 para option e 2 para select (`int`)
- - - - **show_related_products**: Exibir os produtos relacionados (`bool`)
- - - - **show_availability_widget**: Exibir a funcionalidade de quantidade no componente para adicionar ao carrinho (`bool`)
- - - - **show_favorite_widget**: Exibir o botão de favorito (`bool`)
- - - - **show_tags**: Exibir as tags do produto (`bool`)
- - - - **show_campaign_tags**: Exibir as tags de campanha do produto (`bool`)

O arquivo [products.json](https://github.com/shoppub/frontend-challenge/blob/master/products.json) possui um exemplo do JSON de resposta da API para a listagem de produtos. Este JSON deverá ser utilizado para popular os dados no seu componente.

Abaixo temos a descrição de cada campo:

- **id**: ID único do produto (`int`)
- **title**: Título do produto (`str`)
- **images**: Imagens do produto
- - **cover**: URL para a imagem de capa (`str`)
- - **hover**: URL para a imagem de hover da imagem atual (`str`)
- - **is_highlight**: Imagem em destaque. Todo produto possui apenas uma imagem em destaque (`bool`)
- **availability**: Disponibilidade do produto
- - **is_available**: Produto disponível ou não (`bool`)
- - **quantity**: Quantidade disponível para o produto (`int`)
- **attributes**: Atributos do produto, exemplo: Tamanho, voltagem, ...
- - **id**: ID único do atributo (`int`)
- - **label**: Label do atributo (`str`)
- **tags**: Tags do produto
- - **label**: Label da tag (`str`)
- - **color**: Cor da tag no formato hexadecimal (`str`)
- **campaign_tags**: Tags de campanha do produto
- - **label**: Label da tag (`str`)
- - **color**: Cor da tag no formato hexadecimal (`str`)
- **related_products**: Produtos relacionados
- - **id**: ID único do produto relacionado (`int`)
- - **title**: Título do produto relacionado (`str`)
- - **image**: URL para a imagem do produto relacionado (`str`)
- **pricing**: Informações referentes ao valor e condições de pagamento do produto
- - **total_value**: Valor total final do produto (`float`)
- - **total_value_from**: Valor total inicial do produto (`float`)
- - - **installments**: Condições de pagamento do produto (parcelas)
- - - - **quantity**: Quantidade total de parcelas disponíveis (`int`)
- - - - **installment_value**: Valor por parcela (`float`)
- - - - **total_value**: Valor total do produto parcelado (`float`)
