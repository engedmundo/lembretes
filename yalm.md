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
* comentários de uma linha são feitos com # e um espaço
  