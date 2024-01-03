# DNS

O DNS, ou Sistema de Nomes de Domínio, é um sistema de nomeação hierárquico e distribuído para computadores, serviços ou qualquer recurso conectado à Internet ou a uma rede privada. Ele traduz nomes de domínio legíveis por humanos em endereços IP numéricos, que são usados pelos computadores para se identificarem na rede.



## Instalação

Para poder ser feito essa instalação, fiz uma conexão por meio do samba entre um cliente Windows e um servidor Linux Alpine, pois atrás deles é que poderá fazer as configurações.

## Configuração


Incluir o(s) nome(s) e o conteúdo do(s) arquivo(s) de configuração.

>Baixando o contênier e lá peguei o ip para poder colocar no Host (A) do dns

Cinco registros (4 pontos cada):

- 3 do tipo A (Endereços);

> noronha

> peru

> recife

- 2 do tipo CNAME (`www` e `docs`);

> docs

> www

[![Screenshot_2024-01-03_19-47-05](https://i.im.ge/2024/01/04/3XJf1L.Screenshot-2024-01-03-19-47-05.png)](https://im.ge/i/3XJf1L)


## Teste
 Para fazer o teste é necessário pigar na máquina!

[![Screenshot_2024-01-03_19-37-22](https://i.im.ge/2024/01/04/3XnnrP.Screenshot-2024-01-03-19-37-22.png)](https://im.ge/i/3XnnrP)

> Contênier que foi criado!

[![Screenshot_2024-01-03_19-47-20](https://i.im.ge/2024/01/04/3Xn451.Screenshot-2024-01-03-19-47-20.png)](https://im.ge/i/3Xn451)

