## CDP

#### Exibir informações e verificar o status 

```
#show cdp
```

#### Ativar o CPD em todas interfaces do dispositivo 

> Para desativa-lo, basta colocar o parâmetro "no" antes do comando

```
(config)#cdp run
```

#### Desativar o CPD de uma interface 

> Para ativar, basta retirar o "no"

```
(config-if)#no cdp enable
``` 

#### Exibir lista dos vizinhos e status  

```
#show cdp neighbors [detail]
```

#### Exibir interface ativadas 

```
#show cdp interface
```

