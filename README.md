Visual Studio 빌드 전 이벤트에 추가하기 
(C#)
```
@echo off
echo namespace $(ProjectName)> $(ProjectDir)Version.cs
echo {>> $(ProjectDir)Version.cs
echo    public class Version>> $(ProjectDir)Version.cs
echo    {>> $(ProjectDir)Version.cs
echo        static readonly public string Ver = "Build Time : %date% %time%";>> $(ProjectDir)Version.cs
echo    }>> $(ProjectDir)Version.cs
echo }>> $(ProjectDir)Version.cs
@echo on
```
