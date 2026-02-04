# EngApp

# EngApp: Gestão e Padronização de Protocolos

**EngApp** é uma solução corporativa desenvolvida para digitalizar, padronizar e validar fluxos técnicos e normas de segurança em projetos de infraestrutura. O sistema foca em garantir a integridade de dados e a conformidade rigorosa com Normas Regulamentadoras (NRs), eliminando a burocracia do papel e mitigando riscos jurídicos e operacionais.

## Sumário

* Visão Geral
* Roadmap de Desenvolvimento
* Stack Tecnológica
* Arquitetura de Dados
* Manual de Implantação
* Propriedade Intelectual

## Visão Geral

O EngApp foi concebido para resolver o gap de comunicação entre o canteiro de obras e o escritório técnico. Através de formulários inteligentes e validação em tempo real, o app assegura que protocolos de **NR-10, NR-18 e NR-35** sejam seguidos à risca antes do início de qualquer atividade de risco.

### Principais Diferenciais:

* **Checklists Inteligentes:** Bloqueio de processos em caso de não conformidade.
* **Relatórios Instantâneos:** Geração de ARTs e laudos em PDF com um clique.
* **Evidência Digital:** Registro fotográfico com metadados e geolocalização.

## Roadmap de Desenvolvimento

### Fase 1: Fundação & Core (Concluído)

* **Modelagem de Dados:** Estrutura relacional para protocolos, usuários e normas.
* **RBAC (Role-Based Access Control):** Níveis de acesso distintos para Engenheiros, Técnicos e Auditores.
* **CRUD de Campo:** Registro dinâmico de vistorias e atividades.

### Fase 2: Automação e NRs (Em desenvolvimento)

* **Engine de Validação:** Lógica programática para conformidade automática com NR-10, NR-18 e NR-35.
* **Módulo ReportLab:** Geração de PDFs profissionais com gráficos e assinaturas digitais.
* **Mídia:** Compressão automática de fotos para economia de banda em campo.

### Fase 3: Inteligência de Negócio

* **Dashboards (BI):** KPIs de segurança e produtividade via interface web.
* **Geo-Fencing:** Validação de presença em obra via GPS.
* **Ecossistema:** API REST para integração com softwares BIM e ERPs de mercado.

### Fase 4: Resiliência e Mobilidade

* **Offline First:** Sincronização de dados para obras em locais remotos.
* **UI Industrial:** Interface adaptada para alta luminosidade e uso com equipamentos de proteção (EPIs).

## Stack Tecnológica

| Camada         | Tecnologia   | Justificativa Técnica.
| **Linguagem**  | Python 3.12+ | Estabilidade e vasto ecossistema de análise de dados. 
| **Framework**  | Django       | ORM potente para gerir a complexidade das normas técnicas. 
| **Dados**      | Pandas       | Processamento de grandes volumes de dados de conformidade. 
| **Relatórios** | ReportLab    | Precisão milimétrica na geração de documentos técnicos. 
| **Frontend**   | Tailwind CSS | Estilização ágil e responsiva para tablets e smartphones. 

## Manual de Implantação (Guia Rápido)

Este guia é destinado a desenvolvedores e administradores de sistema.

### 1. Pré-requisitos

* Python 3.12 ou superior
* PostgreSQL (Recomendado para produção)
* Virtualenv ou Docker

### 2. Configuração do Ambiente

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/engapp.git
cd engapp

# Crie o ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Instale as dependências
pip install -r requirements.txt

```

### 3. Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
DEBUG=True
SECRET_KEY=sua_chave_secreta
DB_NAME=engapp_db
DB_USER=seu_usuario
DB_PASSWORD=sua_senha

```

### 4. Inicialização do Banco

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser  # Para acessar o painel administrativo

```

### 5. Execução

```bash
python manage.py runserver

```

Acesse `http://127.0.0.1:8000` para visualizar a aplicação.

---

## Licença e Propriedade

**Copyright © 2026 KM PROJETOS.**

Este software é um produto proprietário. O código-fonte, design e metodologias aplicadas são de propriedade exclusiva da **KM PROJETOS**.

* **Desenvolvedor Responsável:** Márcio Rodrigues de Oliveira (Engenheiro de Software e Civil).
* **Restrições:** A reprodução, distribuição ou uso comercial sem autorização expressa e por escrito do detentor dos direitos é estritamente proibida e sujeita a penalidades legais.

