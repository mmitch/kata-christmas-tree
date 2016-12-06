# Christmas Tree programming kata

This is a quite simple kata that mostly involves string and text
processing.  It is similar to the _Diamond kata_.

## Goal of the kata

Build the text representation of a Christmas tree for a given tree
height.

A proper Christmas tree shall consist of these three parts:

* a star on top
* the green part inbetween _(if anybody has a nice word for this: let
  me know!)_
* a trunk

The Christmas tree shall be calculated for use with a fixed-with font
where every character has the same width, like in this string `"iiimmm"`.

## Tree height

The tree height shall have only one digit, so valid heights to
consider are in the range from `0` to `9`.

## Top star

On the top of the Christmas tree shall be an ornamental star,
represented by the character `*`.  The star shall be in the same
column as the trunk.

## The green part in the middle

The branches and needles of the Christmas tree shall consist of
multiple lines of text:

* The top line shall contain only the number `1`.
* The second line shall contain the number ``2`` two times, separated
  by a blank character.
* The third line shall contain the number ``3`` three times, again
  separated by blanks.
* And so on.

In the first line, the character ``1`` shall be in the same column as
the star and the trunk.  Further lines should grow in equal parts to
the left and right.

The height of this part is directly related to the tree height:

* A tree height of `0` gives no middle part at all.
* A tree height of `1` gives one line in the middle part consisting
  of the number `1`.
* A tree height of `2` gives two lines in the middle part consisting
  of one `1` and two `2`s.

A picture says more than 1000 words, please see the examples below.

## Trunk

The trunk is the naked part on the bottom of the tree.  It shall be
represented by the character `#`.  The trunk shall be located in the
same column as the star.

The trunk is always one line tall, even on the biggest of trees.

## Examples

Height 0:
```
*
#
```

Height 1:
```
*
1
#
```

Height 2:
```
 * 
 1 
2 2
 # 
```

Height 3:
```
  *  
  1  
 2 2 
3 3 3
  #  
```

Height 4:
```
   *   
   1   
  2 2  
 3 3 3
4 4 4 4
   #   
```

## Extra curriculum

* Build trees with two-digit heights.
  * Before you start: Which difficulties do you expect?
  * Which problems do you see when you generate a tree with height
    `10`?
  * How can you address those problems?
  * How does your existing design cope with the new requirements?

* Scale your trees up by one or more orders of magnitude. (Just try to
  generate them, it will be hard to visualize them properly or test if
  they are correct.)
  * Before you start: Which difficulties do you expect?
  * Which problems do you see when you generate a tree with a height
    of `100`, `1000` or `10000`?
  * How can you address those problems?
  * How does your existing design cope with the new requirements?
