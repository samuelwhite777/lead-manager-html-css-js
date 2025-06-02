# Modelo Frontend: Sistema Básico de Gestão de Leads

Este projeto é um modelo de frontend para um sistema básico de gestão de leads, desenvolvido como parte de um portfólio para demonstrar habilidades em desenvolvimento web com HTML, Tailwind CSS e JavaScript puro. Ele simula as interações de um sistema de CRM focado em leads.

## 🎯 Sobre o Projeto

O objetivo deste projeto é criar uma interface de usuário (UI) responsiva e interativa para as funcionalidades essenciais de um sistema de gerenciamento de leads. Ele serve como uma base que pode ser expandida e conectada a um backend real. Todas as interações e manipulação de dados são atualmente simuladas no frontend usando dados mock.

## ✨ Funcionalidades Implementadas (Modelo Básico)

* **Autenticação de Usuário (Simulada):**
    * Tela de Login com campos para usuário e senha.
        * Validação simulada: `admin` / `password`.
    * Tela de Cadastro de novos usuários com campos básicos:
        * Nome Completo, Email, Telefone, Senha e Confirmação de Senha.
        * Validação simulada e feedback ao usuário.
    * Alternância visual entre as telas de login e cadastro.
* **Dashboard Interativo:**
    * Exibição de KPIs (Indicadores Chave de Performance) principais:
        * Total de Leads
        * Leads Novos
        * Taxa de Conversão (calculada com base nos dados mock).
    * Gráficos visuais renderizados com Chart.js:
        * "Leads por Status" (Gráfico de Rosca/Doughnut).
        * "Leads por Campanha" (Gráfico de Barras).
* **Gerenciamento de Leads Completo:**
    * Visualização de leads em uma tabela responsiva e interativa.
    * Filtros dinâmicos por:
        * Status do Lead.
        * Campanha do Lead.
    * Campo de busca textual para filtrar por nome ou email do lead.
    * Modal para visualização de detalhes completos de um lead selecionado (incluindo campanha, origem, data de criação).
    * Funcionalidade de edição no modal para:
        * Alterar o Status do Lead.
        * Adicionar/Editar Notas textuais para o lead.
    * As alterações feitas no modal são refletidas nos dados mock e atualizam dinamicamente a tabela e o dashboard.
* **Upload de Leads (Simulado):**
    * Interface para seleção de arquivos (simulando aceitar CSV/XLSX).
    * Exibição do nome do arquivo selecionado.
    * Botão "Processar Arquivo" que simula o processamento:
        * Adiciona um novo lead de exemplo aos dados mock.
        * Atualiza todas as visualizações (KPIs, gráficos, tabela) para refletir o novo lead.
        * Fornece feedback visual ao usuário sobre o processo.
* **Interface Responsiva e Navegação:**
    * Layout totalmente adaptável para diferentes tamanhos de tela (desktop, tablet, mobile) utilizando Tailwind CSS.
    * Menu principal no formato de header fixo no topo.
    * Navegação horizontal em telas maiores (desktop/tablet).
    * Menu "hambúrguer" funcional para navegação em telas menores (mobile), que exibe os mesmos links de forma vertical.
* **Suporte (Simulado):**
    * Botão flutuante do WhatsApp que direciona para uma conversa com um número de suporte (placeholder).

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Estrutura semântica do conteúdo.
* **CSS3 com Tailwind CSS:** Estilização responsiva e moderna, seguindo uma abordagem utility-first.
* **JavaScript (Vanilla JS):** Manipulação do DOM, interatividade, lógica de simulação de dados, controle de estado das views e componentes.
* **Chart.js:** Para a criação dos gráficos dinâmicos e visualmente atraentes no dashboard.

