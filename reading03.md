# File Manipulation / System.IO

## [File and Stream I/O](https://docs.microsoft.com/en-us/dotnet/standard/io/)

* What is File and Stream I/O (input/output)?

> File and stream I/O (input/output) refers to the transfer of data either to or from a storage medium. In .NET, the System.IO namespaces contain types that enable reading and writing, both synchronously and asynchronously, on data streams and files.

> A file is an ordered and named collection of bytes that has persistent storage. When you work with files, you work with directory paths, disk storage, and file and directory names. In contrast, a stream is a sequence of bytes that you can use to read from and write to a backing store, which can be one of several storage mediums (for example, disks or memory).

> Files and Directories

  > File

    * Provides static methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

> FileInfo

  > Provides instance methods for creating, copying, deleting, moving, and opening files, and helps create a FileStream object.

> Directory

  > Provides static methods for creating, moving, and enumerating through directories and subdirectories.

> DirectoryInfo

  > Provides instance methods for creating, moving, and enumerating through directories and subdirectories.

> Path

  > Provides methods and properties for processing directory strings in a cross-platform manner.

* Streams

> The base class of streams supports reading and writing bytes. Streams involve three fundamental operations: reading, writing, and seeking.

* Readers and Writers

> System .IO provides types of reading encoded characters from streams and writing them into streams.

  > Some commonly used reader and writer classes are: binary reader/writer, stream reader/writer, string reader/writer, and text reader/writer

* Asynchronous I/O operations

> Reading or writing a large amount of data can be resource-intensive. You should perform these tasks asynchronously if your application needs to remain responsive to the user. With synchronous I/O operations, the UI thread is blocked until the resource-intensive operation has completed. Use asynchronous I/O operations when developing Windows 8.x Store apps to prevent creating the impression that your app has stopped working.

* Compression

> Compression refers to the process of reducing the size of a file for storage. Decompression is the process of extracting the contents of a compressed file so they are in a usable format. The following classes are used when compressing and decompressing files: ZipArchive, ZipArchiveEntry, ZipFile, ZipFileExtensions, DeflateStream, and GZipStream.

* Isolated Storage

> solated storage is a data storage mechanism that provides isolation and safety by defining standardized ways of associating code with saved data. The storage provides a virtual file system that is isolated by user, assembly, and (optionally) domain. It is particularly useful when your application does not have permission to access user files.

## [Write to a file](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file)

* The following classes and methods are typically used to write text to a file:

  * StreamWriter contains methods to write to a file synchronously (Write and WriteLine) or asynchronously (WriteAsync and WriteLineAsync).

  * File provides static methods to write text to a file, such as WriteAllLines and WriteAllText, or to append text to a file, such as AppendAllLines, AppendAllText, and AppendText.

  * Path is for strings that have file or directory path information. It contains the Combine method and, in .NET Core 2.1 and later, the Join and TryJoin methods, which allow concatenation of strings to build a file or directory path.

## [Read to a file](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)

* The System.IO.BinaryWriter and System.IO.BinaryReader classes are used for writing and reading data other than character strings. The following example shows how to create an empty file stream, write data to it, and read data from it.

### Additional Resources

* Information taken from links provided above
