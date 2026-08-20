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























