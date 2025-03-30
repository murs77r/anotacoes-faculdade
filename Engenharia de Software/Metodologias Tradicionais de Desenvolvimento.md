# Engenharia de Software
## Conceitos Básicos da Engenharia de Software
A **Engenharia de Software** é uma área da computação que aplica princípios de engenharia ao desenvolvimento de software, estabelecendo métodos, ferramentas e procedimentos sistemáticos para criar produtos de software com qualidade, seguindo premissas como:
1. ***Organizar*** o processo de desenvolvimento
2. ***Garantir*** a qualidade do produto final
3. ***Gerenciar*** custos e prazos
4. ***Facilitar*** a manutenção e evolução
5. ***Aumentar*** a confiabilidade do software

## Conceitos Básicos de Software

Dentro dos conceitos básicos de software, alguns pontos fundamentais devem ser tratados para um melhor entendimento:

| Tipo | Definição | Exemplo |
|------|-----------|---------|
| **Software** | Conjunto de instruções lógicas que controlam o funcionamento de um computador | Sistemas operacionais, aplicativos, jogos |
| **Firmware** | Conjunto de instruções programadas em um chip de memória não-volátil | BIOS, sistema operacional de roteadores |
| **Hardware** | Componentes físicos que executam o software | Processadores, memória RAM, placas-mãe |

E dentro do contexto de Software, é importante ressaltar que ele é **intangível** (não pode ser tocado fisicamente), **flexível** (podendo ser modificado com relativa facilidade), **não se desgasta** (mas podendo ficar obsoleto) e é **personalizável** (sendo adaptado às necessidades específicas).

## Metodologias Tradicionais de Desenvolvimento
Uma **metodologia de desenvolvimento** é um conjunto estruturado de práticas, técnicas, procedimentos e regras utilizadas para planejar, desenvolver, testar e manter um sistema de software.

### Cascata (Waterfall)

![Cascata](https://upload.wikimedia.org/wikipedia/commons/0/08/Modelo_em_cascata.png)

As principais características dessa metodologia são:
1. Abordagem **sequencial** e **linear**
2. Cada fase deve ser **concluída** antes de iniciar a próxima
3. **Documentação** extensa em cada etapa
4. Baseado em **planejamento detalhado** prévio

O metodologia em Cascata tem fases bem definidas e fixas, sendo elas:
1. **Levantamento de Requisitos**:
   - Entendimento do problema
   - Definição das necessidades do cliente
   - Documentação completa dos requisitos
2. **Projeto/Design**:
   - Arquitetura do sistema
   - Design de interface
   - Modelagem de dados
3. **Implementação**:
   - Codificação do sistema
   - Criação dos componentes
4. **Verificação/Testes**:
   - Testes unitários
   - Testes de integração
   - Testes de sistema
5. **Manutenção**:
   - Correção de erros
   - Implementação de melhorias
   - Adaptações

Essa metodologia é interessante para projetos com requisitos que tendem a não se alterar ao longo do tempo, entretanto, pelo fato de ser engessada e ter estrutura inflexível, é extremamente desvantajoso para projetos que são sujeitos a mudanças em seu processo de desenvolvimento.

### Prototipação

![Prototipação](https://media.licdn.com/dms/image/v2/C4E12AQGdOYy34uwVtg/article-inline_image-shrink_400_744/article-inline_image-shrink_400_744/0/1586809505963?e=1746662400&v=beta&t=6wDPuI5RDX49Co78IXp-CN2wcwe9NhoIYi9u2HbHu_s)

Essa metodologia se baseia principalmente na criação de **protótipos funcionais** para validação, com foco na **experimentação** e **feedback** do cliente.

As suas fases são formadas por:
1. **Coleta de Requisitos Inicial** 
   - Identificação das necessidades básicas
   - Definição dos objetivos do protótipo
2. **Projeto Rápido** 
   - Design preliminar
   - Foco nas partes visíveis ao usuário
3. **Construção do Protótipo** 
   - Desenvolvimento de uma versão simplificada
   - Implementação das principais funcionalidades
4. **Avaliação** 
   - Demonstração ao cliente
   - Coleta de feedback
5. **Refinamento** 
   - Ajustes baseados no feedback
   - Melhoria do protótipo
6. **Engenharia do Produto** 
   - Desenvolvimento completo do sistema
   - Baseado no protótipo final aprovado

Dentre as vantagens, possibilita a melhora da especificação no desenvolvimento do projeto, o que consequentemente diminui os custos de criação e manuntenção do software. Entretanto, essa metodologia pode enfrentar algumas dificuldades, como a possibilidade do cliente confundir o protótipo com o produto final.

### Espiral

![Espiral](https://engenhariasoftware.wordpress.com/wp-content/uploads/2013/02/espiral.gif)

A metodologia em Espiral combina elementos do **modelo cascata** e da **prototipação**, com base no desenvolvimento em **ciclos repetitivos** (espirais) e foco na **análise de riscos**.

As fases, que são repetidas a cada quadrante (que são 4 ao total), são:
1. **Determinação de Objetivos**
   - Definição de requisitos
   - Identificação de restrições
   - Estabelecimento de alternativas
2. **Análise de Riscos** 
   - Identificação dos riscos
   - Análise das alternativas
   - Estratégia de mitigação
3. **Desenvolvimento e Validação** 
   - Desenvolvimento do produto
   - Verificação e validação
4. **Planejamento da Próxima Fase** 
   - Revisão do progresso
   - Planejamento do próximo ciclo

As vantagens dessa metodologia são o gerenciamento eficaz de riscos ao desenvolvimento do projeto, uma maior flexibilidade para mudanças (mesmo não sendo considerando "Ágil"), e, principalmente, o desenvolvimento incremental. Entretanto, ainda assim é complexa e exige um custo grande para a análise de riscos, além de pode acabar sendo excessivo para projetos pequenos.

## Comparativo entre Metodologias Tradicionais[^1]

| Característica | Cascata | Prototipação | Espiral |
|----------------|---------|--------------|---------|
| **Flexibilidade** | Baixa | Média | Alta |
| **Envolvimento do Cliente** | Início e fim | Frequente | Em cada ciclo |
| **Gerenciamento de Riscos** | Limitado | Moderado | Robusto |
| **Adequado para Requisitos** | Estáveis | Incertos | Complexos |
| **Tempo até primeira entrega** | Longo | Curto | Médio |
| **Documentação** | Extensa | Moderada | Significativa |

[^1]: **OBSERVAÇÃO**: Essa tabela comparativa foi feita por Inteligência Artificial.
