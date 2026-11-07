# Desenvolvimento de Aplicativo — Finanças Pessoais com Inteligência Artificial

## 1. Visão geral do projeto

Desenvolva um aplicativo web de organização de finanças pessoais, com foco em simplicidade, inteligência artificial e experiência conversacional.

O aplicativo deve funcionar como um assistente financeiro pessoal, permitindo que os usuários controlem seus gastos, acompanhem suas receitas, estabeleçam metas e recebam recomendações de economia por meio de conversas em linguagem natural.

O grande diferencial do produto é eliminar a necessidade de preencher formulários extensos ou utilizar planilhas. O usuário deve conseguir registrar suas movimentações financeiras simplesmente conversando com o aplicativo.

**Objetivo principal:** tornar a organização financeira acessível, intuitiva e interessante, especialmente para pessoas que nunca utilizaram ferramentas de controle financeiro.

Todo o aplicativo deve estar em português brasileiro (PT-BR), incluindo textos, mensagens, datas, valores monetários e elementos da interface.

## 2. Identidade visual e experiência do usuário (UI/UX)

Crie uma interface moderna, sofisticada, intuitiva e visualmente atraente.

A identidade visual deve transmitir:
- Confiança e segurança.
- Organização e clareza.
- Tecnologia e inovação.
- Tranquilidade no gerenciamento financeiro.

### Diretrizes de design

- Utilize uma estética moderna, com inspiração em aplicativos financeiros premium.
- Priorize um layout limpo, com boa hierarquia visual.
- Utilize uma paleta de cores baseada em verde-esmeralda, azul-escuro, branco e tons neutros.
- Utilize cores diferentes para identificar receitas, despesas, alertas e metas.
- Adote cards com bordas arredondadas e sombras discretas.
- Utilize ícones modernos e consistentes.
- Adicione microinterações e animações suaves.
- Utilize gráficos claros e de fácil interpretação.
- Evite excesso de informações na tela.
- Mantenha boa legibilidade e acessibilidade.

A interface deve ser totalmente responsiva, funcionando perfeitamente em computadores, tablets e smartphones.

## 3. Estrutura principal do aplicativo

Crie as seguintes telas:

### 3.1. Landing Page

Desenvolva uma página inicial que apresente o aplicativo e seus benefícios.

Elementos:
- Nome e identidade visual do produto.
- Apresentação do assistente financeiro com IA.
- Explicação de como funciona o registro financeiro por conversa.
- Destaque para metas, relatórios e recomendações.
- Botão de cadastro.
- Botão de login.
- Seção de benefícios e funcionalidades.
- Seção explicando a segurança e privacidade dos dados.

A página deve transmitir profissionalismo e incentivar o usuário a experimentar o aplicativo.

### 3.2. Autenticação

Implemente:
- Cadastro com nome, e-mail e senha.
- Login.
- Recuperação de senha.
- Logout.
- Proteção das rotas autenticadas.
- Persistência segura da sessão.

Cada usuário deve possuir um ambiente financeiro individual e privado.

### 3.3. Dashboard financeiro

Crie um painel principal com uma visão geral das finanças do usuário.

Exiba:
- Saldo atual.
- Total de receitas do mês.
- Total de despesas do mês.
- Economia acumulada.
- Metas financeiras em andamento.
- Últimas transações.
- Gráfico de receitas versus despesas.
- Distribuição dos gastos por categoria.

Adicione filtros por período: semana, mês e ano.

Os valores apresentados devem ser atualizados automaticamente sempre que uma transação for criada, editada ou excluída.

### 3.4. Chat com o Agente Financeiro

Esta é a funcionalidade central do aplicativo.

Crie uma interface de chat moderna, semelhante a um aplicativo de mensagens, na qual o usuário possa conversar naturalmente com seu assistente financeiro.

O usuário deve conseguir enviar mensagens como:

