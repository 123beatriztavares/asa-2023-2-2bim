# LDAP
O LDAP (Lightweight Directory Access Protocol) é um protocolo de aplicação utilizado para acessar e manter serviços de diretório de forma eficiente e padronizada. Ele foi projetado para ser uma versão mais leve do protocolo Directory Access Protocol (DAP), usado anteriormente.


## Instalação

Para instalar esse serviço foi ultizado o samba como base:
O comando para instalar o samba!
> apk add samba



## Configuração

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

- Criar duas OU: `vendedores` e `rh`;
- Mover o grupo `sobrenome1` e seus membros para a OU `vendedores`;
- Mover os grupo `sobrenome2` e seus membros para a OU `rh`.

> Criar duas OU: vendedores e rh.

>Para poder criar essas duas OU foi preciso entrar dentro da máquina windows disponibilizada pelo o professor e lá em usuários de computadores do active directory e criar elas.


[![Screenshot_2024-01-03_18-41-57](https://i.im.ge/2024/01/04/3XfcU4.Screenshot-2024-01-03-18-41-57.png)](https://im.ge/i/3XfcU4)


> Grupo sobrenome1 e seus membros para a OU vendedores.


> Após ser criadas as OU, tive que criar um grupo com meu sobrenome e colocar os mesmo desse grupo dentro da OU vendedores.

[![LDAP](https://i.im.ge/2024/01/04/3XffOf.LDAP.png)](https://im.ge/i/3XffOf)

> Grupo sobrenome2 e seus membros para OU rh.

> Após ser criadas as OU, tive que criar um grupo com meu sobrenome e colocar os mesmo desse grupo dentro da OU rh

[![ldap](https://i.im.ge/2024/01/04/3XkPiW.ldap.png)](https://im.ge/i/3XkPiW)
## Teste

 > vendedores

[![Screenshot_2024-01-03_18-50-43](https://i.im.ge/2024/01/04/3XzsJL.Screenshot-2024-01-03-18-50-43.png)](https://im.ge/i/3XzsJL)

> rn

[![Screenshot_2024-01-03_18-52-12](https://i.im.ge/2024/01/04/3XzDNx.Screenshot-2024-01-03-18-52-12.png)](https://im.ge/i/3XzDNx)
