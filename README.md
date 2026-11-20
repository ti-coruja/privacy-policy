# Política de Privacidade — ARA OS Deploy (TI Coruja)

**Última atualização:** Novembro de 2026

A privacidade e a segurança dos dados dos nossos usuários e parceiros são prioridades absolutas. Esta Política de Privacidade descreve como a **TI Coruja Inova Simples (I.S.)** (CNPJ 65.522.668/0001-44) trata informações no ecossistema **ARA OS Deploy** (Aplicativo Android, Agente PC, site oficial e portal de parceiros), em conformidade com a Lei Geral de Proteção de Dados (Lei nº 13.709/2018 – LGPD).

---

### 1. Coleta e Armazenamento de Dados Pessoais (Minimização de Dados)
Operamos sob o princípio de **minimização de dados**, coletando apenas o estritamente necessário para cada finalidade:

* **No Aplicativo Android e Agente PC:** Coletamos exclusivamente o endereço de **e-mail** do titular e o **identificador único de hardware (HWID)**. Essas informações são processadas em nossos servidores para autenticação, gestão de conta, validação de licença e prevenção contra pirataria/uso simultâneo indevido.
* **Na Contratação pelo Site (Checkout):** Para emissão obrigatória de Nota Fiscal de Serviço Eletrônica (NFS-e) e processamento de pagamentos, coletamos **Nome completo ou Razão Social**, **CPF ou CNPJ** e **e-mail**.
* **No Portal de Parceiros / Vendedores (`vendedores.html`):** Para cadastro de afiliados, repasse de comissões e prevenção contra autoindicação, coletamos **Nome completo**, **CPF**, **e-mail** e **Chave PIX**.
* **Não coletamos** localização geográfica, agenda de contatos, histórico de navegação externa ou arquivos pessoais armazenados nos computadores formatados pelo técnico.

---

### 2. Uso da Rede Local (LAN), P2P e Logs Zero-Knowledge
O aplicativo atua como um gerenciador e mini-servidor local de automação para formatação e configuração de sistemas operacionais.

* **Comunicação Restrita à LAN:** Todas as transferências de arquivos (ISOs, executáveis do agente e scripts de configuração) e verificações de presença ocorrem **exclusivamente dentro da sua rede local (Wi-Fi/LAN ou Tethering USB)** entre o dispositivo móvel e o computador de destino.
* **Preferências e Logs:** Suas preferências de pré-personalização permanecem armazenadas localmente no seu dispositivo. Caso o envio opcional de logs em nuvem seja ativado pelo usuário, os registros trafegam com criptografia ponta a ponta (*zero-knowledge*), sem acesso legível por parte da TI Coruja.

---

### 3. Permissões e Recursos do Sistema Solicitados (Android)
Para operar suas funções de automação, servidor HTTP e download de alta performance, o **ARA OS Deploy** solicita e utiliza os seguintes recursos do dispositivo:

* **Serviço em Primeiro Plano (`FOREGROUND_SERVICE` / `FOREGROUND_SERVICE_DATA_SYNC`):** Necessária para manter o mini-servidor HTTP local ativo e realizar o download contínuo de arquivos grandes (ISOs/Agente) sem interrupção do sistema operacional quando o app estiver em segundo plano ou com a tela apagada/bloqueada.
* **Acesso à Rede e Wi-Fi (`INTERNET`, `ACCESS_NETWORK_STATE`, `ACCESS_WIFI_STATE`):** Necessária para identificar o endereço IP local do dispositivo na LAN/Tethering, permitir conexões do computador cliente e efetuar o download dos arquivos oficiais e validação de licença via HTTPS.
* **Armazenamento / Leitura e Escrita (`READ_EXTERNAL_STORAGE`, `WRITE_EXTERNAL_STORAGE`):** Necessária para ler imagens da galeria selecionadas pelo usuário para papel de parede do sistema e salvar arquivos de dados do aplicativo.
* **Notificações (`POST_NOTIFICATIONS`):** Necessária para exibir alertas em tempo real sobre a velocidade de transferência, tempo restante de download e status de execução do servidor local.
* **Gestão de Energia e Repouso (`WAKE_LOCK`, `REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`):** Necessária para evitar que a CPU e o adaptador Wi-Fi entrem em modo de suspensão durante a transferência de arquivos pesados na rede local.

---

### 4. Comunicação Externa, Subprocessadores e Cookies
A TI Coruja **não comercializa dados pessoais** e **não utiliza SDKs de anúncios dentro do aplicativo**. O tráfego externo e o compartilhamento ocorrem estritamente para operação técnica e financeira:

1. **Validação de Licença e Downloads Oficiais:** Comunicação via HTTPS com a infraestrutura oficial da TI Coruja para autenticar a chave/HWID e baixar arquivos oficiais solicitados pelo operador.
2. **Processamento Financeiro (Asaas Gestão Financeira S.A.):** Intermediação de cobranças (PIX e Cartão de Crédito) e repasse de comissões aos parceiros.
3. **Infraestrutura e Segurança (Cloudflare):** Hospedagem, banco de dados serverless, armazenamento de arquivos e proteção anti-bot no site.
4. **Métricas Web e Armazenamento Local:** No site institucional e no portal de parceiros, utilizamos armazenamento local do navegador (`localStorage`/`sessionStorage`) para manter sessões autenticadas, preferência de idioma, aceite de termos e atribuição de indicação comercial por 7 dias, além de tags de conversão do Google Ads no site.
5. **Painel de Parceiros:** Quando uma assinatura ocorre via link de indicação, o parceiro indicador visualiza em seu painel apenas o nome/razão social do cliente, status da assinatura e contato parcialmente mascarado para conferência de comissões.

---

### 5. Retenção e Exclusão de Dados
* Os dados técnicos de conta (e-mail e HWID) são mantidos enquanto a licença estiver ativa e pelo período necessário à prevenção contra fraudes e controle de elegibilidade de testes/reembolsos.
* Dados vinculados a transações financeiras, emissão de NFS-e e comprovantes de repasse PIX (CPF/CNPJ, valores e datas) são mantidos pelo prazo mínimo de **5 (cinco) anos**, conforme exigência da legislação fiscal e tributária brasileira.
* Caso deseje solicitar acesso, correção ou a exclusão definitiva de seus dados não sujeitos à guarda legal obrigatória, envie uma solicitação para o e-mail indicado na seção 7.

---

### 6. Alterações Nesta Política
Podemos atualizar nossa Política de Privacidade periodicamente para refletir melhorias no sistema ou mudanças regulatórias. Recomendamos revisar esta página ocasionalmente.

---

### 7. Contato (Controlador e DPO)
Se você tiver dúvidas sobre esta Política de Privacidade ou sobre o tratamento de dados pessoais, entre em contato com o suporte oficial:

* **Controladora:** TI Coruja Inova Simples (I.S.) — CNPJ 65.522.668/0001-44
* **E-mail:** atendimento@ticoruja.com
