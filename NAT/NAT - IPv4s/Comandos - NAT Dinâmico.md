## NAT - DINÂMICO


**Os endereços são definidos pela indicação do endereço IPv4 inicial e endereço IPv4 final do pool.**

```
(config)#ip nat pool [name] [primeiro-ip-da-rede] [ultimo-ip-da-rede] netmask [máscara]
```

**Configurar uma ACL padrão para permitir os endereços que devem ser convertidos**


```
(config)#access-list [1-99] [deny or permit] [endereço-ip] [wildcard]
```

**Estabelecer a conversão dinâmica de origem, especificando a lista de acesso e o pool**


```
(config)#ip nat inside source list [número-da-acl] pool [name]
```

**Marcar a interface conectada internamente**

```
(config-if)ip nat inside
```

**Marcar a interface conectada externamente**

```
(config-if)ip nat outside
```

**Remover conversões de NAT**

```
#clear ip nat translations *
```

**Exibir as conversões ativas de NAT**

```
#show ip nat translations
```

**Exibir informações sobre o número total de conversões ativas**

```
#show ip nat statistics
```

**Eliminar as estatísticas e as entradas**

```
#clear ip nat statistics
#clear ip nat translation *
```

**Verificar a operação do recurso NAT exibindo as informações sobre cada pacote que está sendo convertido pelo roteador**

```
#debug ip nat
#debug ip nat detailed 
```

