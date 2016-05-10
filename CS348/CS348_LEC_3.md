# CS 348 Lecture 3

***The Relational Model***

Schema: Colum name && domain. (sometimes we omitted the attributed domains)

For example: author(aid:int, name:string)

instance (of previous scheme):
author = {(1, John}, (2,Sue)}

***You should never has two rows that are identicals, each relation is defined to be a set of unique tuples or rows***

wrote(author:int, publication:int), we expect that the first attribute's value is in the domain of author.aid.

Look at these two relation schemeas, book(pubid, publisher, year), journal(pubid, volume, no, year). We should expect dom(journal.pubid) is a subset of dom(book.pubid).

If one pubid occurs in the instance of scheme publication(pubid, title), we should expect this id also in some of the instance iof book, journal, proceeding, and articles.