- "Gastei R$ 35 no almoço."
- "Recebi R$ 2.500 de salário."
- "Paguei R$ 120 na conta de internet."
- "Quanto gastei com alimentação este mês?"
- "Onde estou gastando mais dinheiro?"
- "Quero economizar R$ 500 até dezembro."
- "Como posso reduzir meus gastos?"

O agente deve ser capaz de:

1. Interpretar mensagens em linguagem natural.
2. Identificar valores monetários, datas e descrições.
3. Diferenciar receitas e despesas.
4. Identificar automaticamente a categoria da movimentação.
5. Registrar transações no banco de dados.
6. Consultar o histórico financeiro do usuário.
7. Responder perguntas sobre os dados registrados.
8. Identificar padrões de consumo.
9. Recomendar oportunidades de economia.
10. Auxiliar na criação e no acompanhamento de metas.

### Comportamento inteligente

Quando o usuário informar uma movimentação, o agente deverá interpretar os dados e apresentar uma confirmação antes de salvar.

Exemplo:

Usuário: "Gastei R$ 45 no supermercado."

Agente:
"Entendi! Identifiquei uma nova despesa:

- Valor: R$ 45,00
- Categoria: Alimentação
- Descrição: Supermercado
- Tipo: Despesa

Deseja confirmar o registro?"

Disponibilize as ações "Confirmar" e "Editar".

Se alguma informação importante estiver ambígua, o agente deve perguntar ao usuário antes de registrar a movimentação.

O agente nunca deve inventar transações, saldos ou informações financeiras.

Adicione indicadores visuais de processamento, histórico de mensagens e sugestões de perguntas para facilitar o primeiro uso.

### 3.5. Transações financeiras

Crie uma tela para consultar e gerenciar todas as movimentações.

Funcionalidades:
- Listar receitas e despesas.
- Filtrar por categoria.
- Filtrar por período.
- Pesquisar por descrição.
- Editar movimentações.
- Excluir movimentações com confirmação.
- Visualizar detalhes de cada transação.

Cada transação deve possuir:
- Identificador único.
- Usuário proprietário.
- Descrição.
- Valor.
- Tipo (receita ou despesa).
- Categoria.
- Data.
- Data de criação.

O sistema deve atualizar os indicadores financeiros após qualquer alteração.

### 3.6. Metas financeiras

Permita que o usuário estabeleça objetivos financeiros.

Exemplos:
- Economizar R$ 1.000.
- Comprar um computador.
- Criar uma reserva de emergência.
- Guardar dinheiro para uma viagem.

Cada meta deve apresentar:
- Nome.
- Valor desejado.
- Valor acumulado.
- Data limite opcional.
- Progresso percentual.
- Status.

Utilize barras de progresso e indicadores visuais.

O agente financeiro deve conseguir criar metas por conversa e consultar seu progresso.

Não permita que o valor acumulado ultrapasse o objetivo sem atualizar corretamente o estado da meta.

### 3.7. Agente Financeiro — Recomendações inteligentes

Crie uma área dedicada às recomendações personalizadas.

O agente deverá analisar as movimentações registradas e identificar:
- Categorias com maiores despesas.
- Gastos recorrentes.
- Aumento de despesas em comparação com períodos anteriores.
- Possíveis oportunidades de economia.
- Progresso das metas financeiras.
- Hábitos que podem ser melhorados.

Exemplo:

"Seus gastos com alimentação aumentaram 18% em relação ao mês passado. Uma alternativa seria definir um limite mensal para essa categoria."

As recomendações devem ser baseadas nos dados reais do usuário.

Não invente padrões nem apresente comparações sem dados suficientes.

As recomendações devem possuir linguagem educativa, amigável e não julgadora.

O agente não deve se apresentar como consultor financeiro profissional nem recomendar investimentos específicos como se fossem aconselhamento personalizado.

### 3.8. Relatórios financeiros

Desenvolva uma área de relatórios com visualizações simples.

