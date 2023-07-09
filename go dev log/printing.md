# FORMATTING STRINGS IN GO

Go follows the [printf tradition](https://cplusplus.com/reference/cstdio/printf/) from the C language. In my opinion, string formatting/interpolation in Go is currently _less_ elegant than JavaScript and Python.

- [fmt.Printf](https://pkg.go.dev/fmt#Printf) - Prints a formatted string to [standard out](https://stackoverflow.com/questions/3385201/confused-about-stdin-stdout-and-stderr).
- [fmt.Sprintf()](https://pkg.go.dev/fmt#Sprintf) - Returns the formatted string

## EXAMPLES

These formatting verbs work with both `fmt.Printf` and `fmt.Sprintf`.

### %V - INTERPOLATE THE DEFAULT REPRESENTATION

The `%v` variant prints the Go syntax representation of a value. You can usually use this if you're unsure what else to use. That said, it's better to use the type-specific variant if you can.

```go
s := fmt.Sprintf("I am %v years old", 10)
// I am 10 years old

s := fmt.Sprintf("I am %v years old", "way too many")
// I am way too many years old
```

### `%S` - INTERPOLATE A STRING

```go
s := fmt.Sprintf("I am %s years old", "way too many")
// I am way too many years old
```

### `%D` - INTERPOLATE AN INTEGER IN DECIMAL FORM

```go
s := fmt.Sprintf("I am %d years old", 10)
// I am 10 years old
```

### `%F` - INTERPOLATE A DECIMAL

```go
s := fmt.Sprintf("I am %f years old", 10.523)
// I am 10.523000 years old

// The ".2" rounds the number to 2 decimal places
s := fmt.Sprintf("I am %.2f years old", 10.523)
// I am 10.53 years old
```

If you're interested in all the formatting options, feel free to take a look at the `fmt` package's [docs here](https://pkg.go.dev/fmt#hdr-Printing).

## ASSIGNMENT

Create a new variable called `msg` on line 9. It's a string that contains the following:

```
Hi NAME, your open rate is OPENRATE percent
```

Where `NAME` is the given `name`, and `OPENRATE` is the `openRate` rounded to the nearest "tenths" place.