# Planalto Imóveis

Landing page responsiva de imóveis à venda em Vitória da Conquista (BA), criada como projeto de demonstração de front-end. Os anúncios exibidos são reais e cada cartão leva ao anúncio original.

**Site:** https://renatabfs.github.io/imobiliaria-planalto

## Funcionalidades

- Filtros dinâmicos por tipo (casa, apartamento ou terreno), bairro e valor máximo (até R$ 1 milhão)
- Ordenação por menor preço, maior preço ou maior área
- Cartões com preço, bairro, quartos, área e a fonte do anúncio
- Botão "Ver anúncio", que abre o anúncio original em nova aba
- Formulário de contato com validação de nome e telefone
- Layout responsivo, com cabeçalho fixo e grade de cartões que se ajusta ao celular e ao computador
- Modo escuro automático, conforme a preferência do dispositivo
- Acessibilidade: navegação por teclado, rótulos nos campos, foco visível e respeito à preferência por menos animação

## Anúncios reais

Os 16 imóveis foram pesquisados em portais e imobiliárias da cidade, como ZAP Imóveis, Casa Mineira, Trovit, Chaves na Mão e Loft, com anunciantes locais como Mark Imóveis, Locar Imóvel e Marcelo Leal Imóveis.

- Dados consultados em **02/11/2026**. Preços e disponibilidade mudam a qualquer momento, então confirme sempre no anúncio original.
- Alguns cartões levam ao anúncio individual. Outros levam à página de listagem do portal onde o imóvel aparece, e o imóvel pode ter mudado de posição ou saído do ar.
- As imagens dos cartões são ilustrações, não fotos dos imóveis. As fotos pertencem aos anunciantes e podem ser vistas no anúncio original.
- O terreno da Loft informa o valor por m². O total exibido (R$ 550 mil) é um cálculo sobre esse valor.

### Como atualizar os imóveis

Os dados ficam na lista `imoveis`, no `<script>` do `index.html`. Cada item tem este formato:

```js
{t:"Casa", n:"Nome do anúncio", b:"Bairro", q:3, a:120, p:350000, f:"Fonte", u:"https://link-do-anuncio"}
```

- `t`: tipo (`Casa`, `Apartamento` ou `Terreno`)
- `n`: título do anúncio
- `b`: bairro
- `q`: número de quartos (use `0` para terreno)
- `a`: área em m²
- `p`: preço em reais
- `f`: fonte ou anunciante
- `u`: link do anúncio original
- `pm` (opcional): preço por m², exibido ao lado do valor

Os bairros do filtro são gerados automaticamente a partir dessa lista.

## Tecnologias

- HTML5
- CSS3 (variáveis, Grid, Flexbox e `prefers-color-scheme`)
- JavaScript (sem bibliotecas)
- Fontes Bricolage Grotesque e Public Sans, carregadas do Google Fonts

## Como rodar

Baixe o projeto e abra o arquivo `index.html` no navegador. Não precisa instalar nada. É preciso estar online para carregar as fontes e para abrir os links dos anúncios.

## Observação

A Planalto Imóveis é uma empresa fictícia e não representa nenhuma das imobiliárias ou portais citados. Os imóveis, valores e links pertencem aos respectivos anunciantes. O projeto serve apenas para demonstração.

## Autora

Renata Beatriz Soares