## 🚀 Como Usar/Executar

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_SEU_REPOSITORIO.git)
    ```
2.  Navegue até o diretório do projeto:
    ```bash
    cd NOME_DO_SEU_REPOSITORIO
    ```
3.  Abra o arquivo `index.html` diretamente no seu navegador de preferência (Chrome, Firefox, Edge, etc.).

Como este é um projeto puramente frontend e autocontido em um único arquivo HTML (com CSS e JS embutidos ou via CDN), não há necessidade de instalação de dependências ou um servidor de desenvolvimento complexo para visualizá-lo e testar suas funcionalidades simuladas.

## 🏗️ Estrutura do Projeto

Este projeto foi desenvolvido como uma Single-Page Application (SPA) simulada, onde todo o código (HTML, CSS e JavaScript) está contido em um único arquivo `index.html`. As diferentes "telas" ou "views" (Dashboard, Gerenciar Leads, Upload) são gerenciadas dinamicamente pelo JavaScript, que mostra e oculta as seções apropriadas do DOM conforme a navegação do usuário, proporcionando uma experiência de usuário fluida sem recarregamentos de página.

O código JavaScript está estruturado com funções claras para cada responsabilidade, como manipulação de autenticação, navegação, renderização de componentes (KPIs, gráficos, tabela), manipulação de modais e simulação de interações de backend.

## 📝 Notas para o Portfólio

Este projeto demonstra:
* Capacidade de criar interfaces de usuário (UI) complexas, interativas e responsivas.
* Proficiência em manipulação dinâmica do DOM utilizando JavaScript puro.
* Experiência com bibliotecas JavaScript populares como Chart.js para visualização de dados.
* Habilidade em utilizar frameworks CSS modernos como Tailwind CSS para estilização eficiente e design responsivo.
* Compreensão de como simular funcionalidades de um sistema real para prototipagem rápida e demonstração de conceitos de UI/UX.
* Organização de código frontend em um contexto de SPA simulada, com foco na clareza e manutenibilidade.
* Adição de comentários explicativos no código para facilitar a compreensão da lógica implementada.

## 🌱 Sugestões para Features Futuras (Evolução do Projeto)

Este modelo básico serve como um excelente ponto de partida. Algumas sugestões para evoluir este projeto incluem:

* **Integração com Backend Real:**
    * Desenvolver um backend (ex: Python/Flask, Node.js/Express, PHP/Laravel) para persistir os dados.
    * Substituir os `mockLeads` por chamadas de API (GET, POST, PUT, DELETE) para interagir com o backend.
* **Banco de Dados:**
    * Conectar o backend a um banco de dados (SQL como PostgreSQL/MySQL, ou NoSQL como MongoDB) para armazenamento persistente de leads e usuários.
* **Autenticação e Autorização Reais:**
    * Implementar um sistema de autenticação seguro (ex: JWT, OAuth) no backend.
    * Gerenciar sessões de usuário.
    * Potencialmente adicionar diferentes níveis de permissão de usuário.
* **Upload de Arquivos Real:**
    * Implementar no backend a lógica para receber, validar e processar (parse) arquivos CSV/XLSX enviados.
    * Extrair os dados dos leads dos arquivos e salvá-los no banco de dados.
* **CRM Avançado - Kanban Board:**
    * Reintroduzir a visualização Kanban para o funil de vendas.
    * Permitir arrastar e soltar leads entre as colunas de status, com atualização no backend.
* **Integração com LLM (Assistente IA):**
    * Reintroduzir a aba do Assistente IA.
    * Integrar com uma API de LLM real (como Gemini API, OpenAI API) para fornecer respostas inteligentes a perguntas do usuário sobre os leads ou o sistema.
* **Sistema de Notificações Persistente:**
    * Reintroduzir a aba de Notificações.
    * Implementar um sistema no backend para gerar notificações (novos leads, mudanças de status importantes, lembretes) e exibi-las em tempo real ou ao carregar a página.
* **Paginação e Otimização de Performance:**
    * Para a tabela de "Gerenciar Leads", implementar paginação no frontend e/ou backend para lidar com grandes volumes de dados de forma eficiente.
* **Validação de Formulários Avançada:**
    * Adicionar validação mais robusta nos campos de cadastro e edição, tanto no frontend quanto no backend.
* **Testes:**
    * Escrever testes unitários para as funções JavaScript.
    * Implementar testes de integração e/ou end-to-end.
* **Melhorias de UI/UX:**
    * Animações mais elaboradas e transições suaves.
    * Opção de tema escuro (Dark Mode).
    * Internacionalização (i18n) para suportar múltiplos idiomas.
* **Integração com Facebook Leads API:**
    * Conectar diretamente à API do Facebook para buscar novos leads automaticamente.

---

<p align="center">Desenvolvido para fins de portfólio.</p>
<!-- 
<p align="center">
  <a href="SEU_LINKEDIN_AQUI">LinkedIn</a> •
  <a href="mailto:SEU_EMAIL_AQUI">Email</a> •
  <a href="SEU_WEBSITE_AQUI">Website</a>
</p> 
-->
