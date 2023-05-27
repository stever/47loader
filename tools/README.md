# 47loader Mono/.NET Tools

Build and update tool executables with the following:

```bash
msbuild 47loader.sln -t:Rebuild -p:Configuration=Release
cp 47loader-bootstrap/bin/Release/47loader-bootstrap.exe .
cp 47loader-tzx/bin/Release/47loader-tzx.exe .
cp 47loader-util/bin/Release/47loader-util.dll .
```

```bash
mono rle.exe
```