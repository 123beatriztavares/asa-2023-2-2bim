# DHCP

## Instalação

sudo apt update (atualizar)
apk add install dnsmasq

## Configuração
nano /etc/dnsmasq.d/asa.conf

. Dentro desse arquivo, coloca uma parte da configuração!

### Configuração do DHCP
dhcp-range=192.168.13.10,192.168.13.100,255.255.255.0,12h




Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Distribuir um intervalo (*range* em inglês) de endereços IP; (15 pontos)
- Reservar 2 endereços (IP fixo) fora do intervalo do item anterior. (5 pontos)

## Teste


