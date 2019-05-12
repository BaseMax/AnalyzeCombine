# AnalyzeCombine

Analyze the combine with and without the repetition.

# Structure

## `Combine`

```
array Combine(array $input);
```

List of all of the probability of the combine without repetition.

------------

## `CombineLimit`

```
array CombineLimit(array $input, int $limit);
```

List of all of the probability of the combine without repetition with limitation.

------------

### `CombineRepeat`

```
array CombineRepeat(array $input);
```

List of all of the probability of the combine with repetition.

------------

### `CombineRepeatLimit`

```
array CombineRepeatLimit(array $input, int $limit);
```

List of all of the probability of the combine with repetition with limitation.

------------


## `CustomCombine`

```
array CustomCombine(array $input);
```

List of all of the probability of the combine from custom values. (Favorable values with keeping position)

Demo :

```php
$count=NCustomCombine([ ['x','y'] , ['x','y'] , ['x','y'] ]);
print $count; // 8
```

```php
$array=CustomCombine([ ['x','y'] , ['x','y'] , ['x','y'] ]);
print_r($array);
```

```
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
