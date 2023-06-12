Basic Concept
-------------
The basic concept is that computing Big-decimal structure is slower than computing multiple integers.

First, create a structure with two lists of integers.
Second, the first list of int is the integer part and the other is the decimal part.
Third, when you initialize the structure with examples of strings, floats, and integers, it performs a modulo operation (mod 10^(9*n)) and stores the numbers according to some rules.

# Example

> str s = "00000123123456789.987654321987000"
> a = HyperDecimal.init(s)
> print_info(a)
> print(a)

### output:
> int_list : [123456789,123]
> decimal_list : [987654321,987000000]
> 123123456789.987654321987

