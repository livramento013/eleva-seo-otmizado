# Eleva Digital | Landing Page de Alta Performance 🚀

Bem-vindo ao repositório da infraestrutura front-end da **Eleva Digital**. Esta landing page foi projetada com foco absoluto em conversão (CRO), Core Web Vitals (PageSpeed 100/100) e indexação de SEO Geográfico.

## 📌 Visão Geral

Uma aplicação single-page (SPA) estática otimizada para captação de leads high-ticket, desenvolvida com design system Cyber/Glassmorphism. O principal diferencial estratégico é o motor de **SEO Dinâmico**, que adapta o conteúdo da página (títulos, meta tags e textos) com base na localização do usuário ou em parâmetros de campanha (UTMs).

## ⚙️ Tecnologias Utilizadas

* **HTML5 Semântico:** Estrutura otimizada para leitura de bots de busca.
* **Tailwind CSS (via CDN):** Estilização utilitária ágil para o design Glassmorphism e responsividade.
* **Vanilla JavaScript:** Lógica de manipulação de DOM, geolocalização e integração com WhatsApp sem dependências pesadas.
* **FontAwesome 6.4:** Iconografia vetorizada.
* **Google Fonts:** Tipografias *Outfit* e *Space Grotesk*.

## 🚀 Recursos Principais

1.  **Motor de SEO Dinâmico (Regionalização):**
    * Lê parâmetros na URL (`?cidade=nome-da-cidade` ou `?utm_term=nome`).
    * Caso não haja parâmetro, faz um fetch na API `ipapi.co` para descobrir a cidade do visitante pelo IP.
    * Injeta o nome da cidade dinamicamente nas tags `<title>`, `<meta description>`, na headline (H1) e nos textos de apoio.
2.  **Formulário de Triagem Inteligente:**
    * Captura dados cruciais: Nome, WhatsApp, Faturamento e Principal Dor.
    * Possui um algoritmo de *Scoring* interno que classifica o lead como "PADRÃO", "ALTA" ou "CRÍTICA / HIGH-TICKET" com base no faturamento e na dor escolhida.
    * Gera uma mensagem pré-formatada e redireciona automaticamente para o WhatsApp do time comercial da Eleva Digital.
3.  **Aviso de Privacidade (LGPD):**
    * Banner de consentimento de cookies e políticas de privacidade.
    * Salva a preferência do usuário no `localStorage` do navegador para não exibir o popup em visitas futuras.
4.  **UI/UX Avançada:**
    * Animações de entrada (Fade-up) utilizando `IntersectionObserver`.
    * Marquee (letreiro digital) contínuo destacando polos industriais e cidades da Baixada Santista para reforço de autoridade local.
    * Efeitos de Glassmorphism (vidro fosco) nos cards e navegação.

## 🛠️ Como Executar o Projeto

Por ser uma aplicação construída com HTML, CSS e JS puros (Client-side), não há necessidade de build ou instalação de pacotes (Node.js/NPM).

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/seu-usuario/eleva-digital-lp.git](https://github.com/seu-usuario/eleva-digital-lp.git)
    ```
2.  Abra a pasta do projeto.
3.  Execute o arquivo `index.html` diretamente em qualquer navegador moderno.
    * *Recomendação:* Para testar a API de geolocalização sem bloqueios de CORS locais, utilize a extensão **Live Server** no VS Code.

## 🔗 Testando o SEO Dinâmico

Para simular campanhas de tráfego pago rodando em cidades específicas, adicione o parâmetro `?cidade=` ao final da URL.

**Exemplos:**
* `http://localhost:5500/index.html?cidade=santos`
* `http://localhost:5500/index.html?cidade=carapicuiba`
* `http://localhost:5500/index.html?cidade=sao-paulo`

Observe que a aba do navegador, o H1 principal e as chamadas para o formulário serão alterados imediatamente.

## 📞 Integração Comercial

O script de envio do formulário está configurado para direcionar os leads qualificados diretamente para a central de atendimento:
* **Responsável:** Pedro Alan / Triagem Eleva Digital
* **Destino:** API do WhatsApp Web/Mobile.

---
© 2026 Eleva Digital. Todos os direitos reservados. Engenharia de Performance por Pedro Alan.