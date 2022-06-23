## BACKUP DA IMAGEM DO IOS

#### Teste de conectividade no servidor TFTP

```
#ping [endereço-ip-do-servidor]
```

#### Verificação de espaço para acomodar a imagem do software IOS Cisco

```
#show flash0
```

#### Copiar as configurações para o servidor TFTP

```
#copy flash0: tftp:
[nome-do-arquivo]
[endereço-ip-do-servidor]
```

#### Copiar o arquivo de imagem do servidor TFTP para o dispositivo

```
#copy tftp: flash0:
[nome-do-arquivo]
[endereço-ip-do-servidor]
```

#### Atualizar a imagem do IOS Cisco

```
(config)#no boot system
(config)#boot system flash: [nome-da-imagem]
#copy running-config startup-config
#reload
```

#### Verificação da imagem carregada

```
#sh version
```
