# Running C Sharp

## MacOS

1. Install .NET SDK & Runtime
```zsh
brew install --cask dotnet
```

    !!! NOTE
        Run `open -a "About This Mac"`.

        If your "Chip" is "Intel", run the "INTEL MAC ONLY" step.

        Otherwise, follow the instructions in the [Dev Setup Guide](./dev_setup_guide.md) before running the "M1 MAC ONLY" step.

1. M1 MAC ONLY - Install Mono
```zsh
brow install mono
```

1. INTEL MAC ONLY - Install Mono
```zsh
brew install mono
```

1. Make the working directory.
```bash
mkdir practice && mkdir practice/c_sharp

cd practice/c_sharp
```

1. Copy C Sharp code into `test.cs`
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

1. Compile & Run `test.cs`
```bash
mcs -out:test.exe test.cs

mono test.exe
```

## WSL - Ubuntu 21.04

1. Add Microsoft Package repo
```bash
wget https://packages.microsoft.com/config/ubuntu/21.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb

sudo dpkg -i packages-microsoft-prod.deb

rm packages-microsoft-prod.deb
```

1. Install .NET SDK & Runtime
```bash
sudo apt-get update

sudo apt-get install -y apt-transport-https

sudo apt-get install -y dotnet-sdk-5.0

sudo apt-get install -y dotnet-runtime-5.0
```

1. Install Mono
```bash
sudo apt install mono-complete
```

1. Make the working directory.
```bash
mkdir practice && mkdir practice/c_sharp

cd practice/c_sharp
```

1. Copy C Sharp code into `test.cs`
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

1. Compile & Run `test.cs`
```bash
mcs -out:test.exe test.cs

mono test.exe
```
