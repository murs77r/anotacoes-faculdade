# Engenharia de Software
## Diagramas UML
### Introdução

A UML (Unified Modeling Language) é uma linguagem padrão para especificação, visualização, construção e documentação de artefatos de sistemas de software. Ela fornece uma série de diagramas que facilitam a compreensão e o design de sistemas complexos. Cada tipo de diagrama da UML possui uma finalidade específica e contribui para o entendimento dos diversos aspectos de um sistema, desde sua estrutura estática até seus comportamentos dinâmicos e de interação.

Os diagramas UML podem ser classificados em dois grandes grupos: **diagramas estruturais** e **diagramas comportamentais**. A seguir, estão descritos os principais diagramas UML, categorizados por seu tipo e detalhados quanto à sua finalidade e principais elementos.

---

### 1. Diagramas Estruturais

Os diagramas estruturais representam os aspectos estáticos do sistema, ou seja, os elementos que compõem a estrutura do sistema e seus relacionamentos.

#### 1.1 Diagrama de Classes

- **Descrição:** Representa as classes do sistema, seus atributos, métodos e os relacionamentos entre elas.
- **Principais elementos:** Classes, atributos, métodos, associações, heranças, dependências, agregações e composições.
- **Utilidade:** Fundamental para o design orientado a objetos, serve como base para a implementação do sistema.

#### 1.2 Diagrama de Objetos

- **Descrição:** Mostra instâncias concretas das classes em um determinado momento, destacando valores de atributos e links entre objetos.
- **Principais elementos:** Objetos (instâncias), links (relacionamentos).
- **Utilidade:** Ilustra exemplos reais de funcionamento do sistema em situações específicas.

#### 1.3 Diagrama de Estrutura Composta

- **Descrição:** Detalha a estrutura interna de uma classe, mostrando seus componentes internos e como eles se conectam.
- **Principais elementos:** Partes, portas, conectores, classes internas.
- **Utilidade:** Útil para modelar sistemas complexos, componentes reutilizáveis e arquiteturas baseadas em composição.

#### 1.4 Diagrama de Componentes

- **Descrição:** Representa os componentes físicos do sistema (módulos, bibliotecas, arquivos, etc.) e suas dependências.
- **Principais elementos:** Componentes, interfaces, dependências.
- **Utilidade:** Auxilia na visualização da estrutura de implementação e na organização de grandes sistemas.

#### 1.5 Diagrama de Pacotes

- **Descrição:** Organiza os elementos do sistema em grupos lógicos chamados pacotes e mostra as dependências entre eles.
- **Principais elementos:** Pacotes, classes, dependências.
- **Utilidade:** Facilita a organização e modularização do sistema, sendo útil em projetos de grande porte.

#### 1.6 Diagrama de Implantação

- **Descrição:** Mostra a arquitetura física do sistema, incluindo nós (servidores, dispositivos), artefatos e suas conexões.
- **Principais elementos:** Nós, artefatos, conexões, dispositivos.
- **Utilidade:** Essencial para o planejamento da infraestrutura e distribuição do sistema em ambiente real.

---

### 2. Diagramas Comportamentais

Os diagramas comportamentais enfatizam os aspectos dinâmicos do sistema, ou seja, o comportamento dos objetos e a interação entre eles ao longo do tempo.

#### 2.1 Diagrama de Casos de Uso

- **Descrição:** Descreve as funcionalidades do sistema do ponto de vista do usuário, mostrando atores e seus objetivos.
- **Principais elementos:** Atores, casos de uso, relacionamentos (inclusão, extensão, generalização).
- **Utilidade:** Ajuda a levantar requisitos e a comunicar as funcionalidades do sistema de forma clara.

#### 2.2 Diagrama de Máquina de Estados

- **Descrição:** Modela os estados possíveis de um objeto e as transições entre eles em resposta a eventos.
- **Principais elementos:** Estados, transições, eventos, ações.
- **Utilidade:** Útil para sistemas baseados em eventos ou com comportamento dependente de estados.

#### 2.3 Diagrama de Atividade

