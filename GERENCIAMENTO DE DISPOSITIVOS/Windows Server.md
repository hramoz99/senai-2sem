# Parâmetros - Windows Server


**Acessar o servidor via RDP - Conexão da Área de Trabalho Remota**
```
User: .\[nome-do-usuário]
User: [domínio]\[nome-do-usuário]
```

**Informações do seu servidor**
```
Windows + PauseBreak
```

**Mudar o nome do servidor**
```
Windows + R
    digite sysdm.cpl
```

**Informações de rede - servidor**
```
Windows + R
    digite ncpa.cpl
```

**Acessar GPO**
```
Windows + R
    digite secpol.msc
```

**Acessar gerenciamento de disco**
```
Windows + R
    digite diskmgmt.msc
```

## Acessar pasta compartilhada
```
Abra o Explorador de Arquivos
    
    * digite \\localhost (caso a pasta esteja diretamente atrelada neste servidor)
    * digite \\[nome-do-servidor-de-arquivos] (caso a pasta esteja sob controle de outro servidor)
    * digite \\[ip-do-servidor-de-arquivos] (caso a pasta esteja sob controle de outro servidor)

```

**Caminho do arquivo hosts**
```
Windows + R
    digite C:\Windows\System32\drivers\etc\hosts
```

**Gerenciador de DNS**
```
Windows + R
    digite dnsmgmt.msc
```

**ISS - Serviços de Informações da internet**
```
Windows + R
    digite InetMgr.exe
```
