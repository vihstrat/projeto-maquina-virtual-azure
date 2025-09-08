# Desafio de Máquina Virtual Azure

## 📝 Descrição do Projeto

Este projeto foi desenvolvido como parte de um desafio para consolidar conhecimentos em máquinas virtuais na **Azure**. O objetivo principal foi aplicar os conceitos aprendidos na prática, criando e configurando uma máquina virtual do Windows no portal do Azure.

Este repositório serve como uma documentação técnica e um registro detalhado de todas as etapas, desde o planejamento inicial até a verificação do funcionamento da VM.

## 🎯 Objetivos de Aprendizagem

* **Aplicar conceitos:** Criar e gerenciar recursos na nuvem Azure, focando em máquinas virtuais.
* **Documentar processos:** Registrar de forma clara e estruturada todo o fluxo de trabalho.
* **Utilizar o GitHub:** Usar o GitHub como uma ferramenta para hospedar e compartilhar a documentação técnica do projeto.

---

## 🛠️ Tecnologias Utilizadas

* **Microsoft Azure:** Para a criação e gestão da máquina virtual.
* **GitHub:** Para versionamento e documentação do projeto.
* **Windows:** Sistema operacional da máquina virtual criada.
* **Protocolo de Área de Trabalho Remota (RDP):** Para acesso à VM.

---

## 📋 Etapas do Projeto

Aqui estão os passos detalhados para a criação da máquina virtual, incluindo as decisões e configurações realizadas em cada etapa.

### 1. **Criação da Máquina Virtual (VM)**

* **Serviço:** Acesso ao portal do Azure e seleção do serviço "Máquinas Virtuais".
* **Configurações Básicas:**
    * **Assinatura:** [Nome da sua assinatura do Azure]
    * **Grupo de Recursos:** [Nome do grupo de recursos que você criou, por exemplo, `rg-desafio-vm`]
    * **Nome da VM:** [Nome da sua VM, por exemplo, `vm-desafio-windows`]
    * **Região:** [Região escolhida, por exemplo, `Brazil South`]
    * **Opções de Imagem:** `Windows Server` [Versão específica, por exemplo, `Windows Server 2022 Datacenter`]
    * **Tamanho:** [Tamanho da VM, por exemplo, `Standard_B1s`]. Explique brevemente por que você escolheu esse tamanho (custo, requisitos mínimos).
* **Credenciais do Administrador:** Definição do nome de usuário e senha para acesso à VM.

![Criação da VM - Configurações básicas](images/captura-de-tela-1.png)
*Uma captura de tela das configurações iniciais da VM.*

### 2. **Configuração de Rede**

* **Rede Virtual:** Criação de uma nova rede virtual ou uso de uma existente.
* **IP Público:** Atribuição de um endereço IP público para permitir o acesso externo.
* **Portas de Entrada:** Permissão da porta `3389` (RDP - Remote Desktop Protocol) para que seja possível se conectar à máquina virtual remotamente. **Nota:** Mencione a importância da segurança e de restringir o acesso a essa porta apenas a IPs específicos em um ambiente de produção.

![Configurações de rede](images/captura-de-tela-2.png)
*Visão geral das configurações de rede da VM.*

### 3. **Revisão e Criação**

* Análise do resumo de custos e configurações antes da criação final.
* Clique em `Revisar + criar` e, em seguida, em `Criar`.

### 4. **Conexão com a Máquina Virtual**

* Após a implantação, navegação para a página da VM no portal do Azure.
* Clique em `Conectar` e download do arquivo RDP.
* Uso do arquivo RDP para se conectar à VM, inserindo as credenciais de administrador definidas anteriormente.

![Conexão RDP](images/captura-de-tela-3.png)
*Demonstração do painel de conexão RDP.*

### 5. **Verificação do Funcionamento**

* Verificação do sistema operacional na área de trabalho da VM.
* Confirmação de que o acesso e a navegação estão funcionando conforme o esperado.

---

## 💡 Conclusão e Aprendizados

Este desafio me permitiu não apenas criar um recurso na Azure, mas também entender a importância de cada etapa: desde a escolha do tamanho da VM e da imagem até a configuração de segurança das portas de rede. A documentação do processo no GitHub foi essencial para organizar os aprendizados e ter um registro claro para futuras referências.

## 🔗 Recursos Úteis

* **Início Rápido: Criar uma máquina virtual do Windows no Portal do Azure** - [Artigo da Microsoft Learn](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)
