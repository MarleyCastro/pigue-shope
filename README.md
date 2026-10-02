# Pingue Shop

Protótipo interativo de um aplicativo mobile de compra e venda de produtos, com design minimalista nas cores azul e amarelo. O projeto nasceu de um esboço feito à mão e foi transformado em um fluxo de telas navegável.

> Este repositório contém o **protótipo de interface** (HTML, CSS e JavaScript puros). Ele não tem back-end: os produtos, o saldo e as métricas são dados de exemplo.

## Funcionalidades

- Splash screen com a logo e redirecionamento automático após 2 segundos
- Home com grade de produtos
- Menu em overlay com as opções **Vender**, **Comprar** e **STATUS**
- Formulário de venda com foto, nome e preço
- Galeria para simular a seleção de imagens do celular
- Tela de detalhe do produto com botão **Comprar**
- Tela de confirmação: "Produto Confirmado com Sucesso!!"
- Painel de status do vendedor: produtos anunciados, vendas e saldo
- Transições suaves entre telas (deslize lateral, sheet animado no menu)
- Respeita `prefers-reduced-motion`

## Fluxo de navegação

```
Splash (2s)
   └─► Home (grade de produtos)
          ├─► Menu ─┬─► Vender ─► Galeria ─► (volta ao formulário) ─► OK ─► Confirmação
          │         ├─► Comprar ─► Home
          │         └─► STATUS
          └─► Produto ─► Comprar ─► Confirmação
```

## Design

| Elemento      | Valor                         |
| ------------- | ----------------------------- |
| Azul primário | `#0D47A1`                     |
| Amarelo       | `#FFC107`                     |
| Fonte         | Outfit (Google Fonts)         |
| Estilo        | Minimalista, limpo, cantos arredondados |

## Tecnologias

- HTML5
- CSS3 (variáveis, transições e animações)
- JavaScript (sem frameworks e sem dependências)

## Como executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU-USUARIO/pingue-shop.git
   cd pingue-shop
   ```
2. Abra o arquivo `index.html` no navegador. Não precisa instalar nada.

Para ver como no celular, abra o DevTools do navegador e ative o modo de dispositivo móvel.

## Estrutura

```
pingue-shop/
├── index.html   # Telas, estilos e lógica de navegação
└── README.md
```

## Próximos passos

- [ ] Migrar o protótipo para Flutter ou React Native
- [ ] Cadastro e login de usuários
- [ ] Back-end com API para produtos, vendas e saldo
- [ ] Upload real de fotos
- [ ] Busca e filtros por categoria

## Autor

**Marley Castro Nascimento**

## Licença

Defina a licença do projeto (por exemplo, MIT) e adicione o arquivo `LICENSE`.
