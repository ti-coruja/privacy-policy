# Política de Privacidade — TI-Coruja

**Última atualização:** 25 de agosto de 2026

A privacidade e a segurança dos dados dos nossos usuários são prioridades absolutas. Esta Política de Privacidade descreve como o aplicativo **TI-Coruja** lida com suas informações.

---

### 1. Coleta e Armazenamento de Dados Pessoais (Minimização de Dados)
O **TI-Coruja** opera sob o princípio de **minimização de dados**, limitando a coleta ao estritamente necessário para a autenticação e validação de uso do software.

* **Coletamos exclusivamente** o endereço de **e-mail** do usuário e o **identificador de dispositivo/hardware (HWID)**. Essas informações são processadas de forma não efêmera no nosso servidor para fins de autenticação, gestão de conta, validação de licença e prevenção de fraudes (impedindo a execução simultânea da mesma licença em múltiplos celulares).
* **Não coletamos** nome completo, telefone, localização geográfica, contatos, dados bancários ou históricos de navegação.
* O aplicativo **não possui telemetria de rastreamento** comercial nem utiliza SDKs de terceiros para exibição de anúncios ou análise de perfil de usuário.
* Os dados coletados são transmitidos via conexão criptografada (HTTPS) diretamente para a nossa infraestrutura e **não são compartilhados com terceiros**.

---

### 2. Uso da Rede Local (LAN) e P2P
O aplicativo atua como um gerenciador e mini-servidor local de automação para formatação e configuração de sistemas operacionais.

* **Comunicação Restrita à LAN:** Todas as transferências de arquivos (ISOs, executáveis do agente e scripts de configuração) e verificações de presença ocorrem **exclusivamente dentro da sua rede local (Wi-Fi/LAN ou Tethering USB)** entre o dispositivo móvel e o computador de destino.
* **Nenhum Dado Enviado à Nuvem:** Suas preferências de pré-personalização (como nome de usuário, nome do computador, senha e imagens definidos para o sistema operacional) permanecem estritamente armazenadas no seu dispositivo e são servidas apenas para o agente na sua rede privada em conexão segura de ponta a ponta.

---

### 3. Permissões e Recursos do Sistema Solicitados

Para operar suas funções de automação, servidor HTTP e download de alta performance, o **TI-Coruja** solicita e utiliza os seguintes recursos do dispositivo:

* **Serviço em Primeiro Plano (`FOREGROUND_SERVICE` / `FOREGROUND_SERVICE_DATA_SYNC`):** Necessária para manter o mini-servidor HTTP local ativo e realizar o download contínuo de arquivos grandes (ISOs/Agente) sem interrupção do sistema operacional quando o app estiver em segundo plano ou com a tela apagada/bloqueada.
* **Acesso à Rede e Wi-Fi (`INTERNET`, `ACCESS_NETWORK_STATE`, `ACCESS_WIFI_STATE`):** Necessária para identificar o endereço IP local do dispositivo na LAN/Tethering, permitir conexões do computador cliente e efetuar o download dos arquivos oficiais e validação de licença via HTTPS.
* **Armazenamento / Leitura e Escrita (`READ_EXTERNAL_STORAGE`, `WRITE_EXTERNAL_STORAGE`):** Necessária para ler imagens da galeria selecionadas pelo usuário para papel de parede do sistema e salvar arquivos de dados do aplicativo.
* **Notificações (`POST_NOTIFICATIONS`):** Necessária para exibir alertas em tempo real sobre a velocidade de transferência, tempo restante de download e status de execução do servidor local.
* **Gestão de Energia e Repouso (`WAKE_LOCK`, `REQUEST_IGNORE_BATTERY_OPTIMIZATIONS`):** Necessária para evitar que a CPU e o adaptador Wi-Fi entrem em modo de suspensão durante a transferência de arquivos pesados na rede local.

---

### 4. Validação de Licença e Conexão Externa
A única comunicação externa via Internet realizada pelo aplicativo ocorre para:

1. **Validação do Certificado de Licença:** Comunicação direta com o servidor oficial do TI-Coruja via HTTPS para autenticar a chave do usuário e o HWID do dispositivo. Nenhuma outra informação pessoal além do e-mail de cadastro é anexada a esta requisição.
2. **Download de Arquivos Oficiais:** Conexão direta via HTTPS a repositórios oficiais/seguros para baixar o executável do agente e ISOs oficiais da empresa detentora de seus direitos, quando solicitado pelo usuário.

---

### 5. Retenção e Exclusão de Dados
Os dados de e-mail e HWID são mantidos em nosso servidor enquanto a licença do usuário estiver ativa. Caso deseje solicitar a exclusão definitiva de seus dados de cadastro, o usuário pode enviar uma solicitação diretamente para o suporte técnico através do e-mail indicado abaixo.

---

### 6. Alterações Nesta Política
Podemos atualizar nossa Política de Privacidade periodicamente para refletir melhorias no sistema ou mudanças regulatórias. Recomendamos revisar esta página ocasionalmente.

---

### 7. Contato
Se você tiver dúvidas sobre esta Política de Privacidade ou sobre o funcionamento interno do aplicativo, entre em contato pelo e-mail de suporte:
* **E-mail:** felipe.reskalla7@gmail.com
