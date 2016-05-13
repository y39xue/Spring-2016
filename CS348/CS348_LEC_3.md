# CS 348 Lecture 3

***The Relational Model***

Schema: Colum name && domain. (sometimes we omitted the attributed domains)

For example: author(aid:int, name:string)

instance (of previous scheme):
author = {(1, John}, (2,Sue)}

Note that the instance must be *finite* relations.

***You should never has two rows that are identicals, each relation is defined to be a set of unique tuples or rows***

wrote(author:int, publication:int), we expect that the first attribute's value is in the domain of author.aid.

Look at these two relation schemeas, book(pubid, publisher, year), journal(pubid, volume, no, year). We should expect dom(journal.pubid) is a subset of dom(book.pubid).

If one pubid occurs in the instance of scheme publication(pubid, title), we should expect this id also in some of the instance iof book, journal, proceeding, and articles.

***Relations Models vs SQL Tables***

- Relations are sets of tuples, but tables are multisets (bags) of tuples.
- SQL Tables sometimes has *null* value.

***Integrity constraints***

An instance is only valid when it satisifies all schema constraints.
- tuples level: Domain restrictions, attributes comparisons
- relations level: key contraints(superkey, candidate key, and primary key), functional dependencies(for example, in the university employee databases, the attribute salary is *depends* on the years of serices attribute) 
- database level: Referential integrity and inclusion dependencies(see books)


> By the properties of relational models, superkeys will be theo set of whole attributes. The minimal superkeys is called a *candidate keys*, which is the minimal set that can identifies any two distinct  tuples. We can select (an appropriate) candidate keys to be *primary keys*.

***Relational Operators***










