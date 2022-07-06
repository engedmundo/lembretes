# Linguagem YAML
É uma linguagem de serialização e deserialização de dados, usada para efetuar configurações de docker e kubernets, entre outras.

## Sintaxe básica
* conjuntos de chave-valor, separados por dois pontos
* `host: amazon`
```
  datacenter:
    location: São Paulo
    router: 42
```
* Não utiliza de vírgulas no finaldas instruções
* Listas são indicadas por hifen no início da instrução:
```
roles:
  - web
  - dns
```

## Estilos
São dois estilos básicos - Block e Flow
* **Block:** semelhante a um objeto, separado por identação de dois espaços
* **Flow:** semelhante a um objeto JSON, com abertura de chaves para aninhar objetos, colchetes para aninhar listas, etc.

## Comentários:
* Comentários de uma linha são feitos com # e um espaço

## Mapeamento: 
* Representado por dois pontos e espaço (: ), semelhante a definição de objetos em um dict python
* Elementos de chave e valor

## Sequências
* Listas, arrays, coleções, ou uma mistura destes, etc

## Escalares
* Números, constantes, strings, inteiros, etc
* Não é obrigatório o uso de aspas duplas ou simples para indicar strings
* Se um valor não for usada em uma computação, é preferível defini-lo como string
* Valores de multiplas linhas:
```
funcionamento: |
  segunda - das 08:00 as 17:00
  terça   - das 08:00 as 18:00
````

## Estruturas
* Separação do conteudo semelhante a seções
* Indicado por três traços simples `---`

## Tags:
* etiquetas
```
%TAG ! tag:host:amazon:
---
host: amazon
datacenter:
  - location: !AMAZON São Paulo
```

## Âncoras
* Semelhante a variáveis
* São definidas com e comercial (&)
* São usadas com o asterisco
```
datacenter:
  - location: &SP São Paulo
---
datacenter:
  - location: *SP
```
