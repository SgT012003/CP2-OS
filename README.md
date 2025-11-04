# CP2-OS (IIS)

Integrante
|Nome|RM|
|:-:|:-:|
|Victor Didoff|552965|

## Indice

1. [Instalacao](#instalacao)
2. [Configuracao](#configuracao)
3. [Acesso](#acesso)

## Instalacao

1. Atravez dos Recursos

    Ativar e Desativar Recursos do Windows -> Servicos de Informacoes da Internet (Marcar) -> Aplicar

2. Atravez do PowerShell 4.x ou Acima

    ```bash
    Install-WindowsFeature -Name Web-Server -IncludeManagementTools
    ```

## Configuracao

1. Acessar ao Gerenciador do IIS

    `Win + R` -> `inetmgr`

2. Acessar ao Pools de Aplicativo

3. Criar um novo pool

4. Acessar ao sites

5. Criar um novo site / role

```log
Nome -> Desejado
Pool -> Selecionar o Novo Pool
Caminho fisico -> Pasta com o `index.html`
Porta -> (80 para http, 443 para https (precisa de certificad))
Nome do Host -> Localhost com inuito de teste mas em producao seria o dominio registrado no dns center
```

## Acesso

**[localhost](http://localhost)**
