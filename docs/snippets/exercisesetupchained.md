```{r prepare-flights}
nycflights <- nycflights13::flights
```

```{r filtered-flights, exercise.setup = "prepare-flights"}
# Change the filter to select February rather than January
flights_february <- filter(nycflights, month == 2)
```

```{r arrange, exercise=TRUE, exercise.setup = "filtered-flights"}
# Change the sort order to Ascending
arrange(flights_february, desc(arr_delay))
```