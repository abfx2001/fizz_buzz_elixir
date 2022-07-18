
# Fizz Buzz

Olá a todos!
Essa é o meu primeiro programa feito em Elixir e 
comecei a estudar essa linguagem por curiosidade a 
respeito da programação funcional, é bem divertido e 
interessante, vou continuar a estudar para ver se
realmente vou utilizar essa linguagem para minha vida
profissional.
## Aprendizado

- Uso de Pattern Matching
- Uso de Pipe Operator
- Leitura de Arquivo
- Tratamento de dados
- Explorando as funcionalidades da linguagem

## Documentação da Aplicação

#### Função principal

```http
  FizzBuzz.build()
```

| Parâmetro   | Tipo       | Descrição                           |
| :---------- | :--------- | :---------------------------------- |
| `números inteiros separados por ","` | `.txt` | O programa irá fazer a leitura do arquivo |

#### Retorna uma lista

```http
  {:ok, [1, 2, :Fizz, 4, :Buzz, :FizzBuzz]}
```

O programa transforma uma lista de `String` para uma lista de `int`
e no lugar onde um número é divisível por `3`, troca-se o valor por `:Fizz`, onde é divisível por `5`,
troca-se o valor por `Buzz` e quando é divisível por `3 e 5`, troca-se o valor por `:FizzBuzz`.
| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `divisível por 3`      | `int` | O programa retorna `:Fizz` no lugar do número |
| `divisível por 5`      | `int` | O programa retorna `:Buzz` no lugar do número |
| `divisível por 3 e 5`      | `int` | O programa retorna `:FizzBuzz` no lugar do número |
| `não divisível por 3 ou 5`      | `int` | O programa retorna o próprio número |





## Uso/Exemplos
Um pouco do uso do Pattern Match e do Pipe Operator.

```Elixir
 defp handle_file_read({:ok, result}) do
    result =
      result
      |> String.split(",")
      |> Enum.map(&convert_and_evaluate_numbers/1)
    {:ok, result}
  end
```


## Rodando os testes

Para rodar os testes, rode o seguinte comando via bash

```bash
  mix test
```


## Documentação

[Documentação](https://elixir-lang.org/docs.html)


## Autores

- [@abfx2001](https://www.github.com/abfx2001)

