#SQL day 2 (aka sqewl, aka skl, .)

- Student can add foreign key to new table
- Student can add foreign key to existing table
- Student can use join
- Student can use sub-selects/nested queries
- Student can set null values
- Student can Group by
- Student can update rows
- Student can delete rows
- Student can use distinct
- Student can describe one-to-one relationships
- Student can describe one-to-many relationships
- Student can describe many-to-many relationships

* 1st normal form:

- data in each column is indivisable

- recommended

  - string
  - number
  - boolean
  - null
  - float

- not recommended

  - objects
  - arrays

* 2nd normal form:

- first normal form
- all non key columns are dependant on the tables primary key

* 3rd normal form:

- second normal form
- contains only columns that are non transitively-dependant on a primary key

transitive: A is greater than B, and B is greater than C this it would make sense that A if greater than C

A, B, PK, if the value of A relies on the PK, and B relies on the PK and A also relies on B then you can say A relies on PK through B

```sql
personId, firstName, lastName => non transitively dependant

personId, bodyMassIndex, isObese => transitvely dependant
```

**one to one relationship**

- one column in a table is associated with one and only one column from another a table

<img width='500px' src='https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/CPT-Databases-OnetoOne.svg/500px-CPT-Databases-OnetoOne.svg.png'>

**one to many relationships**

- one column in a table can be associated with on or more columns in another table

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d7/CPT-Databases-OnetoMany2.svg/500px-CPT-Databases-OnetoMany2.svg.png">

**many to many relationships**

- multiple columns in a table can be associated with multiple columns from another table

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c4/CPT-Databases-ManytoMany.svg/500px-CPT-Databases-ManytoMany.svg.png">

<img width='500px' src="https://upload.wikimedia.org/wikipedia/commons/0/02/Databases-ManyToManyWJunction.jpg">
