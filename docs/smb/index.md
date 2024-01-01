# SMB

## Instalação
apk add samba

. Foi ultilizado o comando: samba-tool domain provision -use-rcf2307 - interactive, isso para poder levantar o domínio (noronha).

. Crio as pastas das familias que vou compartilhar.

Pastas /srv/samba/(tavares, barbosa)

. Em seguida é preciso entrar no arquivo (smb.conf), que se encontra na pasta (/etc/samba/), dentro desse arquivo fiz as demais configurações.

## Configuração
/etc/samba/smb.conf

. Fazer as demais configurações!

[Title](https://im.ge/i/Captura-de-Tela-6.xnW5PG)
 
Isso tudo dentro da máquina xarope, em seguida foi iniciado a máquina windows com a conta admin e configurei a placa de rede local 1 que é rede interna.

( rede interna: intnet)
 
Configurei a placa com o ip da máquina linux,entrei na ferramenta usuários e pcs do AD, e criei as famílias e grupos pelo Activedirectory.

[Title](https://im.ge/i/Captura-de-Tela-8.xnK4nT)
 
Criei duas pastas Norte, Sul.


### 2 grupos para dois de meus sobrenomes!

[Title](https://im.ge/i/Captura-de-Tela-9.xnVxtc)

1. barbosa
2. tavares

### 4 usuários, dois para cada um dos sobrenomes!
[Title](https://im.ge/i/Captura-de-Tela-9.xnfhXa)


1. Bianca Tavares
2. Bruna Tavares
3. Carlos Barbosa 
4. Maria Barbosa

### 3 Compartilhar duas pastas de seus sobrenomes!

[Title](https://im.ge/i/Captura-de-Tela-10.xnkNEW) 

1. barbosa
2. tavares

Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

1. Criar 2 grupos para dois de seus sobrenomes;
2. Criar 4 usuários, dois para cada um dos sobrenomes;
3. Compartilhar duas pastas com dois de seus sobrenome, compartilhado para o grupo com o sobrenome correspondente.

## Teste


[Title](https://im.ge/i/Captura-de-Tela-12.xnzmFK)


Quando acessar um grupo a pasta estará vazia e a outra pasta vai pedir senha.