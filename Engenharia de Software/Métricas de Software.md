# Engenharia de Software
## Métricas de Software - Análise de Ponto de Função (APF)

### O que são Métricas de Software?

Imagine que você precisa construir uma casa. Como saber quanto tempo vai levar? Quanto vai custar? Quantos pedreiros você vai precisar? Você usa **medidas**: metros quadrados da casa, quantidade de cômodos, tipo de acabamento, etc.

No desenvolvimento de software, as **métricas** são essas "medidas" que nos ajudam a:

1. ***Estimar*** quanto tempo e esforço será necessário para desenvolver o software.
2. ***Planejar*** recursos (quantas pessoas, quanto dinheiro).
3. ***Controlar*** o progresso do projeto.
4. ***Comparar*** diferentes projetos e equipes.
5. ***Melhorar*** processos futuros com base em dados históricos.

**Análise de Ponto de Função (APF)** é uma das principais técnicas para medir o **tamanho funcional** de um software, focando no que o sistema faz para o usuário, não em como é implementado.

### Conceitos Básicos da APF

| Conceito | O que é? | Analogia |
| :------- | :------- | :------- |
| **Ponto de Função (PF)** | Unidade de medida que representa uma funcionalidade do sistema do ponto de vista do usuário | Como "metro quadrado" para casas |
| **Tamanho Funcional** | Quantidade total de funcionalidades que o software oferece ao usuário | Tamanho total da casa em m² |
| **Função Transacional** | Processos que o usuário executa (entrada, consulta, saída de dados) | Ações que você faz na casa (cozinhar, dormir) |
| **Função de Dados** | Informações que o sistema armazena ou referencia | Móveis e objetos da casa |

**Características da APF:**
- **Independente de tecnologia:** Não importa se é Java, Python, web ou mobile.
- **Foco no usuário:** Mede o que o usuário vê e usa, não o código interno.
- **Padrão internacional:** Definida pelo IFPUG (International Function Point Users Group).
- **Base para estimativas:** Permite calcular prazo, custo e equipe necessária.

### Tipos de Funções

A APF classifica as funcionalidades em **5 tipos principais**:

#### Funções de Dados (Armazenamento)

1. **ALI - Arquivo Lógico Interno**
   - **O que é:** Grupo de dados criado, mantido e usado pelo próprio sistema.
   - **Exemplo:** Cadastro de clientes, produtos, pedidos em um e-commerce.
   - **Analogia:** Gavetas organizadas na sua casa onde você guarda suas coisas.

2. **AIE - Arquivo de Interface Externa**
   - **O que é:** Grupo de dados que o sistema usa, mas é mantido por outro sistema.
   - **Exemplo:** Consultar CEP nos Correios, cotação do dólar no Banco Central.
   - **Analogia:** Usar a internet ou energia elétrica (vem de fora, mas você usa).

#### Funções Transacionais (Processamento)

3. **EE - Entrada Externa**
   - **O que é:** Processo que recebe dados do usuário para criar, alterar ou excluir informações.
   - **Exemplo:** Cadastrar cliente, alterar senha, excluir produto.
   - **Analogia:** Colocar comida na geladeira, organizar o guarda-roupa.

4. **SE - Saída Externa**
   - **O que é:** Processo que envia dados processados/calculados para o usuário.
   - **Exemplo:** Relatório de vendas, gráfico de desempenho, fatura com cálculos.
   - **Analogia:** Usar a calculadora para mostrar o resultado de uma conta.

5. **CE - Consulta Externa**
   - **O que é:** Processo que apenas recupera e mostra dados sem cálculos complexos.
   - **Exemplo:** Listar clientes, buscar produto por nome, visualizar perfil.
   - **Analogia:** Olhar o que tem na geladeira sem mexer em nada.

### Processo de Contagem

O processo de APF segue **7 passos principais**:

