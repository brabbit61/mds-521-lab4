NewFile
================
Jenit Jain
2022-09-26

## Data Types

Data structures are very important to understand because these are the
objects you will manipulate on a day-to-day basis in R. Dealing with
object conversions is one of the most common sources of frustration for
beginners. Everything in R is an object.

R has 5 basic data types.

- character
- numeric (real or decimal)
- integer
- logical
- complex

``` r
i <- 1L
b <- TRUE

paste0(i, " is of type ", class(i))
```

    ## [1] "1 is of type integer"

``` r
paste0(b, " is of type ", class(b))
```

    ## [1] "TRUE is of type logical"

## Lists and Vectors

A vector is a one dimensional array of elements. Vectors are the basic
building blocks of R. Almost all data in R is stored in a vector, or
even a vector of vectors.

Lists are one of the most flexible data structures in R. As a result,
they are used as a general purpose glue to hold objects together. You
will find lists disguised as model objects, data frames, list-columns
within data frames, and more. A list is a recursive vector: a vector
that can contain another vector or list in each of its elements.

``` r
list1 <- list(1, "Jenit", "MDS", TRUE)
vec1 <- c(1, 2, 3, 4, "Jenit")
```

``` r
print("The list is: ")
```

    ## [1] "The list is: "

``` r
list1
```

    ## [[1]]
    ## [1] 1
    ## 
    ## [[2]]
    ## [1] "Jenit"
    ## 
    ## [[3]]
    ## [1] "MDS"
    ## 
    ## [[4]]
    ## [1] TRUE

``` r
print("The vector is: ")
```

    ## [1] "The vector is: "

``` r
vec1
```

    ## [1] "1"     "2"     "3"     "4"     "Jenit"

A list can contain elements of different datatype where a vector coerces
the data types of its elements so that all the elements in the vector
have the same data type
