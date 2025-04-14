## Please follow the below steps

• dotnet new webapi -n UserProfile  
• dotnet add package Microsoft.Data.Sqlite  
• dotnet add package Microsoft.EntityFrameworkCore.Sqlite  
• dotnet add package Microsoft.EntityFrameworkCore.Tools  
• dotnet ef migrations add InitialCreate  
• dotnet ef database update  
• dotnet add package Swashbuckle.AspNetCore  
• http://localhost:5037/swagger/index.html  

## Unit Tests
• dotnet add package Moq  
• dotnet add package Microsoft.AspNetCore.Mvc  
