## LLDP

#### Ativar o LLP nos dispositivos CISCO

> Para desativar o LLDP, insira o comando 'no lldp run'

```
(config)#lldp run 
```

#### Transmissão e recebimento de pacotes LLDP

```
(config-if)#lldp transmit
(config-if)#lldp receive
``` 

#### Verificar o LLPD 

```
#show lldp
```

#### Detecção de vizinhos

```
#show lldp neighbors [detail]
```
