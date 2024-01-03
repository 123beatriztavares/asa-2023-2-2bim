# SMB

O Samba é um software de código aberto que permite a interoperabilidade entre sistemas Unix/Linux e Windows. Ele atua como um servidor que pode comunicar-se com protocolos de rede da Microsoft, fornecendo funcionalidades como compartilhamento de arquivos e impressoras, autenticação e autorização de usuários, entre outros serviços. 


## Instalação
>apk add samba

. Foi ultilizado o comando:(samba-tool domain provision -use-rcf2307 - interactive), isso para poder levantar o domínio (noronha).

. Crio as pastas das familias que vou compartilhar.

>Pastas /srv/samba/(tavares, barbosa)

. Em seguida é preciso entrar no arquivo (smb.conf), que se encontra na pasta (/etc/samba/), dentro desse arquivo fiz as demais configurações.

## Configuração
>nano /etc/samba/smb.conf

. Fazer as demais configurações!

[![Screenshot_2023-12-04_21-07-12](https://i.im.ge/2024/01/03/3MclFG.Screenshot-2023-12-04-21-07-12.png)](https://im.ge/i/3MclFG)

 
Isso tudo dentro da máquina xarope, em seguida foi iniciado a máquina windows com a conta admin e configurei a placa de rede local 1 que é rede interna.

( rede interna: intnet)
 
Configurei a placa com o ip da máquina linux,entrei na ferramenta usuários e pcs do AD, e criei as famílias e grupos pelo Activedirectory.

[![Screenshot_2023-12-04_21-03-34](https://i.im.ge/2024/01/03/3Mg1KP.Screenshot-2023-12-04-21-03-34.png)](https://im.ge/i/3Mg1KP)
 
>Criei duas pastas Norte, Sul.


### 2 grupos para dois de meus sobrenomes!




1. barbosa
2. tavares

### 4 usuários, dois para cada um dos sobrenomes!
[![usuários](https://i.im.ge/2024/01/03/3Mg308.usuarios.png)](https://im.ge/i/3Mg308)


1. Bianca Tavares
2. Bruna Tavares
3. Carlos Barbosa 
4. Maria Barbosa

### 3 Compartilhar duas pastas de seus sobrenomes!

[![Screenshot_2023-12-04_21-00-56](https://i.im.ge/2024/01/03/3MgvMm.Screenshot-2023-12-04-21-00-56.png)](https://im.ge/i/3MgvMm)

1. barbosa
2. tavares

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

1. Criar 2 grupos para dois de seus sobrenomes;
2. Criar 4 usuários, dois para cada um dos sobrenomes;
3. Compartilhar duas pastas com dois de seus sobrenome, compartilhado para o grupo com o sobrenome correspondente.

## Teste
[![Screenshot_2023-12-04_21-01-59](https://i.im.ge/2024/01/03/3MgGdT.Screenshot-2023-12-04-21-01-59.png)](https://im.ge/i/3MgGdT)


. Quando acessar um grupo a pasta estará vazia e a outra pasta vai pedir senha.