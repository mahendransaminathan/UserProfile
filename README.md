## Please follow the below steps

• dotnet new webapi -n UserProfile  
• dotnet add package Microsoft.Data.Sqlite  
• dotnet add package Microsoft.EntityFrameworkCore.Sqlite  
• dotnet add package Microsoft.EntityFrameworkCore.Tools  
• dotnet ef migrations add InitialCreate  
• dotnet ef database update  
• dotnet add package Swashbuckle.AspNetCore  

