# AnalyzeCombine

Analyze the combine with and without the repetition.

# Initialise

```php
$combine=new AnalyzeCombine();
```

# Structure

## `Combine`

```php
array Combine(array $input);
```

List of all of the probability of the combine without repetition.

------------

## `CombineLimit`

```php
array CombineLimit(array $input, int $limit);
```

List of all of the probability of the combine without repetition with limitation.

------------

### `CombineRepeat`

```php
array CombineRepeat(array $input);
```

List of all of the probability of the combine with repetition.

------------

### `CombineRepeatLimit`

```php
array CombineRepeatLimit(array $input, int $limit);
```

List of all of the probability of the combine with repetition with limitation.

------------


## `CustomCombine`

```php
array CustomCombine(array $input);
```

List of all of the probability of the combine from custom values. (Favorable values with keeping position)

Demo :

```php
$count=$combine->NCustomCombine([ ['x','y'] , ['x','y'] , ['x','y'] ]);
print $count; // 8
```

```php
$array=$combine->CustomCombine([ ['x','y'] , ['x','y'] , ['x','y'] ]);
print_r($array);
```

```php
Array
(
    [0] => Array
        (
            [0] => x
            [1] => x
            [2] => x
        )

    [1] => Array
        (
            [0] => x
            [1] => x
            [2] => y
        )

    [2] => Array
        (
            [0] => x
            [1] => y
            [2] => x
        )

    [3] => Array
        (
            [0] => x
            [1] => y
            [2] => y
        )

    [4] => Array
        (
            [0] => y
            [1] => x
            [2] => x
        )

    [5] => Array
        (
            [0] => y
            [1] => x
            [2] => y
        )

    [6] => Array
        (
            [0] => y
            [1] => y
            [2] => x
        )

    [7] => Array
        (
            [0] => y
            [1] => y
            [2] => y
        )

)
```
