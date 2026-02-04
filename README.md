# EngApp

**App para Gestão e Padronização de Protocolos de Engenharia.**

Uma solução robusta para o registro, acompanhamento e validação de fluxos técnicos e normas de segurança, garantindo conformidade e integridade em projetos de infraestrutura.

**Roadmap de Desenvolvimento**

Esta seção apresenta as funcionalidades em implementação e o que está planejado para o futuro do projeto:

* [x] **Fase 1: Estrutura Base**
* [x] Modelagem do banco de dados para Protocolos e Normas.
* [x] Autenticação de usuários (Engenheiro, Técnico, Auditor).
* [x] CRUD básico de registros de campo.

* [ ] **Fase 2: Automação e NRs (Em desenvolvimento)**
* [ ] Implementação de lógica de validação para **NR-10, NR-18 e NR-35**.
* [ ] Motor de geração de relatórios PDF automatizados com `ReportLab`.
* [ ] Upload de evidências fotográficas com compressão automática.

* [ ] **Fase 3: Inteligência e Integração**
* [ ] Dashboard de indicadores de conformidade (KPIs de segurança).
* [ ] Integração de geolocalização para validação de presença em obra.
* [ ] API para exportação de dados para softwares de gestão (ERP/BIM).

* [ ] **Fase 4: Mobilidade Avançada**
* [ ] Sincronização offline para locais sem conectividade.
* [ ] Interface mobile responsiva otimizada para uso com luvas e em ambientes externos.

**Stack Tecnológica**

Linguagem: Python 3.12+

Framework Web: Django (ORM robusto para gestão de bancos de dados complexos de engenharia)

Processamento de Dados: Pandas (para análise de conformidade e métricas de obras)

Geração de Relatórios: ReportLab / WeasyPrint (automação de PDFs profissionais)

Interface de Usuário: Django Templates / Tailwind CSS (focado em usabilidade no canteiro de obras)

**Licença**

Este software é de propriedade da KM PROJETOS. O uso ou reprodução sem autorização do desenvolvedor Márcio Rodrigues de Oliveira é estritamente proibida.
