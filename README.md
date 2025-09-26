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

## 🛡️ 7. Identidade, Acesso e Segurança

Proteger seus recursos, dados e identidade é a prioridade máxima.

* 🆔 **Microsoft Entra ID:** Serviço de gerenciamento de identidades e acesso baseado em nuvem (antigo Azure AD).

* 🔐 **Autenticação vs. Autorização:**

   * **Autenticação:** Confirma quem você é (seu login e senha).

   * **Autorização:** Define o que você pode fazer (suas permissões).

* 🔑🔑 **Autenticação Multifator (MFA):** Camada adicional de segurança que exige duas ou mais formas de verificação para conceder acesso.

* 🚦 **Acesso Condicional (Conditional Access):** Aplica políticas de acesso baseadas em condições (sinais) como usuário, local e dispositivo.

* 👤 **Controle de Acesso Baseado em Função (RBAC):** Concede permissões granulares aos usuários para gerenciar o acesso aos recursos do Azure (quem pode fazer o quê e onde).

* 🕵️‍♂️ **Microsoft Defender para Nuvem:** Ferramenta unificada para monitorar a postura de segurança e proteger cargas de trabalho na nuvem e on-premises contra ameaças.

* 📜 **Confiança Zero (Zero Trust):** Modelo de segurança que parte do princípio "nunca confie, sempre verifique". Assume que toda solicitação de acesso, mesmo interna, é uma ameaça em potencial.

---

## 💰 8. Custos, Governança e Conformidade

Controlar gastos e garantir a conformidade são essenciais para o sucesso na nuvem.

### Custos
* 🧮 **Calculadora de Preços:** Ferramenta para estimar o custo dos produtos e serviços do Azure antes de implantá-los.

* 🧾 **Calculadora de TCO (Custo Total de Propriedade):** Ajuda a estimar a economia que você pode obter ao migrar suas cargas de trabalho locais para o Azure.

* 📊 **Gerenciamento de Custos do Azure:** Ferramenta para monitorar, analisar, controlar e otimizar seus gastos no Azure.

* 🏷️ **Marcas (Tags):** Metadados (par chave-valor) que você pode aplicar aos recursos para organizá-los logicamente e rastrear custos por projeto ou departamento.

### Governança e Conformidade
* 📜 **Azure Policy:** Permite criar, atribuir e gerenciar políticas que impõem regras e padrões organizacionais aos seus recursos, garantindo a conformidade.

* 🔒 **Bloqueio de Recursos:** Protege assinaturas, grupos de recursos ou recursos individuais contra exclusão ou modificação acidental. Níveis: CanNotDelete e ReadOnly.

* 🔍 **Microsoft Purview:** Família de soluções para governança, risco e conformidade de dados, ajudando a mapear e gerenciar dados em todo o seu patrimônio.

---

## 🚀 9. Ferramentas, Implantação e Monitoramento

Ferramentas que facilitam a administração, a implantação e a observabilidade do seu ambiente.

### Gerenciamento e Implantação
* 🌐 **Azure Arc:** Estende o plano de controle e gerenciamento do Azure para ambientes híbridos (on-premises) e multinuvem (AWS, GCP).

* 🏗️ **Azure Resource Manager (ARM):** É o serviço de implantação e gerenciamento do Azure. Ele fornece uma camada de gerenciamento que permite criar, atualizar e excluir recursos em sua assinatura.

* 📄 **Modelos ARM e Bicep (IaC):**

  * **Modelos ARM:** Arquivos JSON que definem a infraestrutura e a configuração da sua implantação (Infraestrutura como Código).

  * **Bicep:** Uma linguagem específica de domínio (DSL) mais simples e declarativa que compila para modelos ARM.

### Monitoramento
* 👨‍🏫 **Assistente do Azure (Azure Advisor):** Um consultor de nuvem personalizado que analisa sua configuração e uso de recursos, oferecendo recomendações para otimizar a confiabilidade, segurança, desempenho, custo e excelência operacional.

* ❤️‍🩹 **Integridade do Serviço do Azure (Service Health):** Fornece uma visão personalizada do status dos serviços do Azure, informando sobre interrupções, manutenções planejadas e avisos de integridade que podem afetar seus recursos.

* 📈 **Azure Monitor:** Plataforma completa para coletar, analisar e agir com base em dados de telemetria de seus ambientes na nuvem e locais para maximizar a disponibilidade e o desempenho.
