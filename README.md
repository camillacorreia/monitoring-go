## Go - Conceitos Iniciais

<img src="./github/go-logo.png" width="200px" >

----

#### Tipos de Variáveis

```go
package main

import "fmt"

func main() {
    var nome string = "Douglas"
    var versao float32 = 1.1
    fmt.Println("Olá sr.", nome)
    fmt.Println("Este programa está na versão", versao)
}
```

Variável sem valor atribuído
- Quando não atribuímos um valor a uma variável, ela assume um valor zerado, ou seja, se for um inteiro, seu valor será 0, se for um número flutuante, seu valor será 0.0, e se for uma string, seu valor será uma string vazia.
```go
package main

import "fmt"

func main() {
    var nome string = "Douglas"
    var idade int
    var versao float32 = 1.1
    fmt.Println("Olá sr.", nome, "sua idade é", idade)
    fmt.Println("Este programa está na versão", versao)
}
```

Não utilização de uma variável
- Não podermos declarar uma variável e não utilizá-la.

#### Inferindo os tipos das variáveis

```go
package main

import "fmt"
import "reflect"

func main() {
    var nome = "Douglas"
    var idade = 24
    var versao = 1.1
    fmt.Println("Olá sr.", nome, "sua idade é", idade)
    fmt.Println("Este programa está na versão", versao)

    fmt.Println("O tipo da variável idade é", reflect.TypeOf(versao))
}
```

#### Declaração curta de variáveis

```go
package main

import "fmt"

func main() {
    nome := "Douglas"
    idade := 24
    versao := 1.1
    fmt.Println("Olá sr.", nome, "sua idade é", idade)
    fmt.Println("Este programa está na versão", versao)
}
```