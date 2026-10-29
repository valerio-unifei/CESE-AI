## Ementa do Curso Avançado: Agentes de IA, Governança e LLMs em Sistemas Elétricos de Potência (SEP)

**Público-Alvo:** Engenheiros, pesquisadores e profissionais do setor elétrico que concluíram a formação técnica/avançada em Análise, Economia, Transmissão e Geração em SEP.

**Pré-requisitos:** Domínio prévio dos conceitos de fluxo de potência, estabilidade, proteção, operação e regulação de energia, além de conhecimento intermediário de programação em Python.

**Objetivo Geral:** Capacitar o profissional a projetar, implementar e implantar agentes autônomos e ecossistemas multiagentes seguros e auditáveis baseados em LLMs, integrando-os de forma interoperável a softwares de simulação elétrica, SCADA/EMS, barramentos de dados regulatórios e registradores operacionais, sob rígidos protocolos de guardrails, privacidade de dados de infraestrutura crítica e rastreabilidade.

---

### Módulo 1: Fundamentos de Arquiteturas de Agentes e LLMs para Engenharia

* **Engenharia de Prompts e Saídas Estruturadas:** Formatação e validação rigorosa de saídas (JSON, Pydantic) para garantir determinismo e interpretação exata de parâmetros de engenharia.
* **Tool Use e Function Calling:** Conexão de LLMs a motores de cálculo elétrico, APIs de campo e bancos de dados relacionais e vetoriais.
* **Padrões de Raciocínio Agêntico:** Arquiteturas *ReAct*, *Plan-and-Solve*, memória operacional, auto-reflexão, correção autônoma de código e tratamento de exceções em tempo de execução.
* **Frameworks e Orquestração:** Desenvolvimento prático com LangChain, LangGraph, LlamaIndex, CrewAI e AutoGen focados em problemas de energia.

---

### Módulo 2: Interoperabilidade e Integração com Sistemas Elétricos Legados

* **Padrões de Dados do Setor Elétrico:** Interoperabilidade baseada no Modelo de Informação Comum — CIM (*Common Information Model* / IEC 61970, IEC 61968) e padronização IEC 61850 em subestações.


* **Protocolos de Comunicação Inter-Agentes e Ferramentas:** Implementação do *Model Context Protocol* (MCP), REST/gRPC e barramentos de mensagens (Kafka, MQTT) para comunicação entre agentes e ecossistemas legados.
* **Gateways Agênticos para SCADA/EMS e GIS:** Arquiteturas de integração segura de agentes com sistemas de gerenciamento de energia (EMS), sistemas de distribuição (DMS) e geoprocessamento sem comprometer a operação em tempo real.



---

### Módulo 3: Guardrails, Dados Sigilosos e Segurança Cibernética

* **Mecanismos de Guardrails e Segurança Elétrica:** Implementação de barreiras de validação (NeMo Guardrails, Llama Guard, regras determinísticas) para impedir que agentes gerem comandos operacionais violares ou semanticamente inválidos.
* **Proteção de Infraestrutura Crítica e Dados Sigilosos:** Adequação à LGPD, conformidade com normas de segurança cibernética da infraestrutura de energia (NERC CIP / diretrizes ONS) e técnicas de anonimização/mascaramento de topologias de rede, PII e segredos industriais.
* **Prevenção de Ataques e Vazamentos:** Mitigação de riscos de *Prompt Injection*, vazamento de dados via chamadas de API externas e estratégias de *deployment* privado e local (Ollama, vLLM, Azure Confidential Computing).

---

### Módulo 4: Agentes para Análise, Operação e Centros de Controle

* **Orquestração de Simulações de Redes:** Agentes para montagem automática de casos, execução e convergência de fluxo de potência e curto-circuito em simuladores abertos e comerciais (OpenDSS, PyPSA, ANAREDE/ANAFAS).


* **Análise de Contingências $N-1/N-2$ com Guardrails:** Automação de varredura de contingências, ranqueamento de severidade e geração de pareceres explicativos sob restrições estritas de operação.


* **Copilotos de Operação em Linguagem Natural:** Assistentes agênticos para interface de linguagem natural com SCADA/EMS, consulta rápida a alarmes operacionais e navegação em manuais dos centros de controle (ONS e concessionárias).



---

### Módulo 5: Agentes RAG, Auditoria e Explicabilidade em Mercado e Regulação

* **Arquiteturas RAG Híbridas Especializadas:** Chunking inteligente e busca semântica em acervos regulatórios extensos (Procedimentos de Rede, Resoluções ANEEL e Regras CCEE).


* **Auditoria e Trilha de Rastreabilidade (*Audit Trail*):** Registro auditável e imutável do processo de raciocínio (*Chain-of-Thought*) e das tomadas de decisão dos agentes em transações financeiras e pareceres regulatórios.
* **Agentes para Contratos, Leilões e Risco:** Automação de verificação de conformidade em enquadramento tarifário (TUST/TUSD), análise de riscos em derivativos e negociação assistida no Mercado Livre (ACL) e Regulado (ACR).



---

### Módulo 6: Agentes para Proteção, Oscilografia, QEE e Subestações

* **Diagnóstico Autônomo e Explicável de Perturbações:** Agentes leitores de arquivos COMTRADE para análise automática de oscilografia e verificação de atuação de relés (funções 50, 51, 21, 87, etc.) com emissão de laudo auditável.


* **Validação de Configurações IEC 61850:** Agentes para verificação de arquivos SCL/SCD, diagnóstico de consistência de mensagens GOOSE/SV e conformidade com esquemas de proteção.


* **Análise de QEE e PRODIST:** Classificação automatizada de distúrbios de Qualidade da Energia Elétrica (afundamentos, harmônicos) e geração de relatórios regulatórios de conformidade.



---

### Módulo 7: Ecossistemas Multiagentes em Estabilidade, Controle e Renováveis

* **Sistemas Multiagentes (MAS) Descentralizados:** Coordenação e negociação entre agentes para sintonia adaptativa de PSS, AVR e conversores em redes com alta penetração de renováveis.


* **Gestão Agêntica de Usinas Híbridas e BESS:** Tomada de decisão em tempo real para otimização de despacho (Solar + Eólica + BESS) e gerenciamento de microredes.
* **Modelos Preditivos de Demanda e Clima:** Integração de agentes a modelos estatísticos e estatística bayesiana para previsão multivariada de geração sob incertezas climáticas.



---

### Módulo 8: Projeto Integrador (*Capstone*) e Validação Industrial

* **Desenvolvimento End-to-End com Foco Industrial:** Implementação de uma solução agêntica completa voltada a um problema real do setor (ex.: Assistente Operacional de Subestação com Guardrails, Agente Auditor Regulatório ANEEL/CCEE com Trilha de Auditoria, ou Diagnosticador de Falhas por COMTRADE).
* **Avaliação de Confiabilidade e Benchmarking:** Aplicação de frameworks de avaliação de agentes (LLM-as-a-Judge, Ragas), métricas de latência, taxa de alucinação, análise de impacto de segurança cibernética e validação técnica em ambiente simulado.