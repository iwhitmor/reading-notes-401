# LINQ & Delegates

## [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/)

* Language-Integrated Query (LINQ) is the name for a set of technologies based on the integration of query capabilities directly into the C# language

* With LINQ, a query is a first-class language construct, just like classes, methods, events. You write queries against strongly typed collections of objects by using language keywords and familiar operators

* The LINQ family of technologies provides a consistent query experience for objects (LINQ to Objects), relational databases (LINQ to SQL), and XML (LINQ to XML)

* Query expressions

  * You use the same basic query expression patterns to query and transform data in SQL databases, ADO.NET Datasets, XML documents and streams, and .NET collection

  * Query expressions can be used to query and to transform data from any LINQ-enabled data source. For example, a single query can retrieve data from a SQL database, and produce an XML stream as output

  * A query is not executed until you iterate over the query variable, for example, in a foreach statement. For more information, see Introduction to LINQ queries

  * Query expressions can be compiled to expression trees or to delegates, depending on the type that the query is applied to. IEnumerable<T> queries are compiled to delegates. IQueryable and IQueryable<T> queries are compiled to expression trees. For more information, see Expression trees

## [Introduction To LINQ Queries](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/introduction-to-linq-queries)

* A query is an expression that retrieves data from a data source

* LINQ simplifies this situation by offering a consistent model for working with data across various kinds of data sources and formats

* Three parts of a query operation

  1. Obtain the data source
  2. Create the query
  3. Execute the query

* Query Execution

  * As stated previously, the query variable itself only stores the query commands. The actual execution of the query is deferred until you iterate over the query variable in a foreach statement. This concept is referred to as deferred execution. The foreach statement is also where the query results are retrieved

  * Queries that perform aggregation functions over a range of source elements must first iterate over those elements

  * You can also force execution by putting the foreach loop immediately after the query expression. However, by    calling ToList or ToArray you also cache all the data in a single collection object

## [Basic LINQ Query Operators](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/basic-linq-query-operations)

* Obtaining a Data Source

  * In a LINQ query, the first step is to specify the data source
  
  * In C# as in most programming languages a variable must be declared before it can be used. In a LINQ query, the from clause comes first in order to introduce the data source and the range variable

  * The range variable is like the iteration variable in a foreach loop except that no actual iteration occurs in a query expression

* Filtering

  * Most common query operation is to apply a filter in the form of a Boolean expression

  * The filter causes the query to return only those elements for which the expression is true. The result is produced by using the where clause

* Ordering

  * Often it is convenient to sort the returned data. The orderby clause will cause the elements in the returned sequence to be sorted according to the default comparer for the type being sorted

  * To order the results in reverse order, from Z to A, use the orderby…descending clause

* Grouping

  * The group clause enables you to group your results based on a key that you specify

* Joining

  * Join operations create associations between sequences that are not explicitly modeled in the data sources

### Additional Resources

* [Walkthrough Writing LINQ Queries in C#](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/walkthrough-writing-queries-linq)

* C# 7.0 In a Nutshell - Chapter 8: LINQ Queries

* Some information taken from the links above
