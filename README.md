# 🍔 Mini Hamburgueria — Curso do Livro

Uma mini loja estilo apps de delivery, feita para estudos e demonstrações em aulas. O projeto simula um cardápio de hambúrgueres com filtros, carrinho, cupons de desconto e finalização do pedido via WhatsApp — tudo em HTML, CSS e JavaScript puro.

---

## ✨ Visão Geral

- Interface moderna e responsiva com paleta quente e foco nos cards.
- Cardápio dinâmico com filtros por categoria (Burgers, Combos, Bebidas, Sobremesas).
- Carrinho completo: adicionar, remover, alterar quantidades e cálculo automático.
- Cupons de exemplo para aulas (JVV10, LIVRO15, CURSODOLIVRO).
- Observações do pedido e envio do resumo diretamente para o WhatsApp.
- “Modo Professor” para adicionar produtos no front-end, ideal para demonstrar arrays/objetos e manipulação de DOM.

---

## 🧰 Tecnologias Utilizadas

- HTML5 sem framework de build.
- CSS3 com design responsivo e Google Fonts (Poppins).
- JavaScript Vanilla (manipulação de DOM, eventos e lógica do carrinho).
- Integração com API do WhatsApp para abrir a conversa com mensagem pré-formatada.

---

## 🗂️ Estrutura do Projeto

```
mini-hamburgueria-main/
├─ index.html          # Estrutura da página e marcação semântica
├─ css/
│  └─ style.css        # Estilos, tema, responsividade e componentes
├─ js/
│  └─ script.js        # Lógica do cardápio, carrinho, cupons e checkout
└─ .vscode/
   └─ settings.json    # Configurações de editor (opcional)
```

---

## 🚀 Como Executar

- Abra o arquivo `index.html` diretamente no navegador.
- Opcional: use a extensão “Live Server” no VS Code para recarregamento automático.

### Configurar o WhatsApp (opcional)

Defina o número que receberá os pedidos em `js/script.js` (com DDI + DDD, apenas dígitos):

```js
// js/script.js
var WHATSAPP_NUMBER = "5511999999999"; // Exemplo: +55 11 XXXXX-XXXX
```

---

## 🛒 Funcionalidades Principais

- 🧭 Filtros de categoria com destaque visual e renderização dinâmica.
- ➕ Adicionar itens ao carrinho a partir dos cards (botão “Adicionar”).
- 🔁 Alterar quantidade (+/−) e remover itens do carrinho.
- 💰 Cálculo de subtotal, desconto e total em tempo real.
- 🎟️ Cupons de desconto de exemplo: `JVV10` (10%), `LIVRO15` (15%), `CURSODOLIVRO` (30%).
- 📝 Campo de observações para personalizar o pedido.
- 🧹 Limpar carrinho com confirmação.
- 📲 Finalizar pedido abrindo conversa no WhatsApp com mensagem formatada.
- ⚙️ “Modo Professor” para incluir novos produtos no cardápio (apenas no front-end).

---

## 🏗️ Organização do Código

- Dados do cardápio: array de objetos com id, name, description, price, category, emoji, calories e tag.
- Estado do carrinho e cupom: estruturas em memória para itens e desconto percentual.
- Seleção de elementos do DOM: referências para grid de produtos, carrinho, botões e inputs.
- Utilitários: formatação de moeda, busca de produto e geração de id.
- Renderização do cardápio: monta cards com HTML e aplica filtros.
- Lógica do carrinho: adicionar, atualizar quantidade, remover, limpar e totalizar.
- Cupons: valida, aplica e exibe mensagens de feedback.
- Checkout via WhatsApp: compõe mensagem com itens, totais e observações; abre a conversa.
- Modo Professor: formulário para criar novos produtos e re-renderizar o cardápio.

---

## 📚 Objetivo Educacional

Este projeto é ideal para praticar:

- Manipulação de DOM e eventos.
- Organização de dados com arrays/objetos.
- Renderização dinâmica e estado em memória.
- Formatação de valores e UX de carrinho.

---

## 📄 Licença

Uso livre para fins educativos. Sinta-se à vontade para adaptar nas suas aulas ou estudos.
