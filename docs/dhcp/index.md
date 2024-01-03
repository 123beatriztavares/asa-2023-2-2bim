# DHCP

O DHCP, sigla para Dynamic Host Configuration Protocol (Protocolo de Configuração Dinâmica de Host), é um protocolo de rede usado para atribuir automaticamente endereços IP e outras informações de configuração de rede a dispositivos em uma rede. O objetivo principal do DHCP é simplificar a administração da configuração de rede.



## Instalação

>sudo apt update (atualizar)

>apk add install dnsmasq (instalação)

## Configuração
>nano /etc/dnsmasq.d/asa.conf

. Dentro desse arquivo, coloca uma parte da configuração!

### Configuração do DHCP
interface=eth1

dhcp-range=192.168.13.10,192.168.13.100,255.255.255.0,12h

dhcp-option=3,192.168.13.254

dhcp-option=6,192.168.13.254

dhcp-option=15,pernambuco.lab

log-facility=/var/log/dnsmasq.log

dhcp-host=08:00:27:80:97:3D,192.168.13.15

dhcp-host=08:00:27:07:9C:19,192.168.13.16


>- Entrar dentro do arquivo:

> nano /etc/network/interfaces

auto lo

    iface lo inet loopback

auto eth0

    iface eth0 inet dhcp

auto eth1 inet static 

    iface eth1 inet static
    address 192.168.13.254/24

### Subir interfaces
> rc-service dnsmasq restart

### log
> tail -f /var/log/dnsmasq.log






Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Distribuir um intervalo (*range* em inglês) de endereços IP; (15 pontos)
- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)

## Teste
. Foi pego os endereços MAC de duas máquinas windows para poder colocar nas configurações do dhcp e pegar o endereço fixo, após isso faz o teste pigando as máquinas.

### Exemplo do teste:
> ping:192.168.13.15

>ping:192.168.13.16

