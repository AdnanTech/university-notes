# Data Design

## Logical Side of things

### Entity

**A data entity is anything real or abstract in which data can be stored about.** E_ntity types fall into five classes: roles, events, locations, tangible things or concepts_. E.g. employee, payment, campus, book. Specific examples of an entity are called instances. E.g. the employee John Jones, Mary Smith's payment, etc.

### Relationship

**A data relationship is a natural association that exists between one or more entities. E.g. Employees process payments**. 

**Cardinality **_defines the number of occurrences of one entity for a single occurrence of the related entity._ E.g. an employee may process many payments but might not process any payments depending on the nature of her job. 

### Attribute

**A data attribute is a characteristic common to all or most instances of a particular entity.** Synonyms include property, data element, field. E.g. Name, address, Employee Number, pay rate are all attributes of the entity employee. An attribute or combination of attributes that uniquely identifies one and only one instance of an entity is called a primary key or identifier. E.g. Employee Number is a primary key for Employee.

## Primary, Foreign and Compsite Keys

Candidate key is the minimal set of attributes that uniquely identify each occurrence of an entity type.

A **primary **key is the candidate key that is selected to uniquely identify a particular occurrence of an entity.

Where there is a one-to-many relationship, the entity on the ‘many’ side must contain the primary key of the entity on the ‘one’ side. This is a **foreign **key.

**Composite **key is where a primary key of an entity type is composed of two or more attributes, whose values together are unique for each entity occurrence, but not separately.

## Data side of things

### Validation

Validationis checking data before processing to see that it is acceptable for the process, it may include:

* Type checks (e.g. numeric or alphanumeric)
* Length checks (right number of characters)
* Range checks (1 to 999)
* Constraints(projectEndDatemust be after projectStartDate) Introduce appropriate validation rules and error messages, in case those rules are broken.

### Redundancy

### Integrity

**Referential Integrity**

Verificationis checking data which has been copied from one place to another to see if that it is still the sam

Use of foreign keys for referencing data in other tables, where a new record cannot be added, without it existing in a linked tables, which contains the primary keyEnsures consistencyReferential integrity controls the links between records

“If a foreign key exists in a relation, either the foreign key value must match a candidate key value of some tuple in its home relation of the foreign key must be wholly null” (Connolly and Begg, 2010)

Entityintegrity◦No attribute of a primary key can be null◦This is where a Primary key is used to make this possible, i.e. ‘studentNumber’ is used to uniquely identify each student whose details are stored in the ‘Student’ relation◦No tuples should be inserted into a relation without a primary key or a composite primary keyDomainintegrity◦Values must conform to the rules that have been defined, i.eformat, range, etc...Referentialintegrity◦Use of a ‘Foreign’ key for referencing with their counterpart the ‘Primary’ key, where a matching value must exist.

## **Check Sums**

A check digit is an extra digit added to a number so that, if a number is changed, the error will be detected

Example: 978023057305** **becomes 978023057305 -5

![](<../../../../../.gitbook/assets/image (131).png>)

Therefore 5 is the check digit that has to check out for a valid number. This is an example of the ISBN-13 checksum (formerly 10)