Inclua:
- Receitas por período.
- Despesas por período.
- Evolução do saldo.
- Gastos por categoria.
- Comparação entre meses.
- Evolução das metas.

Utilize gráficos interativos e filtros de datas.

Permita que o usuário compreenda rapidamente sua situação financeira sem precisar interpretar tabelas complexas.

## 4. Inteligência Artificial e integração

A inteligência artificial deve ser utilizada como núcleo da experiência conversacional.

Implemente uma integração real com um modelo de IA por meio de uma API segura.

Requisitos:
- Nunca exponha chaves de API no frontend.
- Utilize funções de backend ou Supabase Edge Functions para realizar chamadas à IA.
- Armazene credenciais em variáveis de ambiente.
- Envie ao modelo somente os dados necessários para responder à solicitação.
- Estruture as respostas da IA em formato JSON validado quando houver operações financeiras.
- Utilize ferramentas ou funções controladas para consultar, criar e atualizar dados.
- Exija confirmação do usuário antes de executar registros financeiros.
- Trate mensagens inválidas, erros de conexão e respostas incompletas.
- Implemente limites de utilização para evitar abuso e custos inesperados.

Não simule inteligência artificial com respostas estáticas. Caso a integração ainda não esteja configurada, apresente uma mensagem clara informando que o serviço precisa ser conectado.

## 5. Banco de dados e arquitetura

Utilize Supabase como infraestrutura principal, incluindo:
- PostgreSQL.
- Autenticação.
- Persistência de dados.
- Row Level Security (RLS).
- Edge Functions, quando necessário.

Estruture o banco de dados com as seguintes entidades:

**Users**
- id
- name
- email
- created_at

**Transactions**
- id
- user_id
- description
- amount
- type
- category
- transaction_date
- created_at
- updated_at

**Goals**
- id
- user_id
- name
- target_amount
- current_amount
- deadline
- status
- created_at

**ChatMessages**
- id
- user_id
- role
- content
- created_at

**Categories**
- id
- user_id (opcional para categorias personalizadas)
- name
- type
- created_at

Organize o código em componentes reutilizáveis, serviços, funções e estruturas bem definidas.

## 6. Segurança e privacidade

A segurança é um requisito obrigatório do projeto.

Implemente:

- Row Level Security em todas as tabelas que armazenam informações privadas.
- Políticas que garantam que cada usuário só possa acessar seus próprios registros.
- Validação de dados no frontend e no backend.
- Proteção contra SQL Injection.
- Proteção contra XSS.
- Controle de autenticação e autorização.
- Armazenamento seguro de credenciais.
- Proteção contra requisições abusivas.
- Tratamento seguro de erros.
- Proteção de rotas privadas.
- Verificação de propriedade dos registros em todas as operações.
- Princípio do menor privilégio.

Não confie exclusivamente nas validações do frontend.

Não exponha informações financeiras em logs, mensagens de erro ou respostas públicas.

Não armazene senhas manualmente ou em texto puro.

Não disponibilize dados financeiros de um usuário para outro.

O aplicativo não deve solicitar acesso bancário, senhas bancárias ou credenciais de instituições financeiras.

## 7. Regras de negócio

Implemente as seguintes regras:

1. Receitas aumentam o saldo e despesas reduzem o saldo.
2. O saldo deve ser calculado a partir das movimentações registradas.
3. Transações devem possuir valores positivos, com o tipo determinando se são receitas ou despesas.
4. Toda movimentação deve pertencer a um usuário autenticado.
5. Uma transação só pode ser alterada ou excluída pelo seu proprietário.
6. Metas devem possuir valores válidos e progresso consistente.
7. Relatórios devem utilizar dados reais do banco.
8. O agente não pode executar operações financeiras sem autorização.
9. O sistema deve evitar registros duplicados decorrentes de reenvio de mensagens.
10. Todos os valores devem utilizar o padrão monetário brasileiro (R$).

