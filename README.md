# Script---Doorman
Este script previne vazamento acidental de PII (Informação Pessoal Identificável), mas não substitui uma DLP corporativa.

prompt_guard.py
Script Python para prevenir vazamento acidental de PII (Informação Pessoal Identificável) antes de colar textos em ferramentas externas, como chats de IA, formulários ou e-mails.

⚠️ Este script é uma camada de prevenção leve e não substitui uma solução DLP (Data Loss Prevention) corporativa.

Limitações conhecidas

Não valida CPF/CNPJ matematicamente, apenas detecta o padrão numérico
O padrão de CNPJ cobre apenas filial 0001 (matriz)
Não cobre todos os formatos de chave de API do mercado
Não processa imagens, PDFs ou arquivos binários
Não substitui ferramentas DLP corporativas como Symantec DLP, Microsoft Purview, etc.

Requisitos

Python 3.6+
Nenhuma dependência externa (usa apenas re da biblioteca padrão)


### 1. Por que Regex e não um LLM para limpar?
- *Custo Zero:* Não consome tokens da API;
- *Latência Zero:* A limpeza é instantânea;
- Offline First;
### 2. Por que Python?
- *Portabilidade:* Roda em qualquer terminal (Windows/Linux/Mac) sem compilar;
- *Legibilidade:* Facilita a auditoria do código por outros devs (eles podem ver exatamente o que o Regex está fazendo);


