- **Descrição:** Representa fluxos de trabalho, processos ou algoritmos, destacando atividades, decisões e paralelismos.
- **Principais elementos:** Atividades, decisões, ramificações, junções, início/fim.
- **Utilidade:** Ideal para modelar processos de negócio e fluxos de controle complexos.

#### 2.4 Diagrama de Sequência

- **Descrição:** Mostra a interação entre objetos ao longo do tempo, focando na troca de mensagens em uma linha do tempo vertical.
- **Principais elementos:** Objetos, linhas de vida, mensagens, ativações.
- **Utilidade:** Esclarece a ordem das chamadas e interações em cenários específicos.

#### 2.5 Diagrama de Interação Geral (Communication)

- **Descrição:** Foca na estrutura das interações entre objetos, mostrando as mensagens trocadas e os relacionamentos entre eles.
- **Principais elementos:** Objetos, links, mensagens numeradas.
- **Utilidade:** Complementa o diagrama de sequência, enfatizando a topologia da comunicação.

#### 2.6 Diagrama de Tempo

- **Descrição:** Representa o comportamento de objetos em relação ao tempo, mostrando mudanças de estado, eventos e duração.
- **Principais elementos:** Objetos, linhas de tempo, eventos, intervalos temporais.
- **Utilidade:** Útil para sistemas temporizados ou que exigem análise de sincronismo e temporização.

---

### Resumo dos Tipos de Diagramas UML

| Tipo                 | Exemplos de Diagramas                                                   |
|----------------------|-------------------------------------------------------------------------|
| **Estruturais**      | Classe, Objeto, Estrutura Composta, Componentes, Pacotes, Implantação   |
| **Comportamentais**  | Casos de Uso, Máquina de Estados, Atividade, Sequência, Interação Geral, Tempo |

---

### Diferenças entre os Diagramas Apresentados e o Padrão UML 2.5

A UML 2.5 foi publicada em 2015 como uma evolução da linguagem, trazendo ajustes conceituais, melhorias na clareza da documentação e pequenas alterações nos diagramas. As diferenças principais entre os diagramas apresentados acima (que refletem a UML 2.x como um todo) e o padrão UML 2.5 estão listadas a seguir:

- **Padronização e Simplificação:**  
  A UML 2.5 consolidou definições, simplificou regras e tornou a especificação mais coesa e menos ambígua. Alguns diagramas tiveram suas descrições e notações levemente ajustadas para maior clareza, mas os tipos de diagramas permanecem os mesmos.

- **Quantidade de Diagramas:**  
  A UML 2.5 define oficialmente 14 tipos de diagramas, sendo que todos os diagramas listados neste documento estão incluídos na versão 2.5. Algumas nomenclaturas podem variar — por exemplo, o "Diagrama de Interação Geral" também é conhecido como "Diagrama de Comunicação".

- **Reorganização de Conceitos:**  
  Conceitos internos de como os elementos interagem (como relacionamentos, conectores e artefatos) foram reorganizados para facilitar a compreensão e a implementação de ferramentas CASE.

- **Detalhamento dos Diagramas de Interação:**  
  Na UML 2.5, os diagramas de interação são um grupo que engloba: Sequência, Comunicação (Interação Geral), Tempo e Visão Geral da Interação. Todos esses estão contemplados na lista apresentada.

- **Notações e Elementos:**  
  A UML 2.5 manteve a maior parte da notação dos diagramas, mas padronizou e esclareceu alguns símbolos (como setas, caixas e conectores) para garantir consistência entre ferramentas.

- **Exclusão de Diagramas Obsoletos:**  
  Alguns diagramas existentes em versões muito antigas da UML (anteriores à 2.0) foram removidos ou fundidos. Nenhum dos diagramas apresentados nesta lista foi excluído na 2.5.
  
---

### Considerações Finais

O entendimento dos diferentes diagramas UML é essencial para o desenvolvimento de sistemas bem estruturados, facilitando a comunicação entre equipe técnica, stakeholders e usuários. Cada diagrama serve a um propósito específico e, quando usados em conjunto, proporcionam uma visão abrangente do sistema, desde sua concepção até sua implantação e operação.
