# BlazorCapacitorWasmApp
Exploring Blazor Web Assembly on capacitor

# Tested (TODO: Add this steps to a custom build script)
1. build project "dotnet build"
2. create "platforms\capacitor" folder
3. copy wwwroot files to "platforms\capacitor\www"
4. copy "obj\Debug\net5.0\scopedcss\bundle\BlazorCapacitorWasmApp.styles.css" to "platforms\capacitor\www"
5.  copy "bin\Debug\net5.0\wwwroot\\_framework" to "platforms\capacitor\www\framework"
6.  replace "_framework" with "framework" in platforms\capacitor\www\framework\blazor.webassembly.js
7.  delete "*.gz" files under "platforms\capacitor\www\framework"
8.  cd "platforms\capacitor"
9.  npx cap init
10. npx cap add android
11. npx cap open android
12. Build with Android Studio
13. Run in Android Emulator (Pixel C API 30 , Pixel XL API 29)
14. API 28 emulators did not work

