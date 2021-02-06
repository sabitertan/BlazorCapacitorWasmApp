# BlazorCapacitorWasmApp
Exploring Blazor Web Assembly on capacitor

# Tested (TODO: Add this steps to a custom build script)
1. build project "dotnet build"
2. create "platforms\capacitor" folder
3. cd "platforms\capacitor"
4. copy wwwroot files to "platforms\capacitor\www"
5. npx cap init
6. npx cap add android
7. copy "bin\Debug\5.0\_framework" to "platforms\capacitor\www\framework"
8. replace "_framework" with "framework" in platforms\capacitor\www\framework\blazor.webassembly.js
9. delete "*.gz" files under "platforms\capacitor\www\framework"
10. npx cap open android
11. Build with Android Studio
12. Run in Android Emulator (Pixel C API 30 )

