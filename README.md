# az900-resumo-curso
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab no curso da Azure 

# AZ-900 : Introdução aos Conceitos Básicos da Microsoft Azure

### Objetivo Geral

Este curso fornece um nível de conhecimento básico sobre:

- Conceitos do Azure
- Principais serviços do Azure
- Principais soluções e ferramentas de gerenciamento segurança geral e segurança de rede
- Governança, privacidade e recursos de conformidade e gerenciamento de custos do Azure

## Computação em Nuvem ☁

### O que é a computação em Nuvem?

- A **computação em nuvem** é o fornecimento de serviços de computação pela internet, habilitando inovações mais rápidas, recursos flexíveis e economias de escala.



### Nuvem Privada

- As organizações criam um ambiente em nuvem em seu datacenter.
- As organizações são responsáveis por operar os serviços que fornecem.
- Não fornece aceso aos usuários fora da organização.


### Nuvem Pública

- Pertencente a serviços de nuvem ou provedor de hosting.
- Fornece recursos e serviços a várias organizações e usuários
- Acessada via conexão de rede segura (geralmente pela Internet).



### Nuvem Híbrida

- Combina nuvens públicas e privadas para permitir que os aplicativos sejam executados no local mais adequado.



### Comparação de Modelos de Nuvem

**Nuvem pública**

- Nenhuma despesa de capital para escalar verticalmente.
- Os aplicativos podem ser provisionados e desprovisionados rapidamente.
- As organizações pagam apenas pelo que utilizam.

**Nuvem privada**

- As organizações têm controle total sobre os recursos e a segurança
- As organizações são responsáveis pela manutenção e pelas atualizações de hardware.

**Nuvem híbrida**

- As organizações determinam onde executar seus aplicativos.
- As organizações controlam a segurança, a conformidade e os requisitos legais.
- Fornece a maior flexibilidade.

## Comparar CapEx e OpEx

### Despesas de capital (CapEx)

- O gasto inicial de dinheiro em infraestrutura física.
- As despesas do CapEx têm um valor que se reduz com o tempo.
- Comum em ambientes On premisses (Nuvem Privada)

### Despesas operacionais (OpEx)

- Gastar com produtos e serviços conforme necessário, pagamento conforme o uso.
- Seja cobrado imediatamente.
- Comum em ambientes de Nuvem Pública

### Modelo baseado em consumo

Os provedores de serviços em nuvem operam em um modelo baseado no consumo, o que significa que os usuários finais pagam somente pelos recursos que usam

- Melhor previsão de custos.
- São fornecidos preços para recursos e serviços individuais.
- A cobrança é feita com base no seu uso real.

  ### Resumo Principais Ferramentas da Azure

## 🌐 **Computação**

* **Azure Virtual Machines (VMs):** Máquinas virtuais para rodar sistemas operacionais e aplicações.
* **App Service:** Hospedagem de aplicações web, APIs e mobile apps sem precisar gerenciar servidores.
* **Azure Functions:** Funções serverless (executam código sob demanda).
* **Azure Kubernetes Service (AKS):** Gerenciamento de containers e orquestração via Kubernetes.


## 💾 **Armazenamento e Banco de Dados**

* **Azure Blob Storage:** Armazenamento de objetos (arquivos, imagens, backups).
* **Azure Files:** Compartilhamento de arquivos SMB/NFS.
* **Azure SQL Database:** Banco relacional gerenciado (baseado no SQL Server).
* **Cosmos DB:** Banco NoSQL globalmente distribuído.


## 🔒 **Rede e Segurança**

* **Virtual Network (VNet):** Criação de redes privadas na nuvem.
* **Azure Firewall:** Proteção de rede com firewall gerenciado.
* **Azure Front Door / CDN:** Distribuição de conteúdo e balanceamento de carga global.
* **Azure DDoS Protection:** Proteção contra ataques de negação de serviço.
* **Azure Active Directory (Entra ID):** Gerenciamento de identidades e autenticação (SSO, MFA).


## 📊 **Monitoramento e Gestão**

* **Azure Monitor:** Coleta métricas e logs para análise de performance.
* **Log Analytics:** Consultas detalhadas em logs da infraestrutura.
* **Azure Advisor:** Recomendações de otimização de custos, segurança e desempenho.
* **Cost Management + Billing:** Controle e análise de custos da nuvem.


## 🤖 **DevOps e Integração**

