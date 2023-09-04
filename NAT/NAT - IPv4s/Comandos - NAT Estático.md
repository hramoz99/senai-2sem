## NAT - ESTÁTICO


**Conversões de NAT estático são usadas geralmente quando os clientes da rede externa (Internet) precisam acessar servidores da rede interna.**


```
(config)#ip nat inside source static [ip-local] [ip-global]
```

**Marcar a interface conectada internamente**

```
(config-if)ip nat inside
```

**Marcar a interface conectada externamente**

```
(config-if)ip nat outside
```

**Exibir as conversões ativas de NAT**

```
#show ip nat translations
```

**Exibir informações sobre o número total de conversões ativas**

```
#show ip nat statistics
```

**Verificar a operação do recurso NAT exibindo informações sobre cada pacote que está sendo convertido pelo roteador**

```
#debug ip nat
#debug ip nat detailed 
```
