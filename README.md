# Honeypot Lab - Captura de Ataques RDP (Porta 3389) 🛡️

Neste laboratório, configurei uma "isca" no Kali Linux para monitorar tentativas de acesso na porta 3389 (Remote Desktop). Utilize os logs para analisar a origem e o comportamento de bots e scanners de vulnerabilidade.

### 🛠️ Tecnologias Utilizadas
* **Kali Linux** (Ambiente controlado).
* **Pentbox 1.8** (Emulação de Honeypot).
* **Cloudflare Tunnel** (Para expor o serviço de forma segura sem abrir portas no roteador).
* **Check-Host** (Para propagação e teste global do link).

### 📊 O que foi capturado?
Assim que o túnel subiu, o terminal começou a registrar conexões imediatas. Nos logs anexados (`ataquehoneypot`), é possível observar:
* 🇩🇪 Ataques originados na **Alemanha** (IP: 116.203.22.31).
* 🇮🇳 Ataques originados na **Índia** (IP: 198.161.20.15).
* Scanners identificados via User-Agent `CheckHost`.

### 📽️ Demonstração Prática (Honeypot em Ação)


### 📝 Lições Aprendidas
1. O tempo de descoberta de um serviço exposto é quase instantâneo.
2. O uso de túneis (Cloudflare) facilita o laboratório sem comprometer a rede física (Host).
3. A importância de monitorar logs para entender a superfície de ataque.
