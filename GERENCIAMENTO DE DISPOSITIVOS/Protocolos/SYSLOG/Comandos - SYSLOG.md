## SYSLOG

#### Forçar eventos registrados a exibirem a data e hora

> Palavra-chave 'datetime' - relógio configurado manualmente

```
(config)#service timestamps log datetime
ou
(config)#service timestamps log datetime msec
```

#### Armazenar as mensagens de log por padrão

> Oss comandos devem seguir essa ordem

```
(config)#logging console
(config)#logging buffered
```

#### Exibir as configurações de serviço de logging padrão

```
#sh logging
```

## Comandos do roteador e do switch para clientes de Syslog

> São necessários três passos para que o roteador envie mensagens do sistema a um Servidor syslog, onde elas podem ser armazenadas, 
filtradas e analisadas:

#### PASSO 1
**Configurar o nome de host ou o endereço IPv4 do syslog** 

```
(config)#logging [endereço-ipv4-do-syslog]
ou
(config)#logging host [endereço-ipv4-do-host-de-syslog]
```

#### PASSO 2 
**Controlar as mensagens enviadas ao Servidor**

```
(config)#logging trap [nível]
```

#### PASSO 3
**Configurar a interface de origem**

```
(config-if)#logging source-interface [id-da-interface]
```

#### PASSO 4
**Filtrar as saídas de syslog**

*Exemplo*

#show logging | include changed state to up
#show logging | begin Jun 12 22:35

```
#sh logging | [parâmetro]
```
