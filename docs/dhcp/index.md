# DHCP

O DHCP, sigla para Dynamic Host Configuration Protocol (Protocolo de Configuração Dinâmica de Host), é um protocolo de rede usado para atribuir automaticamente endereços IP e outras informações de configuração de rede a dispositivos em uma rede. O objetivo principal do DHCP é simplificar a administração da configuração de rede.



## Instalação
<<<<<<< HEAD

>sudo apt update (atualizar)
=======
sudo apt update
apk add install dnsmasq
>>>>>>> 9a72ed38e5e6cf9c38fc17c7a1e0ec2cd7d3d934

>apk add install dnsmasq (instalação)

## Configuração
<<<<<<< HEAD
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




=======
 
 nano /etc/dnsmasq.d/asa.conf

dentro desse arquivo, colocaca uma parte da configuracão!

# Configuração do DHCP
. interface=eth1
. dhcp-range=192.168.13.10,192.168.13.100, 
  255.255.255.0,12h
. dhcp-option=3,192.168.13.254
. dhcp-option=6,192.168.13.254
. dhcp-option=15,pernambuco.lab
. log-facility=/var/log/dnsmasq.log
. dhcp-host=08:00:27:80:97:3D,192.168.13.15
. dhcp-host=08:00:27:07:9C:19,192.168.13.16


Entrar dentro do arquivo!

. nano /etc/network/interfaces
<br>auto lo
 <br> iface lo inet loopback 
  
  auto eth0
 <br> iface eth0 inet dhcp

  auto eth1 inet static
 <br> iface eth1 inet static
   <br> address 192.168.1.254/24

# subir interfaces
. rc-service dnsmasq restart


# log
. tail -f /var/log/dnsmasq.log
>>>>>>> 9a72ed38e5e6cf9c38fc17c7a1e0ec2cd7d3d934


Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Distribuir um intervalo (*range* em inglês) de endereços IP; (15 pontos)
- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)

## Teste
<<<<<<< HEAD
. Foi pego os endereços MAC de duas máquinas windows para poder colocar nas configurações do dhcp e pegar o endereço fixo, após isso faz o teste pigando as máquinas.

### Exemplo do teste:
> ping:192.168.13.15

>ping:192.168.13.16

=======
. Foi pego os endereços mac de duas máquinas windows para poder colocar nas configuracoẽs do dhcp e pegar o endereço fixo.
Após isso faz o teste pigando as máquinas.

## Exemplo 
ping- 192.168.13.15
<br>ping- 192.168.13.16
>>>>>>> 9a72ed38e5e6cf9c38fc17c7a1e0ec2cd7d3d934
