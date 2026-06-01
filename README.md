<h1>Projeto: Gerenciador/Controle de filmes e séries</h1>
<br>
<h2>Objetivos do Projeto</h2>
<br>
•	Um sistema feito para gerenciar e controlar filmes e séries, categorizando a princípio como "vistos" e "não vistos", com intuito de ajudar o usuário a tanto manter suas experiências pessoais de assistir determinada mídia documentada de uma certa forma, quanto compartilhar dita experiência para outros usuários, descrevendo e recomendando, ou até mesmo criticando essa mídia. <br>
•	O objetivo principal é adicionar funcionalidades mais complexas de sites alternativos para ser uma opção objetivamente mais completa de catalogar e controlar filmes e séries vistos ou não vistos.<br><br>

# 1. Gerência de Configuração

## 1.1 Itens de Configuração do Projeto

Os itens de configuração são os artefatos do projeto que devem ser controlados e versionados para garantir a consistência, rastreabilidade e manutenção da aplicação ao longo do seu ciclo de vida.

### Código-fonte

O código-fonte compreende todos os arquivos responsáveis pela implementação do sistema, incluindo o front-end, o back-end e as integrações com serviços externos.

**Motivo do controle:**  
Alterações no código podem impactar diretamente as funcionalidades da aplicação, sendo necessário manter um histórico de mudanças para facilitar correções, auditorias e evolução do projeto.

---

### README.md

O arquivo README.md contém as principais informações sobre o projeto, incluindo objetivos, requisitos, tecnologias utilizadas, instruções de uso e documentação complementar.

**Motivo do controle:**  
A documentação deve permanecer alinhada com o estado atual do projeto, garantindo que desenvolvedores e avaliadores tenham acesso a informações atualizadas.

---

### Dockerfile

O Dockerfile define o processo de criação da imagem Docker utilizada para executar a aplicação em ambientes padronizados.

**Motivo do controle:**  
Qualquer alteração nesse arquivo pode modificar o ambiente de execução do sistema, afetando sua implantação e funcionamento.

---

### Arquivos YAML

Os arquivos YAML são utilizados para configurar processos de implantação, integração contínua e demais recursos relacionados à infraestrutura do projeto.

**Motivo do controle:**  
Mudanças nesses arquivos podem impactar diretamente a execução automática de processos e a disponibilização da aplicação.

---

### Workflows do GitHub Actions

Os workflows do GitHub Actions automatizam tarefas como testes, build e deploy da aplicação.

**Motivo do controle:**  
A configuração incorreta desses fluxos pode interromper processos automatizados importantes para o desenvolvimento e manutenção do sistema.

---

### Imagem Docker

A imagem Docker representa uma versão empacotada da aplicação pronta para execução.

**Motivo do controle:**  
O versionamento das imagens permite identificar exatamente qual versão da aplicação está sendo executada em cada ambiente.

---

### Dependências

As dependências incluem bibliotecas, frameworks e ferramentas utilizadas pelo projeto, como React, Node.js, Express, Axios e demais pacotes instalados.

**Motivo do controle:**  
Atualizações não controladas podem causar incompatibilidades, falhas de segurança ou problemas de funcionamento da aplicação.

---

### Documentação do Projeto

Inclui requisitos funcionais, requisitos não funcionais, diagramas, atas de reunião, documentação técnica e demais artefatos produzidos durante o desenvolvimento.

**Motivo do controle:**  
A documentação registra decisões importantes do projeto e deve acompanhar sua evolução para manter a consistência das informações.

## 1.2 Baseline do Projeto

### Baseline da Segunda Unidade

**Nome da Baseline:** Entrega da Segunda Unidade  
**Versão Associada:** v2.0.0

#### Arquivos que compõem a Baseline:
- Código-fonte do Front-end
- Código-fonte do Back-end
- README.md
- package.json
- Dockerfile
- deployment.yaml
- Workflows do GitHub Actions
- Scripts de Banco de Dados
- Documentação do Projeto

**Descrição:**

A baseline v2.0.0 representa a versão consolidada da segunda unidade do projeto. Esta versão contém as principais funcionalidades desenvolvidas até o momento, incluindo o sistema de catalogação de filmes e séries, personalização de perfis, sistema de avaliações, acompanhamento de séries por episódios, criação de tags personalizadas e importação de dados de plataformas externas como o Letterboxd.

Essa versão é considerada estável por possuir documentação atualizada, estrutura de implantação definida e funcionalidades devidamente integradas ao sistema.

---

## 1.3 Estratégia de Versionamento

O projeto utiliza o modelo de versionamento semântico (Semantic Versioning) baseado no padrão:

**MAJOR.MINOR.PATCH**

Onde:

