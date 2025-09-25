# ☁️ Guia Visual AZ-900: Fundamentos do Microsoft Azure


## 🏛️ 1. Pilares da Computação em Nuvem

A base de tudo. Entender os modelos de nuvem e de despesas é fundamental.

* 🌍 **Nuvem Pública:** Infraestrutura do provedor (Azure), compartilhada por vários clientes. Pague apenas pelo que usar.
* 🏠 **Nuvem Privada:** Infraestrutura dedicada a uma única organização, em seu próprio datacenter.
* 🤝 **Nuvem Híbrida:** Combinação estratégica das nuvens pública e privada para máxima flexibilidade.

### 🆚 Tabela Comparativa: CapEx vs. OpEx

| Modelo de Despesa               | Descrição                                         | Exemplo Comum        |
| ------------------------------- | ------------------------------------------------- | -------------------- |
| 💰 **CapEx (Despesa de Capital)** | Gasto inicial em infraestrutura física (servidores). | Nuvem Privada / On-premise |
| 💸 **OpEx (Despesa Operacional)** | Gasto contínuo em serviços, pago conforme o uso.  | Nuvem Pública        |

---

## ✨ 2. Benefícios e Conceitos-Chave do Azure

Por que usar a nuvem? Estes são os principais motivos e termos que você precisa saber.

* 📈 **Alta Disponibilidade:** Garantia de que seus aplicativos estarão sempre funcionando (definido por SLAs).
* ↕️↔️ **Escalabilidade & Elasticidade:** Ajuste de recursos para atender à demanda.
    * **Vertical (Scale Up):** Aumentar a potência (CPU, RAM) de uma VM.
    * **Horizontal (Scale Out):** Adicionar mais VMs para distribuir a carga.
* 🛡️ **Confiabilidade:** Resiliência contra falhas, graças à infraestrutura global e descentralizada.
* 🔒 **Segurança:** Ferramentas robustas, mas baseadas em um **modelo de responsabilidade compartilhada**.
* ⚖️ **Governança:** Ferramentas para garantir conformidade com políticas e padrões corporativos.
* ⚙️ **Gerenciabilidade:** Gerencie seus recursos via portal web, linha de comando (CLI), APIs ou PowerShell.

---

## 🔧 3. Tipos de Serviço de Nuvem (IaaS, PaaS, SaaS)

O modelo de responsabilidade compartilhada define o que você gerencia versus o que o Azure gerencia.

* 🏗️ **IaaS (Infraestrutura como Serviço)**
    * **O que é:** Blocos de construção básicos (VMs, Rede, Armazenamento).
    * **Você gerencia:** Sistema Operacional, aplicações, dados.
    * **Analogia:** Alugar o terreno e construir sua própria casa.

* 💻 **PaaS (Plataforma como Serviço)**
    * **O que é:** Ambiente para desenvolver e implantar apps sem se preocupar com a infraestrutura.
    * **Você gerencia:** Apenas suas aplicações e dados.
    * **Analogia:** Comprar uma casa pronta, mas você a decora e mobília.

* 📧 **SaaS (Software como Serviço)**
    * **O que é:** Software pronto para uso, acessado pela internet.
    * **Você gerencia:** Apenas seus dados dentro do software.
    * **Analogia:** Alugar um apartamento totalmente mobiliado e pronto para morar.

---

## 🗺️ 4. Arquitetura e Componentes do Azure

Como o Azure é organizado fisicamente e logicamente.

### Estrutura Global

* 🌍 **Regiões:** Um conjunto de datacenters em uma área geográfica. O Azure tem mais de 60 regiões globais.
* 🏢 **Zonas de Disponibilidade:** Datacenters fisicamente isolados dentro de uma mesma região para proteção contra falhas locais.
* 🔗 **Pares de Regiões:** Uma região do Azure emparelhada com outra na mesma geografia para recuperação de desastres.

### Hierarquia de Gerenciamento
└── 👑 Grupo de Gerenciamento (Políticas para toda a empresa)

└── 💳 Assinatura (Limite de cobrança e acesso)

└── 📂 Grupo de Recursos (Contêiner lógico para seus recursos)

└── 💡 Recurso (VM, Banco de Dados, Rede, etc.)

---

## 🛠️ 5. Principais Serviços por Categoria

Uma visão geral dos recursos mais comuns que você encontrará no Azure.

