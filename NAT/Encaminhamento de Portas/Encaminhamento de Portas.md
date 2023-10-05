## ENCAMINHAMENTO DE PORTA

#### Comunicação Estática entre um endereço local interno, um endereço global interno e a porta global

```
(config)#ip nat inside source [static (tcp or udp)] [ip-local-interno] [porta-local] [ip-global-interno] [porta-global]
```

#### Identificar a interface interna NAT

```
(config)#int [id-da-interface-interna]
(config-if)#ip nat inside
```

#### Identificar a interface externa de NAT

```
(config)#int [id-da-interface-externa]
(config-if)#ip nat outside
```

#### Verificar o encaminhamento de portas

```
#sh ip nat translations
