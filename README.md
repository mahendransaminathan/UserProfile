1. Download Visual Studio Code
For Windows:
    1. Visit the Visual Studio Code website.
    2. Click on the Download for Windows button. The installer will automatically download for your system.

2. Install Visual Studio Code
For Windows:
    1. Once the installer is downloaded, run it.

    2. Follow the installation prompts:

       • Accept the license agreement.
       • Choose the installation folder.
       • Select additional tasks like creating a desktop icon or adding VS Code to the PATH for easier command line access.

    3. Click Install to complete the installation.

3. Launch Visual Studio Code
   After installation is complete, launch Visual Studio Code:

   Windows: You can find it in the start menu (Windows)

4. Install Extensions (Optional)
   VS Code has a rich set of extensions that enhance your development experience. To install extensions:
   Open VS Code.

   Click on the Extensions icon on the left sidebar (or press Ctrl+Shift+X).
   Search for your desired extensions, such as:
   C# for .NET development.

5. Install SQLite Extension for VS Code
   Open Visual Studio Code.
   Go to the Extensions view by clicking the Extensions icon on the left sidebar (or press Ctrl+Shift+X).
   Search for SQLite.
   Look for the SQLite extension by alexcvzz (or any other SQLite extension you prefer).
   Click Install.

Steps to Create a Solution and Add Projects
1. Open VS Code and Open a New Folder
Open a new folder in VS Code (e.g., UserProfileManager).

2. Create a Solution File
Open the terminal in VS Code.

Run the following command
dotnet new sln -n UserProfileManager

This creates a UserProfileManager.sln solution file.


3. Create Your Projects
Let’s say you want:

An API project called UserProfile

A test project called UserProfile.NUnitTests

Run:
dotnet new webapi -n UserProfile
dotnet new nunit -n UserProfile.NUnitTests

You will now have two folders: UserProfile/ and UserProfile.NUnitTests/, each with its own project file (.csproj).

4. Add Projects to the Solution

dotnet sln add UserProfile/UserProfile.csproj
dotnet sln add UserProfile.NUnitTests/UserProfile.NUnitTests.csproj


5. Add Project References
Your test project should reference the main project so it can access its classes:
Run:
dotnet add UserProfile.NUnitTests/UserProfile.NUnitTests.csproj reference UserProfile/UserProfile.csproj



Run the following command to add the packages into the project 
• dotnet add package Microsoft.Data.Sqlite
• dotnet add package Microsoft.EntityFrameworkCore.Sqlite
• dotnet add package Microsoft.EntityFrameworkCore.Tools

Run the following commands to create a Database
• dotnet ef migrations add InitialCreate
• dotnet ef database update

• dotnet add package Swashbuckle.AspNetCore

Open the application in Swagger with the following URL
• http://localhost:5037/swagger/index.html

Unit Tests

• dotnet add package Moq
• dotnet add package Microsoft.AspNetCore.Mvc
• dotnet add package NUnit
• dotnet add package NUnit3TestAdapter
• dotnet add package Microsoft.NET.Test.Sdk
