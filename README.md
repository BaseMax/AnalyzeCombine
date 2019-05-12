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

