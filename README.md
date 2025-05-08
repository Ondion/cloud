# Azure - Material de Apoio para Estudos e Implementações

Este repositório tem como objetivo **documentar o uso prático dos serviços da Microsoft Azure**, com foco na **aplicação dos conceitos aprendidos**, **estruturação clara dos processos técnicos** e **acompanhamento de boas práticas**. Ele pode ser expandido com arquivos complementares como scripts, templates e imagens ilustrativas.

---

## 🧠 Conceitos Fundamentais da Azure

- **Azure é a plataforma de nuvem da Microsoft** que fornece serviços como IaaS, PaaS e SaaS.
- Os recursos na Azure são organizados em **Grupos de Recursos**.
- Tudo na Azure é gerenciado via **Portal**, **CLI**, **PowerShell** ou **ARM Templates**.
- Segurança, escalabilidade e alta disponibilidade são pilares dos serviços Azure.

---

## 📦 Estrutura de Estudo

Cada seção a seguir apresenta um tema estudado, seguido do processo técnico documentado e dicas práticas para implementações futuras.

---

## ☁️ Criação e Configuração de uma Máquina Virtual (VM)

### ✅ Objetivo
Criar uma máquina virtual Windows/Linux na Azure, configurando rede, regras de acesso e disco.

### 🔧 Etapas no Portal Azure

1. **Acesse o Portal Azure** (https://portal.azure.com).
2. Navegue até: `Máquinas Virtuais > Criar > Máquina Virtual`.
3. **Preencha as informações básicas**:
   - Assinatura, Grupo de Recursos
   - Nome da VM, Região e Imagem (ex: Ubuntu 20.04 LTS)
   - Tipo de autenticação: senha ou chave SSH

4. **Tamanho da VM**:
   - Escolha conforme a carga de trabalho (ex: B1s para testes).

5. **Discos**:
   - SSD padrão para melhor desempenho.
   - Habilitar criptografia se necessário.

6. **Rede**:
   - Criar uma nova VNet/Sub-rede ou usar existente.
   - Criar IP público e configurar regras de NSG (ex: permitir porta 22 para SSH).

7. **Revisar + Criar**:
   - Verifique as configurações e clique em “Criar”.

### 🧪 Testes Práticos

- Conexão via SSH:  
  `ssh usuario@ip_publico`
- Instalação de pacotes:  
  `sudo apt update && sudo apt install nginx`
