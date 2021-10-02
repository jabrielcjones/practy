# Running C Sharp

## WSL - 21.04

### Add Microsoft Package repo

```bash
wget https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb

sudo dpkg -i packages-microsoft-prod.deb

rm packages-microsoft-prod.deb
```

### Install .NET SDK & Runtime

```bash
sudo apt-get update

sudo apt-get install -y apt-transport-https

sudo apt-get install -y dotnet-sdk-5.0

sudo apt-get install -y dotnet-runtime-5.0
```

### Install Mono Complete

```bash
sudo apt install mono-complete
```

### Make the working directory.

```bash
mkdir practice && mkdir practice/c_sharp

cd practice/c_sharp
```

### Copy C Sharp code into `test.cs`

```csharp
using System;  
  
namespace Test  
{  
   class TestClass  
   {  
     static void Main(string[] args)  
      {  
          Console.WriteLine("This is a test.");
      }  
   }  
}
```

### Compile & Run `test.cs`

```bash
mcs -out:test.exe test.cs

mono test.exe
```
