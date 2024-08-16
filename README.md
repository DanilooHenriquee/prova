### 1. Como você cria um array em PHP e quais os diferentes tipos de array vc conhece?

### 2. Explique o que são sessões em PHP e como você as utiliza.

### 3. Qual é a diferença entre include e require em PHP?

### 4. Analise o codigo abaixo:
```php
function updateValue(&$value) {
    $value *= 2;
}

$a = 5;
updateValue($a);
echo $a;
```

>a. O que o código imprime e por quê?
>
>b. Explique o papel do operador `&` na função updateValue.
>
>c. O que aconteceria se a função updateValue não utilizasse o operador `&`?
 
 
### 5. Analise o codigo abaixo:
```php
class Calculator {
    private $value = 0;

    public function add($num) {
        $this->value += $num;
    }

    public function getValue() {
        return $this->value;
    }
}

$calc = new Calculator();
$calc->add(10);
$calc->add(5);
echo $calc->getValue();
```
>a. O que o código imprime e como a classe Calculator manipula o valor?
>
>b. Qual é a importância do modificador de acesso `private` para a propriedade `$value`?
>
>c. O que aconteceria se o modificador de acesso de `$value` fosse alterado para `public`?



### 6. Analise o codigo abaixo:
```php
class Counter {
    private static $count = 0;

    public static function increment() {
        self::$count++;
    }

    public static function getCount() {
        return self::$count;
    }
}
```

>a. Qual é a forma para acessar o valor de `$count`
>
>b. Refatore a função increment para permitir um valor opcional como parâmetro. Se nenhum valor for fornecido, a função deve continuar incrementando da forma atual.

### 7. Analise o codigo abaixo:
```php
$venda = [
    'cliente' => [
        'nome' => 'Alice', 
        'cpf' => '123.456.789.56'
    ],
    'produtos' => [
        ['codigo' => '111', 'descricao' => 'Mouse', 'valor' => 15.90],
        ['codigo' => '222', 'descricao' => 'Teclado', 'valor' => 79.80],
        ['codigo' => '333', 'descricao' => 'Monitor', 'valor' => 299.99],
    ]
];
```

>a. Crie uma função para retornar o somatório da venda
>
>b. Utilizando as implementações acima, imprima a mensagem a baixo:
// "A cliente <nomeCliente>, cpf: <cpf> realizou uma compra no valor R$ <somatorio>"


### 8. Crie uma função que receba uma lista de números e retorne uma nova lista contendo apenas os números pares da lista original, mas em ordem inversa.
>Exemplo: [1, 2, 3, 4, 5, 6]
>
>Saída: [6, 4, 2]

### 9. Você tem um array de inteiros. Escreva um algoritmo para encontrar o número que aparece mais vezes no array. Se houver um empate, retorne o menor número.
>Entrada: [1, 2, 2, 3, 3, 3, 4, 4, 4, 4]
>
>Saída: 4

### 10. Dado um array de números inteiros [5, 9, 1, 5, 6, 2], escreva um código que ordene os elementos do array em ordem crescente. Em seguida, retorne o segundo menor número no array ordenado.

