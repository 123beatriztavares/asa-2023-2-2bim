# PROXY

Um servidor proxy é um intermediário entre o seu dispositivo (como um computador ou smartphone) e a Internet. Ele atua como um gateway entre o cliente (você) e o servidor, encaminhando suas solicitações e recebendo as respostas. 



## Instalação
>sudo apt update (atualizar)

>sudo apt install squid (instalação)

>Inicie o serviço Squid
(sudo systemctl start squid)

>Verifique se o serviço está em execução
(sudo systemctl status squid)
 
 . Durante a instalação será criado vários arquivos e diretórios, entre eles:
> debian.conf (o nome varia dependendo da distro)

> access.log


- Por padrão o squid nega todo o acesso quando é instalado, para desabilitar vá em:
> nano /etc/squid/squid.conf
 - Dentro desse arquivo procure a linha http_acess deny all e troque para allow isso vai permitir o acesso para todos os sites.



## Configuração
Será adicionado nossa acl, o padrão de construção é:


> acl NOME_DA_ACL TIPO_DA_ACL parâmetro

> EX: acl exemplo dst www.facebook.com

Arquivo parão!
[![Captura de Tela (13)](https://i.im.ge/2024/01/03/3o9Gpm.Captura-de-Tela-13.png)](https://im.ge/i/3o9Gpm)


### Tipos de permissão:

> deny: nega o acesso

>allow: permite o acesso

### Fotos das acl criadas:
[![Captura de Tela (14)](https://i.im.ge/2024/01/03/3oxSZx.Captura-de-Tela-14.png)](https://im.ge/i/3oxSZx)

[![Captura de Tela (15)](https://i.im.ge/2024/01/03/3o30J0.Captura-de-Tela-15.png)](https://im.ge/i/3o30J0)

[![Captura de Tela (16)](https://i.im.ge/2024/01/03/3oYgy0.Captura-de-Tela-16.png)](https://im.ge/i/3oYgy0)

[![Captura de Tela (17)](https://i.im.ge/2024/01/03/3oYZmL.Captura-de-Tela-17.png)](https://im.ge/i/3oYZmL)

[![Captura de Tela (18)](https://i.im.ge/2024/01/03/3oYvaS.Captura-de-Tela-18.png)](https://im.ge/i/3oYvaS)









Incluir o(s) nome(s) e o conteúdo do(s) 


arquivo(s) de configuração.


Fazer a configuração de 4 ACLs distintas, conforme a atividade passada em sala de aula.

## Teste
Passo a Passo  do teste!

> 1. Abra o navegar.
 > 2. No menu, selecione Configurações ou opções.
> 3. Na seção Rede, selecione Configuracões de Proxy.
> 4. Marque a caixa Usar um servidor proxy.
> 5. Insira o endereço IP do servidor proxy e a porta.
(O navegador fica de sua preferência)

### Logs!
> tail -f /var/log/squid/access.log 