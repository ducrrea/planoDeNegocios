# Plano de negócios: Fábrica de Software

**Autores:** João Gritti Pessoa, Larissa Vieira Lima, Maria Eduarda Correa, Thayssa Maneo

## 1. Introdução e Objetivo:

O projeto **Fábrica de Software** consiste em desenvolver um software em cerca de 30 minutos, a partir da ideia inicial, utilizando uma combinação de ferramentas de IA para prototipação e desenvolvimento, levando em consideração fatores como arquitetura do software e os desejos do cliente, além de inclusão e acessibilidade.

## 2. Solução idealizada:

Visando atingir tal objetivo, será construído um chatbot automatizado e inclusivo que coletará as respostas do cliente sobre o que deseja para o software, montando um prompt de prototipação que será levado para a plataforma Stitch. Após a aprovação do cliente sobre o protótipo, que pode ser aprovado visualmente ou por tecnologias assistivas, e então será montado um prompt para a plataforma AntiGravity que realizará o desenvolvimento da 1° versão do software que passará por testes e aperfeiçoamento e então será entregue ao cliente.

## 3. Processos do desenvolvimento:

Para realizar a construção do software separamos o processo em 4 etapas:

1. Levantamento de requisitos
2. Prototipação
3. Desenvolvimento
4. Testes

### 3.1 Levantamento de requisitos:

Através de um **formulário com 20 perguntas** sendo algumas objetivas outras dissertativas com finalidade de entender exatamente o que o cliente deseja para o seu software. Este processo **não será contabilizado nos 30 minutos**, visando maior clareza e assertividade nas respostas, além de conforto e liberdade nas respostas.

As perguntas estarão integradas ao chatbot e serão feitas diretamente no chat de conversa para manter tudo em somente uma plataforma.

#### Acessibilidade e Inclusão: 
Para que clientes com deficiência visual ou motora interajam com o chatbot de forma autônoma, a plataforma contará com:

- Suporte a Leitores de Tela: Uso de atributos aria-live="polite" para que novas mensagens do bot sejam lidas automaticamente sem interromper a navegação, além de <label> e aria-label em todos os campos.

- Entrada e Ditado por Voz (Speech-to-Text): Recurso para conversão de fala em texto no chat.

- Navegação 100% por Teclado: Acesso a todos os elementos via tecla Tab, Enter e atalhos, com foco visual claro.

- Feedback Sonoro: Sinais sonoros sutis indicando o envio/recebimento de mensagens ou validação de campos.

> **Perguntas do formulário:** \
> 1.\
> 2.\
> 3.\
> 4.\
> 5.\
> 6.\
> 7.\
> 8.\
> 9.\
> 10.\
> 11.\
> 12.\
> 13.\
> 14.\
> 15.\
> 16.\
> 17.\
> 18.\
> 19.\
> 20.

### 3.2 Prototipação:

Com o auxílio do ChatBot, as respostas do formulário serão analisadas e incorporadas em um modelo de prompt padronizado que serpa desenvolvido por nós. Após o modelo de prompt finalizado e revisado, ele então será enviado para a plataforma Stich AI, gerando um protótipo de alta fidelidade e encaminhando para o cliente aprovar para assim prosseguirmos com o desenvolvimento do projeto na plataforma AntiGravity. Caso o cliente queira alterar algo da prototipação, ele pode dizer e assim será alterado antes de ser desenvolvido.

**Modelo de prompt para prototipação:**
> O modelo será feito em inglês para garantir maior acertibilidade na criação dos protótipos. \
> "Context & Role: Act as a senior UI/UX designer. Create <tipo de interface (app de entregas)> for <público-alvo>. 
> 1. Visual Guidelines: Theme: <ex: minimalista, moderno, criativo>; Color palette: Primary <cor principal>, secondary: <cor secundária>, background: <cor do fundo> , text: <cor do texto> ; Typograph: <fonte>; Components Style: <bordas arredondadas, sombras, etc...>
> 2. Page Structure: Global Layout: <menu de navegação lateral, header, footer>; Header: <ordem dos elementos da header>; Main Section: <o que haverá na área central>
> 3. Step-by-Step UI: <Nome da página e o que ela deverá conter: detalhes de um menu, por exemplo>
> 4. UI States & Interactions: <detalhes como responsividade, animações, etc...>"

#### Prototipação Acessível e Inclusiva:
- Audiodescrição e Resumo Estruturado por IA: O próprio chatbot gerará uma descrição em áudio e texto resumindo o layout e a hierarquia visual do protótipo gerado.

- Suporte a ampliação de tela (zoom de até 200% sem quebrar o layout).

- Modo de alto contraste acionável.

- Validação de contraste mínimo de cores (4.5:1) e independência de cores (uso de texto/ícones além das cores para indicar status).

### 3.3 Desenvolvimento:
Para a etapa de desenvolvimentos seguiremos o mesmo processo da prototipação com a criação de um modelo que será adaptado para as necessidades do cliente.

**Modelo de desenvolvimento:**
>Programming Language: [EX: TypeScript / Python / C# / PHP / Java]
Backend Framework/Library: [EX: Node.js (Express) / Django / ASP.NET Core / Laravel / Spring Boot]
View Engine / Frontend: [EX: React with Tailwind CSS / Vue.js / Blade / Plain HTML + CSS / EJS]
Database: [EX: PostgreSQL / MySQL / SQLite / MongoDB]
>
>1. Role and Objective of the System \
Work as a Senior Full-Stack Software Engineer. Design the architecture and build the complete implementation of a web system called [System Name], strictly adhering to the MVC (Model-View-Controller) architectural pattern.
>2. Styling and Interface Guidelines \
For the project’s styling, follow the MCP from Stitch. 
>3. Project Architecture \
Organize the code into a clean, well-defined folder structure following the MVC pattern:
Models/: Definition of data entities, validations, and communication with the database/ORM.
Views/: User interfaces reflecting Stitch’s design, organized by module and separated from business logic.
Controllers/: Intermediaries that receive requests, execute business logic, call the Models, and render/return the Views or JSON data.
Routes/ / Config/: HTTP route mapping (GET, POST, PUT, DELETE) and configuration files.
>4. Code and Functionality Requirements \
Implement all the routes and CRUD methods necessary for the application to function.
Add clean error handling for requests and forms.
Keep the code commented in Portuguese and apply best practices (Clean Code, DRY, and SOLID principles).
Provide quick instructions on how to run the application and execute the database migrations/scripts at the end.
>5. Requisitos do software

### 3.4 Testes:

