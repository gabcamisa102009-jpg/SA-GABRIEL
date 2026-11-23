
# Devolutiva formativa — Atividade 02 da SA

**Estudante:** Gabriel  
**Turma:** São Bento do Sul — Manhã  
**Unidade Curricular:** Programação de Aplicativos  
**Projeto:** NexusHealth ERP — Sistema Hospitalar  
**Repositório:** https://github.com/gabcamisa102009-jpg/SA-GABRIEL  
**Arquivo analisado:** `interface/index.html`  
**Data da verificação:** 23/11/2026

## Evolução identificada

Gabriel, desde a análise anterior, você publicou uma interface hospitalar com diferentes funcionalidades.

O projeto deixou de apresentar somente a estrutura inicial do repositório e passou a demonstrar operações programadas em JavaScript.

**A implementação atual representa uma evolução importante na Atividade 02.**

## Pontos positivos identificados

### 1. Interface organizada

Você desenvolveu um painel com navegação por seções, indicadores e áreas específicas para leitos, triagem e estoque.

A estrutura utiliza HTML e recursos de estilização para organizar a apresentação das informações.

### 2. Gestão de leitos

Foram implementadas funções para:

- Internar pacientes.
- Registrar a alta.
- Alterar o leito para higienização.
- Concluir a higienização e liberar o leito.
- Filtrar leitos por ala e situação.

Essas operações modificam os dados utilizados pela interface e atualizam a apresentação.

### 3. Triagem e fila de atendimento

O formulário permite informar o nome, a queixa e a prioridade de um paciente fictício.

O código organiza a fila de acordo com a prioridade informada e permite chamar pacientes para atendimento.

### 4. Controle de estoque

O sistema apresenta quantidades disponíveis, identifica itens abaixo do estoque mínimo e permite realizar reposições simuladas.

### 5. Organização em funções

Foram criadas funções com responsabilidades identificáveis, como:

- `atualizarKPIs()`
- `renderizarLeitos()`
- `internarPaciente()`
- `darAltaLeito()`
- `renderizarTriagem()`
- `chamarPaciente()`
- `renderizarEstoque()`
- `reporItem()`

Essa organização demonstra aplicação de funções, condições, listas e manipulação de elementos HTML.

## O que precisa ser corrigido

### 1. Separar HTML, CSS e JavaScript

Atualmente, a maior parte da implementação está concentrada em `interface/index.html`.

**Como melhorar:** mover o JavaScript para `interface/script.js` e os estilos personalizados para `interface/style.css`.

Isso facilitará a manutenção e a compreensão do programa.

### 2. Corrigir a apresentação das integrações

A interface apresenta integrações hospitalares com sistemas laboratoriais, imagens médicas e suprimentos.

Entretanto, os eventos são gerados por JavaScript, com dados locais e mensagens simuladas. Não há integração real com esses sistemas.

**Como melhorar:** identificar esses recursos como *simulações educacionais*, evitando transmitir a ideia de que os serviços estão realmente conectados.

### 3. Melhorar a validação e a segurança das entradas

Os nomes de pacientes e as queixas são inseridos em trechos HTML por meio de `innerHTML`.

**Como melhorar:** utilizar `textContent` para informações fornecidas pelo usuário ou realizar tratamento adequado antes de inseri-las no HTML.

Isso evita que uma entrada seja interpretada como código HTML.

### 4. Documentar a ausência de persistência

As informações são mantidas em variáveis JavaScript.

Ao atualizar a página, as alterações feitas durante a utilização são perdidas.

**Como melhorar:** esclarecer essa característica no README. A persistência poderá ser desenvolvida na etapa de banco de dados, não sendo necessário antecipar toda a integração agora.

### 5. Diferenciar classificação informada de classificação automática

Na triagem, a prioridade é selecionada pelo usuário. O programa ordena os pacientes conforme essa seleção.

**Como melhorar:** explicar que a interface organiza uma fila por prioridades informadas, mas não realiza uma classificação clínica automática.

Como o tema é hospitalar, a aplicação deve ser apresentada exclusivamente como simulação didática.

## Oportunidades de melhoria

- Criar comentários específicos para regras de mudança de situação dos leitos.
- Atualizar o README com instruções de execução e funcionalidades.
- Substituir gradualmente o `prompt()` por um formulário próprio de internação.
- Acrescentar mensagens de confirmação para operações importantes.
- Utilizar dados fictícios e evitar informações reais de pacientes.

## Testes recomendados

1. Internar um paciente em um leito disponível.
2. Registrar a alta e confirmar a mudança para higienização.
3. Concluir a higienização e verificar a liberação do leito.
4. Cadastrar pacientes com prioridades diferentes e conferir a ordenação.
5. Chamar um paciente e verificar sua remoção da fila.
6. Repor um item crítico e conferir a atualização do estoque.
7. Testar nomes vazios e entradas contendo caracteres especiais.
8. Atualizar a página e observar o comportamento dos dados.

## Prioridades para a próxima versão

1. **Separar JavaScript e CSS do HTML.**
2. **Tratar com segurança os dados inseridos na interface.**
3. **Identificar claramente as funcionalidades simuladas.**
4. **Atualizar a documentação específica do projeto.**
5. **Demonstrar as operações e explicar suas funções durante a aula.**

## Mensagem final

Gabriel, sua nova entrega demonstra uma evolução expressiva em relação à versão inicial do repositório.

Você implementou diferentes operações utilizando JavaScript, organizou os dados em estruturas apropriadas e criou funções que atualizam os elementos apresentados ao usuário.

O próximo passo é melhorar a separação dos arquivos, as validações e a documentação, mantendo a capacidade de explicar como cada funcionalidade foi construída.

**A interface agora apresenta evidências concretas para avaliação da Atividade 02.**

---
