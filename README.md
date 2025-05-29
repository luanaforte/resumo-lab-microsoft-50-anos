# Laboratório DIO - Microsoft Azure

Este README abrange os fundamentos da plataforma Azure, comparando modelos de nuvem, explorando os benefícios da nuvem, e detalhando os principais serviços e componentes de arquitetura do Azure.

---

## Fundamentos da Plataforma Azure

### Fundamentos da Plataforma de Aplicação Azure
* **Componentes de Arquitetura**: Regiões, zonas de disponibilidade, assinaturas e grupos de recursos.
* **Computação e Rede**: Tipos de computação, hospedagem de aplicativos, redes virtuais.
* **Armazenamento**: Serviços de armazenamento, opções de redundância, gerenciamento e migração de arquivos.

---

## Comparação de Modelos em Nuvem

### Nuvem Pública
* **Acessibilidade**: Serviços disponíveis para o público via internet.
* **Infraestrutura Compartilhada**: Recursos computacionais são compartilhados entre múltiplos usuários.
* **Baixo Custo Inicial**: Não exige grandes investimentos em hardware próprio.

### Nuvem Privada
* **Infraestrutura Dedicada**: Recursos exclusivos para uma única organização.
* **Maior Controle**: Mais controle sobre a segurança e personalização do ambiente.
* **Custo Elevado Inicial**: Demanda alto investimento em hardware e manutenção.

### Nuvem Híbrida
* **Combinação Flexível**: Integra nuvens pública e privada.
* **Flexibilidade**: Permite mover cargas de trabalho entre ambientes.
* **Otimização de Custos**: Utilize a nuvem pública para escalabilidade e a privada para dados sensíveis.

---

## Comparar CAPEX e OPEX

### Despesas de Capital (CAPEX)
* **Investimento Inicial**: Gastos com a compra de ativos físicos, como servidores e infraestrutura.
* **Amortização**: O custo é amortizado ao longo do tempo.

### Despesas Operacionais (OPEX)
* **Custos Recorrentes**: Despesas contínuas para operar um negócio, como aluguel de servidores e serviços.
* **Dedução Imediata**: Os custos podem ser deduzidos no mesmo ano fiscal.

---

## Benefícios da Nuvem

* **Alta Disponibilidade**: Garante que os aplicativos e serviços estejam sempre funcionando, mesmo em caso de falhas.
* **Escalabilidade**: Capacidade de aumentar ou diminuir recursos de forma rápida para atender à demanda.
* **Previsibilidade**: Ajuda a estimar e controlar os custos operacionais da infraestrutura.
* **Governança**: Facilita o controle e a conformidade com políticas e regulamentações.
* **Elasticidade**: Capacidade de aumentar e diminuir a capacidade automaticamente conforme a demanda flutua.
* **Confiabilidade**: Oferece sistemas robustos e resilientes que funcionam sem falhas inesperadas.
* **Segurança**: Protege dados, aplicativos e infraestrutura contra ameaças cibernéticas.
* **Gerenciabilidade**: Simplifica a administração e o monitoramento dos recursos de TI.

---

## Modelos de Serviço em Nuvem

* **IaaS - Infraestrutura**: Oferece controle sobre o sistema operacional, redes e armazenamento. Ideal para migração de máquinas virtuais (VMs) e desenvolvimento de aplicações.
* **PaaS - Plataforma**: Fornece um ambiente completo para desenvolver, executar e gerenciar aplicativos sem se preocupar com a infraestrutura subjacente. Ideal para desenvolvedores que querem focar no código.
* **SaaS - Software**: O software é entregue via internet, sem necessidade de instalação ou manutenção. Ideal para usuários finais que precisam de uma solução pronta para uso (ex: e-mail, CRM).

---

## Componentes de Arquitetura do Azure

