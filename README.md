# Desafio de Documentação - Bootcamp Santander Code Girls

### Anotações sobre Módulos 1 e 2 - Computação em Nuvem AWS

Este projeto é a documentação do aprendizado adquirido nos módulos iniciais do Bootcamp Santander Code Girls, com foco nos conceitos fundamentais da AWS e no serviço de computação EC2.

O objetivo é consolidar o conhecimento sobre a infraestrutura em nuvem, o gerenciamento de recursos e as melhores práticas de custo e segurança, servindo como material de estudo e referência futura.

---

## 1. Módulo 1: Introdução à AWS e Conceitos Básicos

### A AWS e a Computação em Nuvem
A Amazon Web Services (AWS) é a plataforma de nuvem mais segura, abrangente e confiável do mercado, oferecendo uma infraestrutura global escalável e flexível. O modelo de negócio **OPEX** (custo operacional) permite que clientes paguem apenas pelos recursos que consomem, eliminando a necessidade de investimento inicial (CAPEX) em hardware.

### Infraestrutura Global
* **Regions:** Áreas geográficas isoladas que garantem alta tolerância a falhas.
* **Availability Zones (AZs):** Data centers dentro das *regions*, conectados por fibra de alta velocidade, com no mínimo duas AZs por *region* no Brasil.
* **Fatores para escolha de uma *region*:** Compliance, disponibilidade de serviços, custo e latência.

### Modelos de Serviço em Nuvem
A AWS se encaixa em três modelos de serviço, dependendo do nível de gerenciamento e responsabilidade:
* **IaaS (Infrastructure as a Service):** A AWS fornece a infraestrutura (servidores, redes), e o cliente gerencia o sistema operacional e as aplicações. (Ex: EC2)
* **PaaS (Platform as a Service):** A AWS gerencia a infraestrutura e o sistema operacional, e o cliente foca apenas em sua aplicação.
* **SaaS (Software as a Service):** O software completo é fornecido e gerenciado pela AWS.

### Segurança e Controle de Custos
* **IAM (Identity and Access Management):** Ferramenta central para gerenciar usuários, grupos e permissões, garantindo uma *governance* segura na plataforma.
* **MFA (Multi-Factor Authentication):** Essencial para proteger a conta **root**.
* **Alertas de Custo:** Ferramenta importante para monitorar e controlar o consumo de recursos e evitar surpresas na fatura.

---

## 2. Módulo 2: Computação na Nuvem com EC2

### Instâncias EC2 (Elastic Compute Cloud)
As instâncias EC2 são as máquinas virtuais da AWS. Elas são a base do modelo **IaaS**, onde a AWS é responsável pela infraestrutura física e o cliente pela configuração e uso da máquina.

* **Responsabilidade Compartilhada:** A AWS garante a infraestrutura, mas a segurança e configuração do que roda na instância são responsabilidade do cliente.
* **Tipos de Instâncias:** Categorias de instâncias (ex: `t2.micro`, `m5.large`) que oferecem diferentes capacidades de CPU, memória e armazenamento para cada tipo de carga de trabalho.
* **Otimização de Custos:**
    * **Escala (Scale Up/Down):** Aumentar ou diminuir o poder de uma instância (**vertical**) ou o número de instâncias (**horizontal**) para lidar com variações de tráfego e carga.
    * **Modelos de Pagamento:** **On-demand** (pagar por hora), **reservadas** (comprometimento de longo prazo com desconto) e **spot** (instâncias não usadas com grandes descontos, mas que podem ser interrompidas).

### Armazenamento na Nuvem
* **Amazon EBS (Elastic Block Store):** Volumes de armazenamento persistentes (como HDs virtuais) que podem ser anexados e desanexados de instâncias EC2. É ideal para sistemas de arquivos e bancos de dados.
    * **Snapshots:** Cópias pontuais do seu volume EBS, ideais para backup e recuperação de dados.
* **Amazon S3 (Simple Storage Service):** Serviço de armazenamento de objetos, usado para grandes volumes de dados não estruturados (fotos, vídeos, backups).
    * **Classes de Armazenamento:** Diferentes classes (Standard, Glacier, etc.) com diferentes custos e tempos de acesso, permitindo otimizar despesas.

### Gerenciamento Avançado com AMI
* **AMI (Amazon Machine Image):** Uma "imagem" da sua instância EC2 pré-configurada. Permite criar rapidamente novas instâncias idênticas, garantindo a consistência do ambiente.
* **Diferença entre AMI e Snapshot:** A **AMI** é um backup completo do servidor, incluindo o sistema operacional e todos os volumes anexados. O **Snapshot** é uma cópia **pontual** e de apenas um volume EBS específico.

---

### Conclusão

Este desafio foi crucial para solidificar os conhecimentos teóricos em uma base prática. A exploração de serviços como **EC2**, **EBS** e **S3** me proporcionou uma visão clara de como a arquitetura em nuvem é construída, desde os conceitos de infraestrutura global até o gerenciamento diário de recursos.

Agradeço a oportunidade de aprofundar meus estudos na AWS e estou animada para aplicar esses conhecimentos em futuros projetos.