## 8. Experiência inicial e onboarding

Crie um processo de boas-vindas simples para novos usuários.

Apresente:
- Uma breve explicação do funcionamento.
- Uma demonstração de como registrar despesas por conversa.
- Uma opção para cadastrar a primeira receita.
- Uma opção para cadastrar a primeira despesa.
- Uma sugestão para criar a primeira meta financeira.

Evite exigir muitas informações no cadastro inicial.

O usuário deve conseguir começar a utilizar o aplicativo em poucos minutos.

## 9. Validação inicial do MVP

Prepare uma estratégia de validação do produto com:

**Hipóteses principais**
- Usuários preferem registrar despesas por conversa em vez de formulários.
- A classificação automática reduz o esforço de organização.
- Recomendações personalizadas incentivam melhores hábitos financeiros.

**Público para testes**
Comece com um grupo de 10 a 20 usuários iniciantes em organização financeira.

**Métricas de validação**
- Taxa de conclusão do primeiro registro.
- Tempo necessário para registrar uma transação.
- Quantidade de usuários que retornam ao aplicativo.
- Número de transações registradas por usuário.
- Percentual de classificações automáticas aceitas.
- Satisfação com as recomendações do agente.

**Objetivo:** identificar dificuldades de utilização, avaliar a qualidade da experiência conversacional e descobrir quais funcionalidades realmente agregam valor.

## 10. Requisitos técnicos e qualidade

- Desenvolva uma aplicação funcional, não apenas um protótipo visual.
- Utilize componentes reutilizáveis.
- Mantenha separação entre frontend, backend e integração com IA.
- Utilize TypeScript.
- Implemente estados de carregamento, sucesso, vazio e erro.
- Garanta acessibilidade e responsividade.
- Evite dados fictícios em funcionalidades de produção.
- Utilize dados demonstrativos somente em um ambiente claramente identificado como demonstração.
- Implemente feedback visual para todas as operações importantes.
- Não deixe botões sem funcionalidade.
- Não utilize informações sensíveis em exemplos ou dados de demonstração.

## 11. Etapas de desenvolvimento

Antes de iniciar a implementação, apresente um plano técnico contendo:

1. Arquitetura proposta.
2. Estrutura das telas.
3. Modelo do banco de dados.
4. Integração com inteligência artificial.
5. Estratégia de segurança.
6. Etapas de desenvolvimento.
7. Estratégia de validação do MVP.

Depois, desenvolva o aplicativo por etapas, priorizando:

**Fase 1 — Fundação**
- Identidade visual.
- Autenticação.
- Banco de dados.
- Segurança e isolamento dos usuários.

**Fase 2 — Funcionalidades financeiras**
- Dashboard.
- Registro e gerenciamento de transações.
- Categorias.
- Metas financeiras.

**Fase 3 — Inteligência artificial**
- Chat conversacional.
- Interpretação de mensagens.
- Classificação automática.
- Confirmação de operações.
- Recomendações personalizadas.

**Fase 4 — Análises**
- Relatórios.
- Gráficos.
- Comparações.
- Indicadores financeiros.

**Fase 5 — Testes e refinamento**
- Testes de segurança.
- Testes de funcionalidades.
- Testes de responsividade.
- Correção de erros.
- Preparação para validação com usuários reais.

## 12. Resultado esperado

Entregue um aplicativo de finanças pessoais moderno, seguro, intuitivo e funcional, com a inteligência artificial como principal diferencial.

A experiência deve fazer com que o usuário sinta que está conversando com um assistente financeiro pessoal, e não preenchendo uma planilha.

Priorize simplicidade, confiabilidade, transparência e facilidade de utilização.

**Importante:** não sacrifique a segurança ou a funcionalidade para acelerar o desenvolvimento visual. Todas as operações financeiras devem ser verificáveis, persistentes e protegidas.