* **Azure DevOps:** Conjunto de ferramentas para CI/CD, planejamento de projetos e repositórios de código.
* **GitHub Actions (integrado ao Azure):** Automatização de pipelines CI/CD com GitHub.
* **Azure Repos:** Repositório Git privado.
* **Azure Pipelines:** Automação de build e deploy.


## 📈 **IA, Dados e Analytics**

* **Azure Synapse Analytics:** Análise de grandes volumes de dados (data warehouse).
* **Power BI Embedded:** Visualização e dashboards integrados.
* **Azure Machine Learning:** Treinamento e deploy de modelos de IA.
* **Cognitive Services:** APIs prontas de visão computacional, linguagem e voz.


## 🔄 **Backup, Recuperação e Governança**

* **Azure Backup:** Backup em nuvem de servidores e VMs.
* **Azure Site Recovery:** Continuidade de negócios e recuperação de desastres.
* **Azure Policy:** Definição e aplicação de regras de conformidade.
* **Azure Blueprints:** Automação de ambientes com governança.


# Conceitos Iniciais de Cloud com Azure

## Benefícios da Computação em Nuvem

### **Alta disponibilidade**

- A alta disponibilidade se concentra em garantir a disponibilidade máxima, independentemente de interrupções ou eventos que possam ocorrer.
- O Azure é um ambiente de nuvem altamente disponível com garantias de tempo de atividade, dependendo do serviço.
- Essas garantias fazem parte dos SLAs (Contratos de Nível de Serviço)

### **Escalabilidade**

- A escalabilidade refere-se à capacidade de ajustar recursos para atender à demanda.
- A capacidade de escalar significa que você poderá adicionar mais recursos para lidar melhor com o aumento da demanda.
- O outro benefício da escalabilidade é que você não está pagando além do necessário pelos serviços.
- Como a nuvem é um modelo baseado em consumo, você paga apenas pelo que usa.
- Se a demanda cair, você poderá reduzir seus recursos e, assim, reduzir seus custos.
- Com a escala vertical, se você estivesse desenvolvendo um aplicativo e precisasse de mais capacidade de processamento, poderia escalar verticalmente para adicionar mais CPUs ou RAM à máquina virtual.

### **Elasticidade**

- Com a elasticidade, se você experimentasse um salto repentino acentuado na demanda, seus recursos implantados poderiam ser expandidos (automaticamente ou manualmente).
- Por exemplo, você pode adicionar máquinas virtuais ou contêineres por meio da expansão.
- Da mesma forma, se houver uma queda significativa na demanda, os recursos implantados poderão ser reduzidos horizontalmente (de maneira automática ou manual).

### Confiabilidade

- Devido ao design descentralizado, a nuvem naturalmente dá suporte a uma infraestrutura confiável e resiliente.
- Com um design descentralizado, a nuvem permite que você tenha recursos implantados em várias regiões do mundo
- Com essa escala global, mesmo que ocorra um evento catastrófico em uma região, as outras regiões ainda estarão em funcionamento.

### Previsibilidade

- A previsibilidade na nuvem permite que você avance com confiança, seja no desempenho ou no custo. Ambas são influenciadas pelo Microsoft Azure Well-Architected Framework

### Segurança

- A nuvem oferece ferramentas de segurança que atendam às necessidades dos clientes mas, é importante lembrar que a implementação de muitas delas devem ser realizadas pelo cliente.
- Se você quiser o controle máximo da segurança, a infraestrutura como serviço fornecerá recursos físicos, mas permitirá que você gerencie os sistemas operacionais e o software instalado, incluindo aplicação de patches e manutenção
- Se você quiser a aplicação de patches e a manutenção sejam tratadas automaticamente, as implementações de plataforma como serviço ou software como serviço podem ser as melhores estratégias de nuvem para você.

### Governança

- A auditoria baseada em nuvem ajuda a sinalizar qualquer recurso que esteja fora de conformidade com seus padrões corporativos e fornece estratégias de mitigação.
- Dependendo do seu modelo operacional, patches de software e atualizações também podem ser aplicados automaticamente, o que ajuda na governança e na segurança.
- Ao estabelecer uma presença de governança o mais cedo possível, você poderá manter sua presença de nuvem atualizada, protegida e bem gerenciada.

### Gerenciabilidade

- Um dos principais benefícios da computação em nuvem são as opções de capacidade de gerenciamento. Há dois tipos de capacidade de gerenciamento para computação em nuvem que você aprenderá nesta série e ambos trazem excelentes benefícios.

**O gerenciamento da nuvem diz respeito a gerenciar seus recursos de nuvem. Por exemplo:**

