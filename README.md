# 🖥️ PcDriver

🚀 **Seu PC, seu ecossistema cloud pessoal. Sem limites, sem taxas, com controle total.**

O **PcDriver** é um servidor pessoal ultraleve e de alta performance que transforma sua máquina Windows ou Linux em uma central cloud privada. Através de uma interface web única e intuitiva, você gerencia seu drive, compartilhamentos de arquivos, servidores SMB e WebDAV, automações, tarefas agendadas e muito mais.

> 💡 **Nota do Desenvolvedor:** Este é um projeto pessoal que desenvolvi para suprir minhas próprias necessidades diárias. Como ele tem sido extremamente útil e estável no meu dia a dia, resolvi disponibilizá-lo de forma aberta para a comunidade, esperando que possa ajudar mais pessoas que buscam uma solução leve e integrada.

---

## ✨ Por que o PcDriver?

Se você está cansado de mensalidades de serviços em nuvem, quer acessar seus arquivos sem complicações através de qualquer protocolo e precisa de controle remoto real sobre a sua máquina com automações inteligentes, o PcDriver foi feito para você.

* 🌐 **Acesso de Qualquer Lugar:** Acesse seus arquivos na rede local ou na internet de forma segura.
* ⚡ **Performance Nativa:** Construído sobre tecnologia de ponta, oferecendo uma experiência fluida e imediata.
* 🛠️ **Ecossistema Tudo-em-Um:** Gerencie arquivos via Web, monte unidades via SMB/WebDAV e agende tarefas no mesmo lugar.
* 🔒 **Segurança Inteligente (Dual Port):** Suporta duas portas simultâneas — uma interna (para acessar a administração - na rede local ou VPN) e outra para uso externo de coisas limitadas, eliminando o overhead da VPN e mantendo a segurança.
* 📦 **Zero Complicações:** Leve, autônomo e sem necessidade de bancos de dados complexos ou configurações iniciais dolorosas.

---

## 🛠️ Recursos Principais

### 📂 Nuvem Privada & Drive
* **Gestão Total:** Upload, download, criação de pastas e busca inteligente.
* **Streaming de Vídeo:** Assista aos seus vídeos diretamente no navegador (com integração *ffmpeg*).

### 🔗 Protocolos de Rede & Compartilhamento (SMB & WebDAV)
* **Servidor SMB Integrado:** Compartilhe suas pastas na rede local de forma nativa, permitindo que Smart TVs, consoles e outros computadores acessem seus arquivos instantaneamente sem softwares adicionais.
* **Suporte WebDAV:** Sincronize e monte o seu PcDriver como um disco virtual diretamente no gerenciador de arquivos do seu sistema operacional (Windows Explorer, Finder, Nautilus) ou celular.
* **Links Temporários:** Compartilhe arquivos e pastas publicamente através de links web que expiram.
* **Proteção Extra:** Proteja qualquer pasta, arquivo ou protocolo compartilhado com senhas exclusivas.

### ⏱️ Agendamentos & Tarefas em Segundo Plano (Cron)
* **Tarefas em Background:** Execução assíncrona de processos pesados sem travar a interface (conversão de vídeos, compactação de arquivos e pastas, backups).
* **Crons Customizadas:** Agende rotinas, scripts e automações do sistema para rodar nos dias e horários exatos que você precisar.
* **Fila de Execução:** Acompanhe o progresso de tarefas longas em tempo real com logs dedicados.

### 🕹️ Controle Remoto & Ferramentas
* **Execução Remota:** Inicie programas e execute automações no seu PC a partir do celular ou de outro dispositivo.
* **Wake-on-LAN (WoL):** Ligue outros computadores da sua rede local remotamente.
* **SpeedTest:** Meça a velocidade da sua conexão com a internet diretamente pelo painel.
* **Log do Sistema:** Monitore todas as ações, conexões de rede e execuções de tarefas através do registro de atividades.

### 👥 Gestão de Acessos
* **Controle de Usuários:** Crie múltiplas contas, defina permissões granulares de leitura/escrita e monitore sessões ativas em tempo real.

---

## 📅 Agendamentos e Tarefas em Segundo Plano

