# 🕵️ OSINT-Awesome-Modern

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Stars](https://img.shields.io/github/stars/FTRep01/OSINT-Awesome-Modern?style=social)](https://github.com/FTRep01/OSINT-Awesome-Modern/stargazers)
[![Forks](https://img.shields.io/github/forks/FTRep01/OSINT-Awesome-Modern?style=social)](https://github.com/FTRep01/OSINT-Awesome-Modern/network/members)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-como-contribuir)
[![Last Commit](https://img.shields.io/github/last-commit/FTRep01/OSINT-Awesome-Modern)](https://github.com/FTRep01/OSINT-Awesome-Modern/commits/main)
[![Issues](https://img.shields.io/github/issues/FTRep01/OSINT-Awesome-Modern)](https://github.com/FTRep01/OSINT-Awesome-Modern/issues)
[![Made with Markdown](https://img.shields.io/badge/Made%20with-Markdown-1f425f.svg)](https://daringfireball.net/projects/markdown/)

Uma coleção curada e moderna de ferramentas de **OSINT (Open Source Intelligence)** voltada para profissionais de **Cibersegurança/Pentest**, **Investigações Privadas** e **Cyber Threat Intelligence (CTI)**.

O objetivo deste repositório é reunir, em um único lugar, ferramentas testadas e amplamente utilizadas pela comunidade — evitando listas genéricas e desatualizadas — com foco em aplicabilidade prática no dia a dia de Red Teams, investigadores e analistas de inteligência de ameaças.

---

## 📑 Sumário

1. [Introdução e Objetivo do Repositório](#-introdução-e-objetivo-do-repositório)
2. [Enumeração de Domínios e Infraestrutura (Foco Pentest/Red Team)](#-enumeração-de-domínios-e-infraestrutura-foco-pentestred-team)
3. [Investigação de Identidades e SOCMINT (Foco Privado/Pessoas)](#-investigação-de-identidades-e-socmint-foco-privadopessoas)
4. [Cyber Threat Intelligence (CTI) e Análise de Ameaças](#-cyber-threat-intelligence-cti-e-análise-de-ameaças)
5. [E-mails, Vazamentos e Credenciais](#-e-mails-vazamentos-e-credenciais)
6. [Ferramentas de Suporte e Análise de Dados (Canivetes Suíços)](#-ferramentas-de-suporte-e-análise-de-dados-canivetes-suíços)
7. [Como Contribuir](#-como-contribuir)

---

## 🎯 Introdução e Objetivo do Repositório

O **OSINT-Awesome-Modern** nasceu da necessidade de organizar, em uma estrutura clara e objetiva, as principais ferramentas de código aberto (e algumas gratuitas/freemium relevantes) usadas em fluxos de trabalho de:

- 🔓 **Pentest e Red Team** — reconhecimento ativo e passivo de superfície de ataque;
- 🔎 **Investigações Privadas** — verificação de identidade, background checks e SOCMINT;
- 🛡️ **Cyber Threat Intelligence** — atribuição de ameaças, análise de IOCs e monitoramento de atores maliciosos.

Cada ferramenta listada passa por um critério mínimo de relevância: manutenção ativa (ou robustez consolidada), adoção pela comunidade e valor prático comprovado em cenários reais.

> ⚠️ **Aviso legal:** As ferramentas aqui listadas devem ser utilizadas apenas em investigações legítimas, testes autorizados (com escopo definido) e em conformidade com a legislação aplicável (LGPD, GDPR, Computer Fraud and Abuse Act, etc.). O uso indevido é de responsabilidade exclusiva do usuário.

---

## 🌐 Enumeração de Domínios e Infraestrutura (Foco Pentest/Red Team)

Ferramentas para mapeamento de superfície de ataque, descoberta de subdomínios, ativos expostos e infraestrutura de rede.

- **[Amass](https://github.com/owasp-amass/amass)** 🕸️
  Projeto da OWASP para mapeamento de superfície de ataque via enumeração de subdomínios, coleta de ASN e correlação de infraestrutura em grafo de rede.

- **[Subfinder](https://github.com/projectdiscovery/subfinder)** ⚡
  Ferramenta rápida de enumeração passiva de subdomínios do ecossistema ProjectDiscovery, ideal para reconhecimento inicial em larga escala.

- **[Shodan](https://www.shodan.io/)** 🔌
  Motor de busca de dispositivos conectados à internet; essencial para identificar serviços expostos, banners e vulnerabilidades em infraestrutura pública.

- **[Censys](https://censys.io/)** 🔍
  Alternativa robusta ao Shodan, com indexação detalhada de certificados TLS/SSL e hosts, muito usada para pivoteamento de infraestrutura maliciosa.

- **[Nmap](https://github.com/nmap/nmap)** 🛰️
  Scanner de rede clássico e indispensável para descoberta de hosts, portas abertas, serviços e fingerprinting de sistemas operacionais.

- **[httpx](https://github.com/projectdiscovery/httpx)** 🌍
  Toolkit de sondagem HTTP multipropósito, usado para validar hosts ativos, capturar títulos, status codes e tecnologias em massa.

- **[Nuclei](https://github.com/projectdiscovery/nuclei)** 🎯
  Scanner de vulnerabilidades baseado em templates YAML, permitindo automação de testes de segurança contra grandes conjuntos de alvos.

- **[dnsx](https://github.com/projectdiscovery/dnsx)** 📡
  Ferramenta de resolução e enumeração de DNS de alta performance, útil para validar subdomínios descobertos e identificar registros relevantes.

- **[SecurityTrails](https://securitytrails.com/)** 🕰️
  Plataforma de inteligência de DNS histórico, indispensável para rastrear mudanças de infraestrutura e domínios associados a um alvo.

- **[FOFA](https://fofa.info/)** 🌏
  Motor de busca de ativos de internet com forte cobertura na Ásia, complementar ao Shodan/Censys em investigações globais.

---

## 🧑‍💻 Investigação de Identidades e SOCMINT (Foco Privado/Pessoas)

Ferramentas para verificação de identidade, rastreamento de perfis em redes sociais e correlação de dados pessoais.

- **[Sherlock](https://github.com/sherlock-project/sherlock)** 🔦
  Localiza contas de usuário associadas a um username em centenas de plataformas sociais simultaneamente — ponto de partida clássico em SOCMINT.

- **[Maltego](https://www.maltego.com/)** 🕷️
  Plataforma de análise de vínculos (link analysis) que transforma dados brutos em grafos visuais, essencial para correlacionar pessoas, domínios e organizações.

- **[Social-Analyzer](https://github.com/qeeqbox/social-analyzer)** 📊
  Ferramenta de análise e detecção de presença de uma pessoa em diversas plataformas, com módulos de análise textual e visual.

- **[SpiderFoot](https://github.com/smicallef/spiderfoot)** 🕸️
  Automação de reconhecimento OSINT que integra dezenas de fontes de dados, cobrindo tanto infraestrutura técnica quanto identidades.

- **[Google Dorks (GHDB)](https://www.exploit-db.com/google-hacking-database)** 🔎
  Banco de dados de operadores de busca avançados do Google, técnica fundamental para descoberta de informações expostas sobre pessoas e organizações.

- **[Pipl](https://pipl.com/)** 🪪
  Serviço especializado em busca de identidade profunda (deep identity search), amplamente utilizado por investigadores privados.

- **[IntelTechniques Search Tools](https://inteltechniques.com/tools/)** 🧰
  Conjunto de ferramentas e buscadores customizados criado por Michael Bazzell, referência mundial em investigações OSINT sobre pessoas.

- **[Osintgram](https://github.com/Datalux/Osintgram)** 📸
  Ferramenta de coleta de informações de perfis públicos do Instagram, útil para análise de comportamento e rede de contatos.

---

## 🛡️ Cyber Threat Intelligence (CTI) e Análise de Ameaças

Ferramentas para atribuição de ameaças, análise de malware, correlação de IOCs e monitoramento de atores maliciosos.

- **[MISP](https://github.com/MISP/MISP)** 🧩
  Plataforma open source de compartilhamento e correlação de indicadores de comprometimento (IOCs), padrão de mercado em times de CTI.

- **[VirusTotal](https://www.virustotal.com/)** 🦠
  Serviço de análise multi-engine de arquivos, hashes, URLs e domínios suspeitos — ferramenta base em qualquer triagem de ameaça.

- **[AlienVault OTX](https://otx.alienvault.com/)** 🌩️
  Plataforma colaborativa de threat intelligence com pulsos (pulses) compartilhados pela comunidade, ótima para contextualizar IOCs.

- **[YARA](https://github.com/VirusTotal/yara)** 🧵
  Motor de criação de assinaturas para identificação e classificação de malware, amplamente usado em caça a ameaças (threat hunting).

- **[MITRE ATT&CK Navigator](https://github.com/mitre-attack/attack-navigator)** 🗺️
  Ferramenta visual para mapear táticas, técnicas e procedimentos (TTPs) de atores de ameaça segundo a matriz MITRE ATT&CK.

- **[Cortex (TheHive Project)](https://github.com/TheHive-Project/Cortex)** ⚙️
  Motor de análise e enriquecimento automatizado de observáveis, integrado ao TheHive para resposta a incidentes e CTI.

- **[TheHive](https://github.com/TheHive-Project/TheHive)** 🐝
  Plataforma open source de resposta a incidentes de segurança, projetada para trabalhar em conjunto com MISP e Cortex.

- **[urlscan.io](https://urlscan.io/)** 🖥️
  Serviço de escaneamento e sandboxing de URLs suspeitas, gerando screenshots e análise de comportamento de páginas maliciosas.

- **[abuse.ch (URLhaus / ThreatFox)](https://abuse.ch/)** 🚨
  Conjunto de feeds públicos de IOCs mantidos pela comunidade, cobrindo malware, botnets e infraestrutura maliciosa ativa.

---

## 📧 E-mails, Vazamentos e Credenciais

Ferramentas para verificação de exposição de e-mails, credenciais vazadas e enumeração de contas corporativas.

- **[Have I Been Pwned](https://haveibeenpwned.com/)** 💥
  Referência mundial para verificar se um e-mail ou domínio foi exposto em vazamentos de dados conhecidos.

- **[theHarvester](https://github.com/laramies/theHarvester)** 📬
  Ferramenta clássica de coleta de e-mails, subdomínios, hosts e nomes de funcionários a partir de fontes públicas.

- **[Holehe](https://github.com/megadose/holehe)** ✉️
  Verifica se um e-mail está associado a contas em dezenas de serviços online, sem necessidade de acesso à conta.

- **[DeHashed](https://www.dehashed.com/)** 🗝️
  Plataforma de busca em bases de dados vazadas, muito utilizada para investigar credenciais comprometidas em breaches.

- **[LeakCheck](https://leakcheck.io/)** 🧪
  Serviço de verificação de vazamentos de dados com cobertura ampla de bases públicas e privadas.

- **[H8mail](https://github.com/khast3x/h8mail)** 🎣
  Ferramenta de OSINT para caça a e-mails vazados, com suporte a múltiplas APIs de breach data em uma única consulta.

---

## 🔧 Ferramentas de Suporte e Análise de Dados (Canivetes Suíços)

Ferramentas multipropósito que auxiliam na manipulação, visualização e organização de dados coletados durante investigações.

- **[CyberChef](https://github.com/gchq/CyberChef)** 🍳
  "O canivete suíço cibernético" — plataforma web para decodificação, criptografia, parsing e transformação de dados em geral.

- **[Recon-ng](https://github.com/lanmaster53/recon-ng)** 🧭
  Framework modular de reconhecimento web com interface similar ao Metasploit, facilitando automação de coleta OSINT.

- **[Gephi](https://gephi.org/)** 🕸️
  Software de visualização e análise de grafos, útil para representar relações complexas entre entidades investigadas.

- **[Obsidian](https://obsidian.md/)** 🗒️
  Ferramenta de notas em grafo, adotada por investigadores para organizar evidências e conectar informações ao longo do tempo.

- **[jq](https://github.com/jqlang/jq)** 🔩
  Processador de linha de comando para JSON, essencial na manipulação de respostas de APIs OSINT em scripts de automação.

- **[Exiftool](https://github.com/exiftool/exiftool)** 🖼️
  Ferramenta para extração e análise de metadados de arquivos (imagens, documentos, PDFs), revelando dados ocultos relevantes para investigações.

- **[Timesketch](https://github.com/google/timesketch)** ⏱️
  Plataforma de análise forense colaborativa para criação de linhas do tempo (timelines) a partir de grandes volumes de eventos.

---

## 🤝 Como Contribuir

Contribuições são muito bem-vindas! Para manter a qualidade e relevância do repositório, siga este fluxo:

1. Faça um **fork** deste repositório.
2. Crie uma branch descritiva: `git checkout -b adiciona-ferramenta-x`.
3. Adicione a ferramenta na seção correspondente, seguindo o padrão:
   ```markdown
   - **[Nome da Ferramenta](link-oficial)** 🔧
     Descrição concisa (1-2 linhas) do valor prático da ferramenta para pentest, investigação ou CTI.
   ```
4. Certifique-se de que a ferramenta:
   - Possui repositório oficial ativo ou site oficial confiável;
   - Tem relevância comprovada para OSINT/Pentest/CTI/SOCMINT;
   - Não duplica uma ferramenta já listada.
5. Abra um **Pull Request** explicando brevemente por que a ferramenta deve ser incluída.

Sugestões de melhorias na estrutura do README, correção de links quebrados e traduções também são muito apreciadas via **Issues**.

---

⭐ Se este repositório foi útil para você, considere deixar uma estrela para ajudar outros profissionais a encontrá-lo!
