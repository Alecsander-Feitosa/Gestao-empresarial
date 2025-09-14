# 🏭 Gestão Framark - Sistema de Gestão de Produção

![Banner do Dashboard Principal](https://github.com/Alecsander-Feitosa/Gestao-empresarial/blob/main/fotos/Dashborad.png)


*[➡️ Acesse a demonstração ao vivo aqui!](https://gestao-empresax.onrender.com/login)*

---
### **Backend**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)

### **Frontend**
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

### **Banco de Dados & Infraestrutura**
![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)
![Google Drive](https://img.shields.io/badge/Google_Drive-4285F4?style=for-the-badge&logo=google-drive&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white)

### **Deploy**
![OnRender](https://img.shields.io/badge/OnRender-46E3B7?style=for-the-badge&logo=render&logoColor=white)


## 📄 Descrição

O **Gestão Framark** é um sistema ERP (Enterprise Resource Planning) completo, desenvolvido para digitalizar e otimizar o fluxo de produção de uma fábrica de produtos personalizados. A plataforma centraliza o controle de pedidos, desde a criação pelo designer (ou cliente) até a finalização, passando por todas as etapas de manufatura.

O projeto foi construído com o objetivo de resolver problemas reais como falta de comunicação entre setores, dificuldade no rastreamento de pedidos e falta de visibilidade do processo para o cliente final.

---

## ✨ Funcionalidades Principais

O sistema é dividido em dois portais principais, cada um com suas próprias funcionalidades:

### **Portal Interno (Funcionários)**
* **🔑 Autenticação e Permissões:** Login seguro para funcionários com diferentes níveis de acesso (Admin, Designer, Pintura, Laser, etc.), garantindo que cada usuário só possa gerenciar a sua etapa do processo.
* **📊 Dashboard Interativo:** Visualização de dados em tempo real com estatísticas de produção (total de pedidos, prontos, em produção, atrasados) e gráficos de pedidos por modelo e status.
* ** Kanban e Tabela:** Duas formas de visualizar os pedidos, permitindo alternar entre uma visão de fluxo de trabalho (Kanban) e uma visão detalhada em lista (Tabela).
* **📝 Gerenciamento Completo de Pedidos:** Funcionalidades de criar, editar e atualizar o status e sub-status de cada pedido.
* **☁️ Integração com Google Drive:** Upload de layouts (PDF) e fotos de confirmação de cada etapa diretamente para uma pasta no Google Drive, mantendo um histórico visual do processo.
* **📷 Captura de Foto via Webcam:** Ferramenta para tirar fotos diretamente pelo sistema para comprovar a finalização de uma etapa.

### **Portal do Cliente**
* **👤 Cadastro e Login de Clientes:** Clientes (empresas) podem se cadastrar e acessar um portal exclusivo para visualizar e gerenciar seus pedidos.
* **📈 Acompanhamento de Pedidos:** Visualização em um painel Kanban simplificado que mostra em qual etapa da produção cada um dos seus pedidos se encontra.
* **🆕 Criação de Novos Pedidos:** Clientes podem iniciar novos pedidos diretamente pelo portal, preenchendo detalhes, quantidade e fazendo o upload de arquivos de logo e layout.
* **👥 Gestão de Vendedores:** O cliente principal pode cadastrar sub-usuários (vendedores) para sua empresa, que também podem criar e acompanhar pedidos.

---

## 🛠️ Tecnologias Utilizadas

| Categoria | Tecnologia |
| :--- | :--- |
| **Backend** | Python, Flask, GSpread (API do Google Sheets) |
| **Frontend** | HTML5, CSS3, JavaScript (Vanilla), Tailwind CSS |
| **Banco de Dados** | Google Sheets (utilizado como sistema de banco de dados) |
| **Infraestrutura & APIs** | Google Drive API (para armazenamento de arquivos), Chart.js (gráficos) |
| **Segurança** | Passlib (para hashing de senhas) |
| **Deploy** | OnRender |

---

## 🚀 Como Testar a Aplicação Ao Vivo

A aplicação está hospedada na plataforma OnRender e pode ser testada diretamente pelo navegador. Existem dois portais principais, cada um com seu próprio método de acesso.

### **1. Portal Interno (Funcionários)**

Acesse a tela de login principal e utilize um dos perfis de teste abaixo para explorar as diferentes permissões e funcionalidades do sistema.

| Usuário | Senha | Perfil e Permissões |
| :--- | :--- | :--- |
| **`admin`** | `123456` | **Administrador:** Acesso total. Vê todos os pedidos e pode gerenciar todas as etapas. |
| **`designer`** | `123456` | **Entrada/Designer:** Pode criar novos pedidos e gerenciar a primeira etapa do fluxo. |
| **`separacao`** | `123456` | **Separação:** Gerencia a etapa de separação de peças. |
| **`pintura`** | `123456` | **Pintura:** Vê e gerencia apenas os pedidos que estão na etapa de pintura. |
| **`sublimacao`** | `123456` | **Sublimação:** Vê e gerencia apenas os pedidos na etapa de sublimação. |
| **`laser`** | `123456` | **Laser:** Vê e gerencia apenas os pedidos na etapa de corte a laser. |
| **`bordado`** | `123456` | **Bordado:** Vê e gerencia apenas os pedidos na etapa de bordado. |
| **`costura`** | `123456` | **Costura:** Gerencia a etapa de costura das peças. |
| **`finalizacao`**| `123456` | **Finalização:** Gerencia a última etapa antes do pedido ser finalizado. |

### **2. Portal do Cliente**

Para testar a visão do cliente, você pode:
1. Acessar a página de **login do cliente**.
2. Clicar em **"Cadastre-se aqui"** para criar uma nova conta de empresa.
3. Fazer login com a conta criada para acessar o dashboard do cliente, onde é possível criar e acompanhar pedidos.


**Status do Projeto: Versão de Portfólio (v1.0)**
A versão apresentada nesta demonstração (v1.0) representa um marco específico no desenvolvimento do projeto, 
servindo como uma vitrine de minhas habilidades e do conceito da aplicação.
O desenvolvimento ativo continuou, e versões posteriores incluem otimizações, 
melhorias de segurança e novas funcionalidades que não estão refletidas aqui.




## 👨‍💻 Autor

**Alecsander Silva Feitosa**

* **LinkedIn:** https://www.linkedin.com/in/alecsander-feitosa-800181347/
* **Email:** Alecsandersfr@gmail.com