### 🖥️ Computação
* **Máquinas Virtuais (VMs):** Servidores Windows ou Linux na nuvem (IaaS).
* **Serviços de Contêineres:**
    * **Instâncias de Contêiner:** Execute contêineres rapidamente, sem gerenciamento.
    * **Serviço de Kubernetes (AKS):** Orquestração de contêineres em larga escala.
* **Azure Functions:** Execute código sob demanda, sem servidores (Serverless).
* **Área de Trabalho Virtual do Azure:** Desktop como serviço (DaaS) na nuvem.

### 🌐 Rede
* **Rede Virtual (VNet):** Sua rede privada e isolada no Azure.
* **Gateway de VPN:** Conexão segura entre sua rede local e a VNet pela internet.
* **ExpressRoute:** Conexão privada e dedicada entre sua rede local e o Azure.

### 📦 Armazenamento
* **Blob Storage:** Armazenamento de objetos para grandes volumes de dados não estruturados.
* **Disk Storage:** Discos para suas Máquinas Virtuais.
* **Azure Files:** Compartilhamentos de arquivos de rede na nuvem.

---

## 🛡️ 6. Identidade, Acesso e Segurança

Proteger seus recursos e dados é crucial.

* 🆔 **Microsoft Entra ID:** Serviço de identidade e acesso baseado em nuvem. Fornece autenticação e autorização.
* 🔑🔑 **Autenticação Multifator (MFA):** Camada extra de segurança que exige duas ou mais provas de identidade.
* 👤 **Controle de Acesso Baseado em Função (RBAC):** Conceda permissões granulares aos usuários (quem pode fazer o quê e onde).
* 🕵️‍♂️ **Microsoft Defender para Nuvem:** Ferramenta para monitoramento de segurança e proteção contra ameaças.
* 📜 **Confiança Zero (Zero Trust):** Modelo de segurança que assume que não há confiança implícita. "Nunca confie, sempre verifique".

---

7. Identidade, Acesso e Segurança
Microsoft Entra ID (antigo Azure AD): Serviço de gerenciamento de identidades e acesso baseado em nuvem.

Autenticação vs. Autorização:

Autenticação: Confirma quem você é.

Autorização: Define o que você pode fazer.

Autenticação Multifator (MFA): Camada adicional de segurança que exige duas ou mais formas de verificação.

Acesso Condicional: Aplica políticas de acesso com base em condições (usuário, local, dispositivo).

RBAC (Role-Based Access Control): Controle de acesso baseado em função para gerenciar o acesso aos recursos do Azure.

Confiança Zero (Zero Trust): Modelo de segurança que assume que toda solicitação de acesso é uma ameaça em potencial.

Microsoft Defender para Nuvem: Ferramenta para monitorar e proteger cargas de trabalho na nuvem e on-premises contra ameaças.

---

8. Gerenciamento de Custos, Governança e Conformidade
Custos
Calculadora de Preços: Estima o custo dos produtos do Azure.

Calculadora de TCO (Custo Total de Propriedade): Estima a economia ao migrar do ambiente on-premises para o Azure.

Gerenciamento de Custos do Azure: Ferramenta para monitorar, controlar e otimizar os gastos no Azure.

Marcas (Tags): Metadados (par nome-valor) para organizar recursos e rastrear custos.

Governança e Conformidade
Azure Policy: Impõe padrões organizacionais e avalia a conformidade dos recursos.

Bloqueio de Recursos: Protege recursos de exclusão ou modificação acidental (níveis: CanNotDelete e ReadOnly).

Microsoft Purview: Família de soluções para governança de dados, risco e conformidade.

---

9. Ferramentas de Gerenciamento, Implantação e Monitoramento
Gerenciamento e Implantação
Azure Arc: Estende o gerenciamento do Azure para ambientes híbridos e multinuvem.

Azure Resource Manager (ARM): Serviço de implantação e gerenciamento do Azure que permite criar, atualizar e excluir recursos.

Modelos ARM: Arquivos JSON que definem a infraestrutura e a configuração para implantação (Infraestrutura como Código - IaC).

Bicep: Linguagem específica de domínio (DSL) que simplifica a criação de modelos ARM.

Monitoramento
Assistente do Azure (Azure Advisor): Analisa os recursos e oferece recomendações personalizadas para otimizar confiabilidade, segurança, desempenho, custo e excelência operacional.

Integridade do Serviço do Azure (Service Health): Informa sobre o status dos serviços do Azure, problemas que podem afetar você e a integridade de seus recursos específicos.

Azure Monitor: Coleta, analisa e age com base em telemetria de ambientes na nuvem e on-premises para maximizar a disponibilidade e o desempenho.

