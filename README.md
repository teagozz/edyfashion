# Edy Fashion - Vitrine Virtual 👗

Este é um projeto de **Front-end** que desenvolvi para simular uma vitrine virtual moderna e focada em conversão. O objetivo principal foi criar uma experiência de e-commerce sem a complexidade de um gateway de pagamento: o cliente escolhe os produtos, monta o carrinho e o pedido é formatado automaticamente para ser finalizado no **WhatsApp** da loja.


## 💡 A Ideia

Muitas lojas locais preferem fechar vendas pelo WhatsApp para manter um contato próximo com o cliente e evitar taxas abusivas de plataformas. Criei esse sistema para automatizar aquela parte chata de "tirar print" do que quer comprar. O site gera uma lista organizada do pedido e envia pronta para o vendedor.

## 🛠️ Tecnologias Utilizadas

Como o foco era agilidade e performance no navegador, utilizei:

  * **HTML5** (Semântico)
  * **Tailwind CSS** (Via CDN para estilização rápida e responsiva)
  * **JavaScript (Vanilla)** (Toda a lógica de carrinho, modais e manipulação de DOM)

## 🚀 Funcionalidades

  * **Vitrine Dinâmica:** Listagem de produtos separados por categorias com navegação em abas.
  * **Sistema de Carrinho:** Adição e remoção de itens em tempo real (estado local).
  * **Lógica de WhatsApp Inteligente:**
      * Se o cliente comprar 1 item, a mensagem sai no singular.
      * Se comprar vários, o JS monta uma lista numerada com IDs e Nomes.
  * **Modais Interativos:** Para login (simulado), detalhes do produto e visualização do carrinho.
  * **Design Responsivo:** Funciona bem no celular e no desktop.
  * **Área Legal:** Estrutura pronta para LGPD, Termos de Uso e Políticas de Troca.

## 🧠 Desafios e Aprendizados

Um dos pontos mais legais foi fazer a lógica de montagem da URL do WhatsApp (`finalizePurchaseWhatsApp`), pois tive que garantir que o JavaScript percorresse o array do carrinho, somasse o total e formatasse a string (`encodeURIComponent`) para que a mensagem chegasse bonitinha no celular do vendedor, com quebras de linha e formatação correta.

Também trabalhei bastante com manipulação de classes do Tailwind via JS para fazer as animações de entrada dos modais e a troca de abas das categorias.



## Agora: 
  📂 Como rodar o projeto

Como o projeto é estático, não depende de build no Node.js (por enquanto), é bem simples:

1.  Clone este repositório.
2.  Garanta que as imagens (logo.jpg, p1.jpg, etc) estejam na mesma pasta para carregar corretamente.
3.  Abra o arquivo `index.html` em qualquer navegador.



## **🔜 Meus próximos passos**

  * Integrar com um Back-end (Java/Spring Boot) que estou estudando.
  * Salvar o carrinho no `localStorage` para não perder os itens ao atualizar a página.
  * Criar um painel administrativo para cadastrar produtos sem mexer no código.


Feito utilizando muito ☕ e código por **[Thiago Dias Jardim](https://www.linkedin.com/in/thiagodjardim/)**.
