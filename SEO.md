# Relatório de Otimização SEO — Projeto Rock Nacional

**URL Publicada:** https://github.io  
**Autor:** Fernando Martins  
**Data:** 25/11/2026  

---

## 1. Estratégia de Palavras-Chave por Página

Cada página recebeu 3 palavras-chave foco (1 principal e 2 secundárias) distribuídas estrategicamente nas tags `<title>`, `<meta name="description">`, cabeçalhos (`<h1>`) e links internos:

* **Página Inicial (`index.html`):**
  * **Principal:** rock nacional
  * **Secundárias:** bandas brasileiras, punk rock e crossover thrash
* **Página Estilos (`estilos.html`):**
  * **Principal:** estilos do rock
  * **Secundárias:** história do rock, vertentes do rock
* **Página Contato (`contato.html`):**
  * **Principal:** contato rock nacional
  * **Secundárias:** sugestão de bandas brasileiras, cena punk brasileira

---

## 2. Decisões Técnicas Tomadas

1. **Meta Tags Únicas:** Criação de `<title>` (até 60 caracteres) e `<meta name="description">` (entre 140 e 160 caracteres) exclusivos para cada uma das 3 páginas.
2. **URLs Canônicas e Amigáveis:** Uso de nomes de arquivos limpos (`index.html`, `estilos.html`, `contato.html`) e definição da tag `<link rel="canonical">` com URL absoluta em cada página para evitar conteúdo duplicado.
3. **Open Graph e Twitter Cards:** Implementação completa das tags `og:title`, `og:description`, `og:url`, `og:type`, `og:locale` e `og:image` com banner dedicado de `1200×630 px` (`og-rock-nacional.jpg`) para previews otimizados em redes sociais e mensageiros.
4. **Dados Estruturados (Schema.org / JSON-LD):** Inserção de scripts `application/ld+json` adequados ao contexto de cada página (`CollectionPage` com `ItemList` de `MusicGroup` e `Person` na home; `WebPage` na página de estilos; `ContactPage` na página de contato).
5. **Rastreamento e Indexação (`robots.txt` e `sitemap.xml`):** Publicação dos arquivos na raiz do projeto autorizando a varredura pelos buscadores e mapeando todas as URLs ativas com prioridades e datas de atualização.
6. **Arquitetura de Links Internos Descritivos:** Conexão entre as páginas por meio de texto-âncora contextualizado dentro do `<main>` (evitando termos genéricos como "clique aqui").
7. **Otimização de Imagens e Performance:** Conversão das imagens de conteúdo para o formato moderno `.webp`, definição explícita de atributos `width` e `height` para prevenir *Layout Shift (CLS)*, textos alternativos (`alt`) descritivos e carregamento tardio (`loading="lazy"`) aplicado apenas às imagens abaixo da primeira dobra.
8. **Acessibilidade e Semântica HTML5:** Uso de estrutura semântica (`<header>`, `<nav aria-label="...">`, `<main>`, `<h1>`, `<caption>` em tabelas, `<fieldset>`/`<legend>` em formulários) e ajuste de contraste de cores.

---

## 3. Resultados Lighthouse (Modo Celular) — Antes e Depois

Testes realizados via **Google PageSpeed Insights (Mobile)** na URL principal (`https://github.io`):

| Métrica (Lighthouse Mobile) | Antes | Depois | Evolução | Meta Exigida |
| :--- | :---: | :---: | :---: | :---: |
| **SEO** | 91 | **100** | +9 pts | **≥ 95** |
| **Acessibilidade** | 100 | **100** | Mantido | **≥ 90** |
| **Práticas Recomendadas** | 100 | **100** | Mantido | — |
| **Desempenho (Performance)** | 63 | **74** | +11 pts | — |
