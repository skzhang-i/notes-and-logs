# How to change the language of java outputs in the Command Prompt? 

The language of my Windows OS is Chinese. When I run java in the CMD, the console gives Chinese infomation. To change the language of outputs to English, use this argument: 
`-J-Duser.language=en` 
Just like this, 
```
javac -J-Duser.language=en
javac
```
Now the output is English, **temporarily**. If you close the CMD and reopen it, type in the command then press enter, the output will be Chinese again. 

To set English as the default language of output, you need to set an environment variable. 
1. Press Win+R and type in `sysdm.cpl`.
2. Add an environment variable called `JAVA_TOOL_OPTIONS`. Its value is `-Duser.language=en`. 