#### 1. Identificar o Escopo da Contagem
- **O que contar:** Definir quais funcionalidades serão medidas.
- **Fronteira:** Separar o que é do sistema e o que é externo.

#### 2. Identificar Funções de Dados
- Encontrar todos os **ALI** (dados internos) e **AIE** (dados externos).
- Contar os **tipos de dados** (campos) e **tipos de registros** de cada função.

#### 3. Identificar Funções Transacionais
- Encontrar todas as **EE** (entradas), **SE** (saídas) e **CE** (consultas).
- Analisar a complexidade de cada função.

#### 4. Determinar a Complexidade
Cada função é classificada como **Simples**, **Média** ou **Complexa** baseada em:
- **Dados:** Quantidade de tipos de dados e registros.
- **Transações:** Quantidade de arquivos referenciados e tipos de dados.

#### 5. Calcular Pontos de Função Não Ajustados
Use a tabela de pesos para cada tipo e complexidade:

| Tipo de Função | Simples | Média | Complexa |
| :------------- | :------ | :---- | :------- |
| **ALI** | 7 PF | 10 PF | 15 PF |
| **AIE** | 5 PF | 7 PF | 10 PF |
| **EE** | 3 PF | 4 PF | 6 PF |
| **SE** | 4 PF | 5 PF | 7 PF |
| **CE** | 3 PF | 4 PF | 6 PF |

#### 6. Calcular o Fator de Ajuste (FA)
Avalia 14 características gerais do sistema (0 a 5 pontos cada):
- Comunicação de dados
- Processamento distribuído
- Performance
- Facilidade de uso
- Taxa de transações
- Entrada de dados online
- Interface com usuário
- Atualização online
- Processamento complexo
- Reusabilidade
- Facilidade de instalação
- Facilidade operacional
- Múltiplos locais
- Facilidade de mudanças

**Fórmula do FA:** FA = 0,65 + (0,01 × Σ características)

#### 7. Calcular Pontos de Função Ajustados
**PF Ajustado = PF Não Ajustado × FA**

### Considerações Finais

A **Análise de Ponto de Função** é uma ferramenta poderosa para medir software do ponto de vista funcional. Ela ajuda gerentes de projeto e desenvolvedores a:

- **Planejar** melhor os projetos
- **Estimar** custos e prazos com mais precisão
- **Comparar** diferentes equipes e projetos
- **Controlar** o progresso durante o desenvolvimento
- **Melhorar** processos com base em dados históricos

**Dica Importante:** A APF é mais eficaz quando usada consistentemente ao longo do tempo, permitindo que a organização construa uma base histórica de dados para estimativas cada vez mais precisas.

Como qualquer métrica, a APF não é perfeita, mas quando aplicada corretamente por pessoas treinadas, fornece uma base sólida e objetiva para o gerenciamento de projetos de software.

---

### NESMA: Alternativa à APF

A **NESMA** (Netherlands Software Metrics Association) é uma metodologia de contagem de pontos de função baseada na APF, mas com algumas diferenças práticas:

- **Origem:** Criada na Holanda, segue o padrão ISO/IEC 24570.
- **Semelhanças:** Mede o tamanho funcional do software, utiliza conceitos e tipos de funções semelhantes à APF (ALI, AIE, EE, SE, CE).
- **Diferenças principais:**
  - **Regras de contagem:** NESMA detalha mais situações específicas, como contagem em projetos de manutenção e melhorias.
  - **Documentação:** NESMA é mais pragmática, com guias claros para casos do dia a dia.
  - **Ajuste:** O fator de ajuste é opcional e menos enfatizado.
- **Quando usar:** NESMA é bastante utilizada na Europa, especialmente em contratos públicos, e facilita auditorias e comparações entre fornecedores.

**Resumo:** NESMA e APF são muito parecidas, mas NESMA é mais prática para manutenção e contratos, enquanto APF é mais tradicional e aceita internacionalmente.