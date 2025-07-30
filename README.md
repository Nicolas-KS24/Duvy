# D'uvy

Aplicação web pessoal para armazenar e compartilhar momentos especiais, como poemas, desenhos, fotos e presentes. Criada inicialmente como um presente para a namorada, mas pensada para ser um modelo-base reutilizável para outros usos, como galerias ou organizadores de conteúdo.

---

## Visão Geral

- Armazenar e exibir conteúdos pessoais divididos em seções.
- Permitir comentários para cada tipo de conteúdo.
- Sistema de permissões com diferentes níveis (administrador e colaboradora).
- Upload e edição de arquivos.
- Funcionalidades opcionais: autenticação simples, modo claro/escuro e exportação em PDF.

---

## Funcionalidades

### Módulos principais

- **Fotos:** Upload e visualização de imagens com comentários.
- **Poemas:** Upload ou criação manual, com exibição e comentários.
- **Desenhos:** Upload e exibição, com comentários.
- **Presentes:** Seção restrita ao administrador, com upload e observações.
- **Comentários:** Associados a cada conteúdo, com autor e data.
- **Autenticação (opcional):** Login simples para controle de permissões.
- **Modo Claro/Escuro (opcional):** Alternância de tema da interface.
- **Exportação PDF (opcional):** Exportar conteúdos em formato PDF.

---

## Requisitos Funcionais

| Código | Descrição                                      |
|--------|------------------------------------------------|
| RF01   | Permitir upload de arquivos nas seções.       |
| RF02   | Exibir arquivos organizados por seção.        |
| RF03   | Permitir comentários em cada conteúdo.         |
| RF04   | Restringir edição da seção de presentes ao admin. |
| RF05   | Permitir edição/exclusão pelos autores.        |
| RF06   | Persistência dos dados em banco PostgreSQL.    |
| RF07   | Login simples para distinguir permissões (opcional). |
| RF08   | Alternância entre modo claro e escuro (opcional). |
| RF09   | Exportar conteúdos em PDF (opcional).           |

---

## Requisitos Não-Funcionais

| Código | Descrição                                        |
|--------|--------------------------------------------------|
| RNF01  | Aplicação responsiva e acessível em dispositivos móveis. |
| RNF02  | Uso do banco de dados PostgreSQL.                |
| RNF03  | API REST para comunicação com o front-end.       |
| RNF04  | Tempo de carregamento dos arquivos < 3 segundos. |
| RNF05  | Compatibilidade com hospedagens simples.         |
| RNF06  | Funcionalidades opcionais devem ser modulares.   |

---

## Tecnologias Utilizadas

- **Front-end:** HTML5, CSS3, JavaScript puro (ou React, se desejar).
- **Back-end:** Node.js com Express.
- **Banco de Dados:** PostgreSQL.
- **Autenticação:** JWT ou sessões (opcional).
- **Upload de arquivos:** Multer.
- **Exportação PDF:** jsPDF ou html2pdf.js.
- **Tema claro/escuro:** CSS custom properties + JS toggle.

---

## Estrutura do Projeto

