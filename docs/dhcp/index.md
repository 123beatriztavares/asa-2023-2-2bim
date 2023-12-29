# DHCP

## Instalação
sudo apt update
apk add install dnsmasq


## Configuração
 
 bat /etc/dnsmasq.d/asa.conf

dentro desse arquivo, colocaca uma parte da configuracão!

#Configuração do DHCP
interface=eth1
dhcp-range=192.168.13.10,192.168.13.100,255.255.255.0,12h
dhcp-option=3,192.168.13.254
dhcp-option=6,192.168.13.254
dhcp-option=15,pernambuco.lab
log-facility=/var/log/dnsmasq.log
dhcp-host=08:00:27:80:97:3D,192.168.13.15
dhcp-host=08:00:27:07:9C:19,192.168.13.16



Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Distribuir um intervalo (*range* em inglês) de endereços IP; (15 pontos)
- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)

## Teste


