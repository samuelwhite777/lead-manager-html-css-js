# Modelo Frontend: Sistema Básico de Gestão de Leads

Este projeto é um modelo de frontend para um sistema básico de gestão de leads, desenvolvido como parte de um portfólio para demonstrar habilidades em desenvolvimento web com HTML, Tailwind CSS e JavaScript puro.

## 🎯 Sobre o Projeto

O objetivo deste projeto é criar uma interface de usuário (UI) responsiva e interativa para as funcionalidades essenciais de um sistema de gerenciamento de leads. Ele serve como uma base que pode ser expandida e conectada a um backend real. Todas as interações e manipulação de dados são atualmente simuladas no frontend.

## ✨ Funcionalidades Principais (Versão Básica)

* **Autenticação de Usuário:**
    * Tela de Login (simulada com usuário `admin` e senha `password`).
    * Tela de Cadastro de novos usuários (simulada, com campos básicos como nome, email, telefone e senha).
    * Alternância visual entre as telas de login e cadastro.
* **Dashboard:**
    * Exibição de KPIs (Indicadores Chave de Performance) principais (Total de Leads, Leads Novos, Taxa de Conversão - com dados mock).
    * Gráficos visuais para "Leads por Status" e "Leads por Campanha" (renderizados com Chart.js e dados mock).
* **Gerenciamento de Leads:**
    * Visualização de leads em uma tabela interativa.
    * Filtros por status e campanha.
    * Busca por nome ou email do lead.
    * Modal para visualização de detalhes completos de um lead.
    * Modal para edição do status e adição de notas a um lead (interações simuladas).
* **Upload de Leads:**
    * Interface para upload de arquivos (CSV/XLSX).
    * Simulação do processamento do arquivo e adição de um novo lead à lista.
* **Interface Responsiva:**
    * Layout adaptável para diferentes tamanhos de tela (desktop, tablet, mobile) usando Tailwind CSS.
    * Menu principal no formato de header, com navegação horizontal em telas maiores e menu "hambúrguer" em telas menores.
* **Suporte (Simulado):**
    * Botão flutuante do WhatsApp para simular um canal de suporte.

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica do conteúdo.
* **CSS3 com Tailwind CSS:** Estilização responsiva e moderna.
* **JavaScript (Vanilla JS):** Manipulação do DOM, interatividade, simulação de lógica de negócios e chamadas de API.
* **Chart.js:** Para a criação dos gráficos no dashboard.

## 🚀 Como Usar/Executar

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git)
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd NOME_DO_SEU_REPOSITORIO
    ```
3.  Abra o arquivo `index.html` diretamente no seu navegador de preferência.

Como este é um projeto puramente frontend e autocontido em um único arquivo HTML (com CSS e JS embutidos ou via CDN), não há necessidade de instalação de dependências ou um servidor de desenvolvimento complexo para visualizá-lo.

## 🏗️ Estrutura do Projeto

Este projeto foi desenvolvido como uma Single-Page Application (SPA) simulada, onde todo o código (HTML, CSS e JavaScript) está contido em um único arquivo `index.html`. As diferentes "telas" ou "views" são gerenciadas dinamicamente pelo JavaScript, mostrando e ocultando seções do DOM conforme a navegação do usuário.

## 📝 Notas para o Portfólio

Este projeto demonstra:
* Criação de interfaces de usuário complexas e interativas.
* Manipulação do DOM com JavaScript puro.
* Uso de bibliotecas JavaScript (Chart.js).
* Estilização responsiva com Tailwind CSS.
* Simulação de funcionalidades de um sistema real para prototipagem e demonstração de UI/UX.
* Organização de código frontend em um contexto de SPA simulada.

## 🌱 Próximos Passos (Sugestões para Evolução)

Este modelo básico pode ser expandido com:
* Integração real com um backend (Python/Flask, Node.js/Express, PHP/Laravel, etc.).
* Conexão com um banco de dados (SQL ou NoSQL).
* Autenticação e autorização reais de usuários.
* Implementação real do upload e parsing de arquivos CSV/XLSX.
* Funcionalidades avançadas de CRM (como o Kanban board completo).
* Integração com APIs de LLMs (como Gemini, ChatGPT).
* Sistema de notificações persistente.
* Testes unitários e de integração.

---

<p align="center">Desenvolvido para fins de portfólio.</p>