O PcDriver conta com um poderoso gerenciador de tarefas integrado. Você não precisa mais depender do Agendador de Tarefas do Windows ou do Cron do Linux para automatizar sua máquina.

* **Sintaxe Cron Padrão:** Configure agendamentos flexíveis de forma simples e visual.
* **Automação de Scripts:** Deixe scripts de backup, limpeza de disco ou inicialização rodando 100% no background.
* **Visualização de Status:** Monitore o histórico de execuções, tempo gasto e o status de sucesso ou falha das tarefas diretamente pelo painel web.

---

## Screenshots
<img width="955" height="438" alt="image" src="https://github.com/user-attachments/assets/87402106-c99c-45d2-8263-b6d4137bb3ee" />

<img width="947" height="422" alt="image" src="https://github.com/user-attachments/assets/c102b2f4-d1f8-4492-8d3a-c3987725e209" />

<img width="955" height="437" alt="image" src="https://github.com/user-attachments/assets/01645212-0c93-4fa0-baff-571d192c2d98" />

<img width="637" height="353" alt="image" src="https://github.com/user-attachments/assets/86e97a1f-2038-4b38-8922-cf13360b0b80" />

---

## 🚀 Primeira Execução

O PcDriver inclui um **assistente de configuração web interativo** para que você não precise editar arquivos de texto ou configurar bancos de dados manualmente. 

A configuração inicial deve ser acessada por **http://localhost:8088/Setup**.

1. Execute o PcDriver pela primeira vez.
2. Abra a interface web e crie o seu usuário **Administrador**.
3. Defina as configurações de rede (Nome do dispositivo, Portas do painel, e ativação dos módulos **SMB** e **WebDAV**).
4. Configure seus certificados HTTPS (Suporta certificados autoassinados gerados automaticamente ou certificados autênticos).

---

## 🛡️ Isenção de Responsabilidade e Termos de Uso

Como este projeto nasceu de uma iniciativa pessoal e é disponibilizado de forma gratuita e aberta, **o seu uso é por sua conta e risco**. Ao utilizar este software, você concorda explicitamente com as seguintes condições:

* 🫵 **Responsabilidade Exclusiva do Usuário:** Toda e qualquer rotina de **segurança, camadas de proteção, firewalls, permissões de pastas SMB/WebDAV e execução de backups** é de sua inteira e exclusiva responsabilidade.
* 💾 **Backups:** É sua obrigação manter cópias de segurança periódicas dos seus arquivos, do `config.ini`, de certificados, das tarefas agendadas e do arquivo `pcdriver.db`.
* 🔐 **Credenciais:** Não armazene senhas críticas no sistema sem proteção adicional e certifique-se de que as portas expostas externamente estejam devidamente protegidas e monitoradas.
* ❌ **Isenção Total do Desenvolvedor:** O desenvolvedor **não possui qualquer responsabilidade** por perda de dados, danos ao sistema, invasões, exposição indevida de arquivos na rede ou quaisquer prejuízos decorrentes de má configuração, falhas ou uso incorreto deste software.

---

## 💻 Stack Tecnológica

O PcDriver utiliza tecnologia moderna e robusta para garantir a máxima eficiência:

* 🔥 **[ASP.NET Core 8](https://dotnet.microsoft.com/)** — Motor web de alta performance e gerenciamento nativo de *Hosted Services* para as tarefas em background.
* ⚡ **[Kestrel](https://learn.microsoft.com/aspnet/core/fundamentals/servers/kestrel)** — Servidor web nativo ultraleve.
* 🗄️ **[SQLite](https://www.sqlite.org/)** — Banco de dados local rápido e em arquivo único para logs, usuários e agendamentos.
* 🎨 **[Bootstrap 5](https://getbootstrap.com/)** & **[Font Awesome](https://fontawesome.com/)** — Interface moderna, limpa e totalmente responsiva (Mobile-First).
* 🛠️ **JavaScript (SPA)** — Arquitetura de página única para navegação instantânea sem recarregamentos.
* 🎬 **[FFmpeg](https://ffmpeg.org/)** — Processamento e streaming de vídeo inteligente.

e outras...

---

## 📄 Licença

Consulte o arquivo `LICENSE` para mais detalhes.

---

Deixo a discussão aberta no github para contatos.
