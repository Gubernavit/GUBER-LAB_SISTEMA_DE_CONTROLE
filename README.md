# 🟠 GUBER-LAB | Universal Automation System

> **Status do Sistema:** 🟢 Operacional 
> **Ambientes:** Industrial & Residencial

O **GUBER-LAB** é uma plataforma de automação de alto desempenho desenvolvida para o controle e monitoramento de dispositivos via protocolo MQTT. Com uma interface inspirada em painéis industriais modernos, o sistema oferece uma experiência imersiva e segura para o gerenciamento de cargas elétricas em tempo real.

---

## 🛠️ Tecnologias & Core
`HTML5` | `CSS3 (Industrial Dark)` | `JavaScript ES6` | `MQTT WebSockets` | `Web Audio API`

---

## 🚀 Funcionalidades Elite

### ⚡ Controle de Potência
* **Grid de 8 Canais**: Acionamento individual de relés com feedback visual de estado.
* **Comandos de Grupo**: Funções "Master ON" e "Master OFF" para controle total imediato.

### 🛰️ Diagnóstico e Conectividade
* **Status de Nuvem**: Indicador visual de conexão com o Broker MQTT.
* **Heartbeat de Hardware**: Monitoramento de presença do ESP32/Dispositivo local via sinal "PONG".

### 🔐 Segurança Administrativa
* **Gestão de Hierarquia**: Criação de usuários com permissões granulares (Operar, Criar, Editar, Deletar).
* **Autorização por Senha**: Modais de confirmação para ações críticas do sistema.
* **Privacidade**: Alternância de visibilidade de senha (ícone de olho) integrada em todos os módulos.

### 🔊 Interface Auditiva
* **Motor de Áudio Interno**: Tons sintetizados para confirmação de comandos, alertas de sistema e erros de rede.

---

## 🏗️ Estrutura de Comunicação (MQTT)

O GUBER-LAB utiliza o Broker **HiveMQ** para orquestrar as mensagens:

| Tópico | Função | Mensagem |
| :--- | :--- | :--- |
| `guberlab/comando` | Envio de ordens | `T1..T8`, `L_TUDO`, `D_TUDO` |
| `guberlab/status` | Recebimento de dados | `PONG` (Online), `S1:1` (Estado) |

---

## 💻 Instalação & Teste

1.  **Hospedagem**: O sistema está otimizado para **GitHub Pages**.
2.  **Acesso Para testes**:
    * **User:** `Teste`
    * **Pass:** `123`
    * O usuario **"Teste"** tera acesso a todo o sistema mas nao tera poder de fazer nada.
3.  **Configuração de Hardware**: Basta configurar seu ESP32/ESP8266 para escutar os tópicos acima via WebSockets na porta `8000`.

---

## 🎨 Identidade Visual
* **Primária:** `#ff6a00` (International Orange)
* **Background:** `#0d0d0d` (Deep Carbon)
* **Cards:** `#1a1a1a` (Industrial Gray)

---
**Desenvolvido com foco em precisão e robustez por Gubernavit.**
