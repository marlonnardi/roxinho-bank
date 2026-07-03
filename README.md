# Roxinho Bank

App mobile de banco digital em um unico arquivo HTML autocontido, inspirado na experiencia de bancos digitais brasileiros.

## Como abrir

Abra `index.html` diretamente no navegador.

## O que esta incluido

- Moldura de celular 390x844 para demonstracao mobile.
- Home com saldo, acoes rapidas e resumo de cartao.
- Fluxo Pix funcional com validacao de CPF, e-mail e telefone.
- Teclado numerico customizado com formatacao em reais.
- Confirmacao, sucesso animado e comprovante Pix.
- Extrato com busca em tempo real e transacoes agrupadas por data.
- Cartao virtual com flip, bloqueio visual e progresso de fatura.

## Prompt utilizado

```text
Construa um app de banco mobile totalmente funcional, inspirado nos bancos digitais brasileiros, chamado "Roxinho Bank", como um ÚNICO arquivo HTML autocontido (CSS/JS inline, sem frameworks).

APRESENTAÇÃO:
- Renderize dentro de uma moldura de celular centralizada (390x844) com fundo escuro ao redor, para parecer uma demo em dispositivo.
- Linguagem visual: roxo profundo como cor primária (família #820AD1), cards brancos, cantos arredondados, ícones nítidos desenhados em SVG inline (nada de ícones em emoji), transições de tela suaves a 60fps (slide/fade).

O APP PRECISA SER UM PRODUTO REAL FUNCIONANDO, não um mockup estático. Estado apenas em memória (sem localStorage). Popule com dados realistas: saldo de R$ 3.847,52 e 15 transações passadas com nomes de estabelecimentos brasileiros (iFood, Uber, Mercado Livre, Padaria São José, etc), datas e valores.

TELAS E FLUXOS (tudo em português do Brasil, tudo navegável):
1. HOME: saudação com nome do usuário, saldo com ícone de olho para ocultar/mostrar (exibe •••• quando oculto), linha horizontal de ações rápidas (Pix, Pagar, Transferir, Recarga), resumo do cartão de crédito com fatura atual, seção de atalhos.
2. FLUXO PIX (o teste central):
   a. Escolher "Enviar" > digitar uma chave Pix (validar 3 formatos: CPF com máscara 000.000.000-00, email e telefone)
   b. Digitar o valor com um teclado numérico customizado renderizado na interface, formatação em reais enquanto digita (R$ 0,00)
   c. Tela de confirmação mostrando destinatário, valor e data
   d. Tela de sucesso animada com animação de check e um "Comprovante" que pode ser aberto, mostrando ID da transação e horário
   e. O saldo PRECISA diminuir e a transação PRECISA aparecer no topo do extrato imediatamente.
   f. Bloquear envio acima do saldo disponível com um estado de erro bem feito.
3. EXTRATO: lista completa de transações agrupadas por data, cada uma com ícone SVG por categoria, campo de busca que filtra em tempo real, valores de entrada em verde com "+".
4. TELA DO CARTÃO: frente do cartão virtual com número oculto por padrão, toque para revelar com animação de flip, toggle "Bloquear cartão" que congela o cartão visualmente (escala de cinza + ícone de cadeado), barra de progresso da fatura em relação ao limite.
5. NAVEGAÇÃO INFERIOR: tab bar persistente (Início, Extrato, Cartão) com estados ativos.

DETALHES QUE SERÃO JULGADOS:
- Formatação correta de reais em todo lugar (R$ 1.234,56).
- Microcopy realista em PT-BR, sem texto de placeholder.
- Todo botão visível na tela precisa fazer algo (ou mostrar um toast elegante de "em breve").
- Skeletons de carregamento ou spinners nas transições, para parecer um app fintech de verdade.
```

## Comparativos

![Captura do projeto](comparativos/Captura%20de%20tela%202026-07-03%20122622.png)

![Captura mobile do app](comparativos/Captura%20de%20tela%202026-07-03%20123635.png)
