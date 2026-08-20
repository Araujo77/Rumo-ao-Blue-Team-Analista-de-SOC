# Analista de SOC (Security Operations Center)



 
 1. Fundamentos de TI e Redes (A Base)Antes de proteger qualquer coisa, você precisa entender como os dados trafegam.
   
  -   Redes: Modelo OSI/TCP/IP, endereçamento IP, sub-redes, e portas.
   
  -   Protocolos essenciais: DNS, HTTP/HTTPS, DHCP, SSH, SMB e RDP.
   
  -   Ferramenta inicial: Aprenda o básico do Wireshark para capturar e inspecionar pacotes de rede.

   

2. Sistemas Operacionais (Windows e Linux)Você precisa conhecer a fundo os sistemas que vai defender.
   
   
  -  Linux: Comandos essenciais de terminal, permissões de arquivos, processos e navegação no sistema de arquivos.
   
  -  Windows: Entender a estrutura interna básica, diretórios e noções de Active Directory (essencial para ambientes corporativos).
   
  -  Logs de Eventos: Aprender onde ficam e como ler os logs do Windows (Event Viewer) e do Linux (syslog, /var/log/).



  3. Conceitos de Segurança Defensiva e Ferramentas
     
  -  Conceitos: Tríade CIA (Confidencialidade, Integridade e Disponibilidade), princípios de Defesa em Profundidade e o framework MITRE ATT&CK.
   
  -  SIEM (Security Information and Event Management): Ferramentas que centralizam e analisam logs de segurança (como Splunk, ELK Stack ou Wazuh).
   
  -  EDR (Endpoint Detection and Response): Entender o monitoramento de estações de trabalho e servidores.


   

   4. Onde Praticar de Forma Prática e Gratuita
      
    
   -  Utilize plataformas de laboratórios interativos focados em defesa, como o TryHackMe (faça as salas voltadas para Blue Team/SOC).
      
   -   Explore trilhas de introdução à defesa como o curso gratuito Blue Team Junior Analyst (BTJA) da Security Blue Team.
      
   -   No Brasil, acompanhe iniciativas públicas de capacitação como o programa Hackers do Bem para trilhas estruturadas em cibersegurança.




# Criar regras para notificações de alerta


Você pode criar regras que determinam os dispositivos e as severidades de alerta para enviar notificações por email a destinatários de notificação.


- No portal do Microsoft Defender, selecione Configurações, Pontos de extremidade e Notificações por email.

  <img width="796" height="47" alt="image" src="https://github.com/user-attachments/assets/40a24ad4-d053-47f5-b6ac-f6bd0a758c5e" />
  
<img width="388" height="796" alt="image" src="https://github.com/user-attachments/assets/83a022e9-4fe0-4e38-9c1c-ea0404ab3f44" />


- Selecione Adicionar item.

  <img width="901" height="266" alt="image" src="https://github.com/user-attachments/assets/f4b94831-2bb0-4764-ae39-335cc1b83927" />


## Especifique as informações gerais:

- Nome da regra – Especifique um nome para a regra de notificação.

  <img width="1314" height="405" alt="image" src="https://github.com/user-attachments/assets/964dae6f-9d91-40b5-ad62-a80b772e6aab" />


- Incluir nome da organização – Especifique o nome do cliente que aparece na notificação por email.

- Incluir link do portal específico ao locatário – Adiciona um link com a ID do locatário para permitir o acesso a um locatário específico.

- Incluir informações do dispositivo – Inclui o nome do dispositivo no corpo do alerta de email.

- Dispositivos – Escolha se deseja notificar os destinatários para alertas em todos os dispositivos (somente função de administrador da empresa) ou grupos de dispositivos selecionados. Para obter mais informações, veja Criar e gerenciar grupos de dispositivo.

- Severidade do alerta – Escolha o nível de severidade do alerta.

- Selecione Avançar.
  

  <img width="1485" height="858" alt="image" src="https://github.com/user-attachments/assets/b76b393f-36cf-45b7-a033-3e873f1f13f0" />


- Digite um endereço de email e, em seguida, selecione Adicionar destinatário. Você pode adicionar vários endereços de email.
  

  <img width="1444" height="850" alt="image" src="https://github.com/user-attachments/assets/7ffc6ec6-573c-42e6-8f29-cbeb58ec2c8e" />