- **MAJOR:** mudanças significativas ou incompatíveis com versões anteriores;
- **MINOR:** adição de novas funcionalidades compatíveis;
- **PATCH:** correções de erros e pequenas melhorias.

### Histórico de Versões

| Versão | Descrição |
|---------|------------|
| v1.0.0 | Entrega da primeira unidade |
| v2.0.0 | Entrega da segunda unidade |
| v2.0.1 | Correções de bugs e ajustes menores |
| v2.1.0 | Inclusão de novas funcionalidades sem quebra de compatibilidade |
| v3.0.0 | Alterações estruturais significativas |

---

## 1.4 Controle de Mudanças

### Mudança 1

**Descrição:** Implementação do sistema de acompanhamento de séries por episódios.

**Itens Impactados:**
- Front-end
- Back-end
- Banco de Dados

**Motivo:**  
Permitir um controle mais detalhado do progresso do usuário em séries.

**Impacto:**  
Criação de novas estruturas para armazenamento do progresso por episódio e cálculo automático de porcentagem de conclusão.

**Status:** Concluído.

---

### Mudança 2

**Descrição:** Implementação do sistema de tags personalizadas.

**Itens Impactados:**
- Front-end
- Back-end
- Banco de Dados

**Motivo:**  
Permitir que cada usuário organize seus conteúdos utilizando categorias próprias.

**Impacto:**  
Criação de entidades para armazenamento das tags e relacionamento com filmes e séries.

**Status:** Concluído.

---

### Mudança 3

**Descrição:** Implementação da importação de dados de plataformas externas.

**Itens Impactados:**
- Front-end
- Back-end
- Integrações Externas

**Motivo:**  
Facilitar a migração de usuários provenientes de plataformas como Letterboxd.

**Impacto:**  
Criação de mecanismos para leitura, validação e importação de dados externos.

**Status:** Concluído.

---

## 1.5 Solicitação de Mudança

**Título da Mudança:**  
Sistema de Recomendações Personalizadas

**Descrição da Mudança:**  
Implementar um sistema capaz de recomendar filmes e séries com base no histórico de avaliações, conteúdos assistidos e tags utilizadas pelos usuários.

**Motivo da Mudança:**  
Melhorar a experiência do usuário e facilitar a descoberta de novos conteúdos.

**Itens de Configuração Impactados:**
- Código-fonte
- Banco de Dados
- API
- Documentação

**Impacto Técnico:**  
Necessidade de desenvolver algoritmos de recomendação e consultas adicionais ao banco de dados.

**Riscos Envolvidos:**  
Possível aumento do tempo de processamento e necessidade de ajustes no desempenho.

**Prioridade:** Alta.

**Necessidade de Testes:** Sim.

**Decisão:**  
Aprovada para análise e implementação em versões futuras.

---

## 1.6 Auditoria de Configuração

| Item Verificado | Conforme? | Observação |
|----------------|-----------|------------|
| README atualizado | Sim | Documentação revisada e atualizada |
| Dockerfile presente | Sim | Arquivo configurado para containerização |
| deployment.yaml presente | Sim | Configuração de implantação disponível |
| Imagem Docker versionada | Sim | Controle realizado por tags de versão |
| Link do Docker Hub correto | Sim | Repositório configurado corretamente |
| Baseline definida | Sim | Baseline v2.0.0 registrada |
| Mudanças registradas | Sim | Histórico documentado |

---

## 1.7 Gerência de Dependências

### Dependências Utilizadas

#### Front-end
- React
- React Router DOM
- Axios
- CSS3
- HTML5

#### Back-end
- Java / Spring Boot
- Node.js
- Express
- JWT (JSON Web Token)
- bcrypt

#### Banco de Dados
- MySQL ou PostgreSQL

#### Containerização
- Docker
- Imagem Base Node.js

#### Ferramentas de Desenvolvimento
- Git
- GitHub
- GitHub Actions

---

### Onde as Dependências Estão Registradas?

As dependências do projeto estão registradas principalmente nos seguintes arquivos:

- Dockerfile
- deployment.yaml
- Documentação do Projeto

---

### Riscos de Atualização sem Testes

A atualização de dependências sem a realização de testes pode causar:

- Quebra de compatibilidade entre bibliotecas;
- Falhas de execução da aplicação;
- Vulnerabilidades de segurança;
- Alterações inesperadas no comportamento do sistema;
- Interrupção de funcionalidades já implementadas.

---

### Controle de Atualização de Dependências

A equipe realizará o controle das dependências através das seguintes práticas:

- Utilização de versionamento pelo GitHub;
- Atualizações realizadas em branches específicas;
- Execução de testes antes da integração;
- Revisão das alterações pela equipe;
- Registro das mudanças realizadas na documentação do projeto;
- Utilização de versões estáveis das bibliotecas sempre que possível.
