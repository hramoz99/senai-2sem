## PAT - Pool de Endereços

**Definir um pool de endereços globais a serem usados para conversão de sobrecarga**

```
(config)#ip nat pool [name] [intervalo-de-IPs] netmask [máscara]
```

**Configurar uma ACL padrão para permitir os endereços que devem ser convertidos**
```
(config)#access-list [1-99] [deny or permit] [endereço-ip] [wildcard]
```

**Estabelecer a conversão de sobrecarga, especificando a lista de acesso e o pool**

```
(config)#ip nat inside source list [número-da-acl] pool [name] overload
```

**Marcar a interface conectada internamente**

```
(config-if)ip nat inside
```

**Marcar a interface conectada externamente**

```
(config-if)ip nat outside
```

**Eliminar as estatísticas e as entradas**

```
#clear ip nat statistics
#clear ip nat translation *
```

**Exibir as conversões ativas de NAT**

```
#show ip nat translations
```

**Exibir informações sobre o número total de conversões ativas**

```
#show ip nat statistics
```

## PAT - Endereço único

**Configurar uma ACL padrão para permitir os endereços que devem ser convertidos**

```
(config)#access-list [1-99] [deny or permit] [endereço-ip] [wildcard]
```

**Estabelecer a conversão dinâmica de origem, especificando as opções de ACL, interface de saída e sobrecarga**

```
(config)#ip nat inside source list [1-99] interface [id-da-interface] overload
```

**Marcar a interface conectada internamente**

```
(config-if)ip nat inside
```

**Marcar a interface conectada externamente**

```
(config-if)ip nat outside
```

**Eliminar as estatísticas e as entradas**

```
#clear ip nat statistics
#clear ip nat translation *
```

**Exibir as conversões ativas de NAT**

```
#show ip nat translations
```

**Exibir informações sobre o número total de conversões ativas**

```
#show ip nat statistics
```

**Verificar a operação do recurso NAT, exibindo informações sobre cada pacote que está sendo convertido pelo roteador**

```
#debug ip nat
#debug ip nat detailed 
```