- Verifique se os destinatários de email podem receber as notificações por email selecionando Enviar email de teste.

- Selecione Salvar regra de notificação.

  <img width="1439" height="858" alt="image" src="https://github.com/user-attachments/assets/ab5bb694-a26e-446f-9607-3a20001f0e66" />


# Gerenciar supressão de alerta

## Exibir regras existentes
Você pode visualizar uma lista de todas as regras de ajuste de alertas e gerenciá-las em um só lugar. Você também pode ativar ou desativar uma regra de ajuste de alerta concluindo estas ações:

1- No portal do Microsoft Defender, selecione Configurações, selecione Microsoft Defender XDR e, em Seguida, em Regras, selecione Ajuste de alerta. A lista de regras de ajuste de alerta que os usuários da sua organização criaram são exibidas.

2- Selecione uma regra marcando a caixa de seleção ao lado do nome da regra.

3- Selecione Ativar regra, Editar regra ou Excluir regra. Ao fazer alterações em uma regra, você pode optar por liberar alertas que já foram suprimidos, independentemente de esses alertas corresponderem ou não aos novos critérios.


Gerenciar indicadores
Para gerenciar indicadores:

No painel de navegação, selecione Configurações > Pontos de extremidade e, na área Regras, selecione Indicadores.

Selecione a guia do tipo de entidade que você deseja gerenciar.

Atualize os detalhes do indicador e selecione Salvar, ou selecione o botão Excluir, se desejar remover a entidade da lista.

# Pré-requisitos
Antes de criar indicadores para arquivos, você deve entender os seguintes pré-requisitos:

- Esse recurso estará disponível se a sua organização usar o Windows Defender Antivírus e se a proteção baseada em Nuvem estiver habilitada. Para obter mais informações, consulte Gerenciar proteção baseada em nuvem.

- A versão do cliente antimalware deve ser 4.18.1901.x ou posterior.

- Ele tem suporte em computadores que executam Windows 10 (versão 1703 ou posterior), Windows 11, Windows Server 2016, Windows Server 2019 ou Windows Server 2022.

- Para iniciar o bloqueio de arquivos, primeiro você precisa ativar o recurso Bloquear ou permitir em Configurações.

- Esse recurso foi projetado para impedir que o malware suspeito (ou arquivos possivelmente maliciosos) seja baixado da Web. Atualmente, ele dá suporte a arquivos PE (executáveis portáteis), incluindo arquivos de .exe e .dll. A cobertura será estendida ao longo do tempo.

## Criar indicadores para arquivos

Você pode evitar a propagação adicional de ataques em sua organização, proibindo arquivos potencialmente mal-intencionados ou malware suspeito. Se você souber de um arquivo executável portátil (PE) potencialmente malicioso, poderá bloqueá-lo. Essa operação impede que ela seja lida, gravada ou executada em computadores em sua organização.

Há duas maneiras de criar indicadores para arquivos:

- Criar um indicador na página Configurações

- Criar um indicador contextual usando o botão Adicionar indicador da página de detalhes do arquivo


# Criar indicadores para IPs e URLs/domínios

O Defender para Endpoint pode bloquear IPs/URLs que a Microsoft considera mal-intencionados por meio do Microsoft Defender SmartScreen em navegadores da Microsoft e por meio da Proteção de Rede para navegadores que não sejam da Microsoft ou chamadas feitas fora de um navegador.

O conjunto de dados de inteligência contra ameaças para isso foi gerenciado pela Microsoft.

Ao criar indicadores para IPs e URLs ou domínios, agora você pode permitir ou bloquear IPs, URLs ou domínios com base em sua própria inteligência contra ameaças. Você pode fazer isso por meio da página configurações ou por grupos de computadores, se julgar que certos grupos tenham mais ou menos risco do que outros. Não há suporte para a notação CIDR (Roteamento entre Domínios sem Classificação) em endereços IP.

## Pré-requisitos

Você deve entender os seguintes pré-requisitos antes de criar indicadores para IPS, URLs ou domínios:

- Permissão e bloqueio de URL/IP depende da proteção de rede do componente do Microsoft Defender para Ponto de Extremidade a ser habilitada no modo de bloqueio. Para obter mais informações sobre proteção de rede e instruções de configuração, consulte Habilitar a proteção de rede.

- A versão do cliente Antimalware deve ser 4.18.1906.x ou posterior.

- Compatível com computadores com Windows 10, versão 1709 ou posterior.

- Verifique se os indicadores de rede Custom estão habilitados no portal Microsoft Defender. Selecione Configurações > Endpoints > Recursos avançados e ative Indicadores de rede personalizados.


  <img width="1425" height="839" alt="image" src="https://github.com/user-attachments/assets/04776c94-e1af-4562-b15a-b307b9059a3a" />


Somente IPs externos podem ser adicionados à lista de indicadores. Não é possível criar indicadores para IPs internos. Para cenários de proteção da Web, é recomendável usar os recursos internos do Microsoft Edge. O Microsoft Edge usa a proteção de rede para inspecionar o tráfego de rede e permite bloqueios para TCP, HTTP e HTTPS (TLS). Para os outros processos, os cenários de proteção da Web usam a proteção de rede para inspeção e imposição:

- O IP tem suporte para todos os três protocolos

- Há suporte apenas para endereços IP únicos (sem bloqueios CIDR ou intervalos de IP)

- URLs criptografadas (caminho completo) só podem ser bloqueadas em navegadores primários

- URLs criptografadas (caminho completo) só podem ser bloqueadas em navegadores primários

- Blocos de caminho de URL completos podem ser aplicados no nível de domínio e em todas as URLs não criptografadas

Pode haver até 2 horas de latência (geralmente menos) entre a hora em que a ação é executada e a URL e o IP sendo bloqueados.


# Criar um indicador para IPs, URLs ou domínios


1- No painel de navegação, selecione Configurações > Ponto Final >Indicadores.

<img width="411" height="782" alt="image" src="https://github.com/user-attachments/assets/c0eb03b2-3842-4c1b-8141-630b9e92a943" />


2- Selecione a guia de endereços IP ou URLs/Domínios.

<img width="917" height="307" alt="image" src="https://github.com/user-attachments/assets/f944db97-b1eb-405c-8c70-a045867129e4" />


3- Selecione Adicionar item.

<img width="909" height="379" alt="image" src="https://github.com/user-attachments/assets/9d27f7fd-4234-4a44-b932-31a5d7e7990e" />


4- Especifique os seguintes detalhes:

- Indicador – Especifique os detalhes da entidade e defina a expiração do indicador.

- Ação – Especifique a ação a ser executada e forneça uma descrição.

- Escopo – Defina o escopo do grupo de computadores.

<img width="1472" height="861" alt="image" src="https://github.com/user-attachments/assets/02ef8a1d-95d1-44c5-abe3-658947abe03f" />

<img width="1391" height="851" alt="image" src="https://github.com/user-attachments/assets/48632b76-7352-4cdc-a3ae-526603d9efd1" />

<img width="1397" height="851" alt="image" src="https://github.com/user-attachments/assets/4c113e45-4533-4fa4-9b34-e05a7d7c8534" />


5- Examine os detalhes na guia Resumo e, em seguida, selecione Salvar.

<img width="1418" height="846" alt="image" src="https://github.com/user-attachments/assets/9340cbb3-dc68-40f6-afb4-ff795d612eaa" />


#Importar uma lista de IoCs

Você também pode optar por carregar um arquivo CSV que define os atributos dos indicadores, a ação a ser executada e outros detalhes.

Baixe o CSV de exemplo para saber os atributos de coluna com suporte.

1- No portal do Microsoft Defender, selecione Configurações > Pontos de extremidade > Indicadores.

2- Selecione a guia do tipo de entidade para a qual você gostaria de importar os indicadores.

3- Selecione importar > Escolher arquivo.


<img width="919" height="378" alt="image" src="https://github.com/user-attachments/assets/fa9f7e2f-4292-4d5a-8ee1-ede3963d5e86" />


4- Selecione Importar. Faça isso para todos os arquivos que você gostaria de importar.


<img width="336" height="847" alt="image" src="https://github.com/user-attachments/assets/a2116ed1-06dc-4939-87fe-2a3fa5dab6f4" />


5- Selecione Concluído.