- Escalar automaticamente a implantação de recursos com base na necessidade.
- Implantar recursos com base em um modelo pré-configurado, removendo a necessidade de configuração manual.
- O gerenciamento na nuvem diz respeito à maneira de gerenciar seu ambiente de nuvem e seus recursos por exemplo:
    - Por meio de um portal da Web.
    - Usando uma interface de linha de comando.
    - Usando APIs.
    - Usando o PowerShell.

# Tipos de Serviço de Nuvem na Azure

## IaaS (Infraestrutura como Serviço)

- Crie uma infraestrutura de TI de pagamento conforme o uso alugando servidores, máquinas virtuais, armazenamento, redes e sistemas operacionais de um provedor de nuvem.

## PaaS Plataforma como Serviço)

- Fornece um ambiente para a criação, o teste e a implementação de aplicativos de software, sem focar no gerenciamento da infraestrutura subjacente.

## SaaS (Software como Serviço)

- Os usuários se conectam e usam aplicativos com base em nuvem pela Internet: por exemplo, Microsoft Office 365, e-mail e calendários.

## Modelo de Responsabilidade Compartilhada

- **IaaS**
    - O serviço de nuvem mais flexível.
    - Você configura e gerencia o hardware para seu aplicativo.
- **PaaS**
    - Focado no desenvolvimento de aplicativos.
    - O gerenciamento de plataforma é realizado pelo provedor de nuvem.
- **SaaS**
    - Modelo de preço de pagamento conforme o uso.
    - Os usuários pagam pelo software que utilizam em um modelo de assinatura.

# Componentes de Arquitetura do Azure

### Contas do Azure

- Conta do Azure
- Conta gratuita do Azure
- Conta de estudante gratuita do Azure
- Área restrita do Microsoft Learn

## Regiões


- O Azure oferece mais regiões globais do que qualquer outro provedor de nuvem, com mais de 60 regiões representando mais de 140 países.
- As regiões são compostas de um ou mais datacenters muito próximos.
- Eles fornecem flexibilidade e escala para reduzir a latência do cliente.
- As regiões preservam a residência dos dados com uma oferta abrangente de conformidade.

## Zonas de Disponibilidade

- Fornece proteção contra tempo de inatividade devido a falha do datacenter.
- Separe fisicamente os datacenters dentro da mesma região
- Cada datacenter é equipado com alimentação, resfriamento e rede independentes
- Conectadas por meio de redes privadas de fibra óptica.

## Pares de Regiões

- No mínimo 300 milhas de separação entre pares de regiões.
- Replicação automática para alguns serviços.
- Recuperação de região priorizada em caso de interrupção.
- As atualizações são distribuídas sequencialmente para minimizar o tempo de inatividade.

## Regiões soberanas do Azure

### Serviços Governamentais dos EUA

- Atende às necessidades de segurança e conformidade das agências federais, governos estaduais e locais dos EUA e seus provedores de soluções.

### Azure Governamental:

- Instância separada do Azure.
- Fisicamente isolada de implantações que não sejam do governo dos EUA
- Acessível somente a pessoal verificado e autorizado.

### Azure China:

- A Microsoft é o primeiro provedor estrangeiro de serviços de nuvem pública da China, em conformidade com as regulamentações governamentais.

### Recursos do Azure China:

- Instância fisicamente separada dos serviços de nuvem do Azure operados pela 21Vianet.
- Todos os dados permanecem dentro da China para garantir a conformidade.

## Recursos do Azure

Os recursos do Azure são componentes como armazenamento, máquinas virtuais e redes que estão disponíveis para criar soluções de nuvem.

### Grupos de recursos

- Um grupo de recurso é um contêiner que você usa para gerenciar e agregar recursos em uma única unidade.
- Os recursos podem existir em apenas um grupo de recursos.
- Os recursos podem existir em diferentes regiões.
- Os recursos podem ser movidos para diferentes grupos de recursos.
- Os aplicativos podem utilizar vários grupos de recursos.

## Assinaturas do Azure

- Uma assinatura do Azure fornece a você acesso autenticado e autorizado às contas do Azure.
- **Limite de cobrança:**
    - gere relatórios de cobrança e faturas separados para cada assinatura.
- **Limite do controle de acesso:**
    - gerenciar e controlar o acesso aos recursos que os usuários podem provisionar com assinaturas específicas.

## Grupos de Gerenciamento


- Os grupos de gerenciamento podem incluir várias assinaturas do Azure.
- As assinaturas herdam as condições aplicadas ao grupo de gerenciamento.

  