* **Regiões**: Locais geográficos que contêm um ou mais datacenters do Azure, oferecendo proximidade para usuários e conformidade com regulamentações.
* **Zonas de Disponibilidade**: Datacenters fisicamente separados dentro de uma região, cada um com energia, refrigeração e rede independentes, protegendo contra falhas de datacenter único.
* **Pares de Regiões**: Duas regiões do Azure que estão emparelhadas logicamente dentro da mesma geografia, garantindo recuperação de desastres e alta disponibilidade.
* **Regiões Soberanas (EUA e China) e Recursos do Azure**: Regiões projetadas para atender requisitos específicos de residência de dados e conformidade para governos e setores altamente regulamentados.
* **Assinaturas do Azure e Grupos de Gerenciamento**: Assinaturas organizam recursos para fins de cobrança e controle de acesso, enquanto grupos de gerenciamento permitem aplicar políticas e conformidade em várias assinaturas.

---

## Grupos de Recursos

Um grupo de recursos é um contêiner que você usa para agregar recursos em uma única unidade.

* **Implantação de Recursos**: Todos os recursos necessários para um aplicativo (VMs, bancos de dados, redes) podem ser implantados juntos.
* **Gerenciamento Unificado**: Facilita o gerenciamento do ciclo de vida dos recursos, permitindo que sejam monitorados, atualizados e excluídos em conjunto.
* **Controle de Acesso**: Permite aplicar permissões e políticas de controle de acesso (RBAC) em um conjunto de recursos.
* **Visualização e Análise**: Fornece uma visão consolidada de todos os recursos pertencentes a um projeto ou aplicação específica.

---

## Assinaturas do Azure

* **Limites de Cobrança**: Define a unidade de cobrança para os serviços do Azure que você consome. Tudo o que você usa dentro de uma assinatura será cobrado nela.
* **Limite do Controle de Acesso**: Serve como um limite de segurança e controle de acesso, onde permissões e políticas são aplicadas para governar quem pode acessar e gerenciar os recursos.

---

## Grupos de Gerenciamento

* **Hierarquia Organizacional**: Permitem criar uma hierarquia para organizar suas assinaturas.
* **Aplicação de Políticas**: Facilitam a aplicação de políticas e conformidade em várias assinaturas.
* **Controle de Acesso Consolidado**: Permitem definir permissões e controle de acesso em um nível superior.
* **Gerenciamento Centralizado**: Oferecem uma forma centralizada de governar e gerenciar um grande número de assinaturas.
* **Conformidade Abrangente**: Ajudam a garantir a conformidade com regulamentações em toda a organização.

---

## Serviços de Contêineres do Azure

Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.

* **Instância de Contêineres (ACI)**: Ideal para hospedar contêineres isolados que não exigem orquestração complexa.
* **Aplicativos de Contêiner do Azure (ACA)**: Plataforma para construir e implantar microsserviços e aplicativos baseados em contêineres com recursos de dimensionamento e tráfego.
* **Serviços de Kubernetes do Azure (AKS)**: Um serviço gerenciado de Kubernetes para orquestração de contêineres em grande escala.
* **Azure Functions**: Serviço de computação serverless que permite executar código em resposta a eventos sem gerenciar a infraestrutura.

---

## Serviços de Aplicativo do Azure

Os serviços de aplicativo do Azure consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos web e APIs rapidamente.

---

## Armazenamento do Azure

* **Domínio de Objetivo**: O tipo de armazenamento é escolhido com base no objetivo dos dados: blobs para objetos, discos para VMs, arquivos para compartilhamentos de rede.
* **Redundância de Armazenamento**: Opções como LRS, ZRS, GRS e RA-GRS garantem que os dados estejam protegidos contra perdas em caso de falhas.
* **Serviço de Armazenamento do Azure e Ponto de Extremidade**: O Armazenamento do Azure é um serviço de armazenamento altamente escalável e durável que oferece diferentes tipos de armazenamento acessíveis via endpoints únicos.
* **Camadas de Acesso de Armazenamento do Azure**: Diferentes camadas (hot, cool, archive) permitem otimizar custos com base na frequência de acesso aos dados.
* **Azure Data Box**: Solução para transferir grandes volumes de dados de forma offline para o Azure.
