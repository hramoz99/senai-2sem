## NTP

#### Definir o horário MANUALMENTE 

*Exemplo*
- clock set 20:36:00 dec 11 2015

```
#clock set [hh:mm:ss] {mmm (em-inglês | apenas as 3 primeiras letras)} [dd] [aaaa]
```

#### Indicicar o número de saltos de NTP - FONTE AUTORITATIVA

```
(config)#ntp master [nível-de-stratum]
```

#### Configurar NTP 

```
(config)#ntp server [endereço-ip]
```

#### Atualizar o calendário

```
(config)#ntp update-calendar
```

#### Definição do fuso horário

*Exemplo*

- (config)#clock timezone PST -8

```
(config)#clock timezone [fuso] [gmt]
```

#### Definir para horário VERÃO 

```
(config)#clock summer-time PDT recurring
```

#### Exibir a hora atual

```
#show clock [detail]
```

#### Exibir informações 

```
#show ntp associations
#show ntp status
```
