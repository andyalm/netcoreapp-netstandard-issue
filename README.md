# netcoreapp1.0 referencing netstandard1.5 issue
Sample dotnet core project that demonstrates an issue with a netcoreapp1.0 referencing a local netstandard1.5 library in the same source tree.
When I run `dotnet restore`, I get a huge number of errors that all look something like this:
```
Unable to satisfy conflicting requests for 'System.Runtime.Extensions': System.Runtime.Extensions (>= 4.1.0-rc2-24027) (via package/Microsoft.CSharp 4.0.1-rc2-24027), System.Runtime.Extensions (>= 4.1.0-rc2-24027) (via package/Microsoft.VisualBasic
```

What am I doing wrong?
