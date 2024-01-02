# PROXY

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

[Title](https://im.ge/i/Captura-de-Tela-1-Edited.xBEq54)

- Por padrão o squid nega todo o acesso quando é instalado, para desabilitar vá em:
> nano /etc/squid/squid.conf
 - Dentro desse arquivo procure a linha http_acess deny all e troque para allow isso vai permitir o acesso para todos os sites.



## Configuração
Será adicionado nossa acl, o padrão de construção é:


> acl NOME_DA_ACL TIPO_DA_ACL parâmetro

> EX: acl exemplo dst www.facebook.com

Arquivo parão!
[Title](https://im.ge/i/Captura-de-Tela-2.xBbYpX)

### Tipos de permissão:

> deny: nega o acesso
allow: permite o acesso

### Fotos das acl criadas:


[Title](https://im.ge/i/Captura-de-Tela-7.xBWsRh)

[Title](https://im.ge/i/Captura-de-Tela-8.xBWzO9)

[Title](https://im.ge/i/Captura-de-Tela-9.xBWpW8)

[Title](https://im.ge/i/Captura-de-Tela-10.xBWBBD)



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
> tail -f /var/ç/log/squid/access.log 