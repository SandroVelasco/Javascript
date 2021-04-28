# Introdução
Criei esse documento para facilitar o entendimento e o estudo de regex. Todo o conteúdo foi retirado de codecademy.com.

## `|` Alternation
A alternância, realizada em expressões regulares com o símbolo de barra vertical |, permite-nos fazer a correspondência entre os caracteres que precedem `|` e os caracteres após `|`. A regex `baboons|gorillas` irá corresponder baboons no texto I love baboons, mas também irá corresponder gorillas no texto I love gorillas.

**Exemplo de uso:** `baboons|gorillas // lê-se procure baboons ou gorillas no texto.`

## `[]` Conjunto de caracteres
Todos os caracteres dentro de `[]` serão opções para formação da palavra.

**Exemplo de uso:** `ba[cb]oon // match: bacoon / baboon`

## `[^xyz]` Negação
Todos os caracteres dentro de [] serão negados por conta do simbolo ^.

**Exemplo de uso:** ba[^cb]oon // match everything but not bacoon / baboon

## `.` Curinga
Combina com qualquer caracter único.

**Exemplo de uso:**
.... // Combina com qualquer palavra com 4 caracteres. 
Eu comi . bananas // Combina com, por exemplo: Eu comi 3 bananas.

Para usar o ponto no texto, invés do símbolo coringa, adicionar: \. (\ = escape character)

## `-` Range/Intervalo
Especifica um intervalo de caracteres.

**Exemplo de uso:** Eu adotei [0-9] cães. // Combinará com eu adotei 0 a 9 cães.

## Classes de caracteres abreviados
`\w` (caractere de palavra): Corresponde a qualquer caracter de palavra - caracter maiúsculo, minúsculo, digito ou sublinhado.
`\d` (caractere de dígito): Corresponde a qualquer dígito - número. 
`\s` (caractere de espaço em branco): Corresponde a - espaço, tab, \r\n, form feed ou vertical tab

**Exemplo de uso:**
`\d\s\w\w\w\w\w\w\w` corresponde a um dígito, seguido por um espaço, seguido por 7 caracteres. Match 3 monkeys

## Negação de caracteres abreviados
`\W` (não-caractere de palavra)
`\D` (não-caractere dígito)
`\S` (não-caractere whitespace)

**Exemplo de uso:** Não necessário.

## `()` Grouping
Permite agrupar partes de uma expressão regular e permite limitar alternation para parte da regex.

**Exemplo de uso:** I love (baboons|gorillas) corresponde a I love baboons ou I love gorillas

## `{}` Quantificadores - Fixo
Para evitar ter que digitar \w\w\w\w\w\s\w\w\w\w\w os quantificadores entram em ação.

**Exemplo de uso:**
\w{3} corresponde a \w\w\w
\w{4,7} corresponde a no mínimo \w\w\w\w e no máximo \w\w\w\w\w\w\w
roa{3}r corresponde a roaaar
roa{3,}r quando o valor máximo não é especificado, ele é infinito.

Vale ressaltar que quantificadores são gananciosos. Isso significa que eles sempre vão escolher corresponder com a palavra que tiver o máximo definido.

## `?` Quantificadores - Opcional
Permite especificar um caracter opcional.

**Exemplo de uso:** `humou?r` corresponde a humor ou humour

## Quantificadores - 0 ou mais, 1 ou mais
`*`: 0 ou mais
`+`: 1 ou mais

**Exemplo de uso:**
`meo*w`: Corresponde a mew, ou meoooow, ou meooooooow.
`meo+w`: Correspond ea meow, meoooooow, meooooooooow.

## Âncoras
`^`: Corresponde se a palavra estiver no início do texto
`$`: Corresponde se a palavra estiver no final do texto

**Exemplo de uso:**
`^Sandro é lindo$` corresponde a Sandro é lindo, mas não corresponde a O Sandro é lindo demais.
