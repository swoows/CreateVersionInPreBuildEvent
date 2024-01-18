# CreateVersionInPreBuildEvent
빌드 전 이벤트에 버젼 파일 만들기

@echo off
echo namespace adminTool> $(ProjectDir)Version.cs
echo {>> $(ProjectDir)Version.cs
echo    public class Version>> $(ProjectDir)Version.cs
echo    {>> $(ProjectDir)Version.cs
echo        static readonly public string Ver = "Build Time : %date% %time%";>> $(ProjectDir)Version.cs
echo    }>> $(ProjectDir)Version.cs
echo }>> $(ProjectDir)Version.cs
@echo on
