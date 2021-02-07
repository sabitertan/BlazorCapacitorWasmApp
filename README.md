# BlazorCapacitorWasmApp
Exploring Blazor Web Assembly on capacitor

# Tested (TODO: Add this steps to a custom build script)
1. build project "dotnet build"
2. create "platforms\capacitor" folder
3. cd "platforms\capacitor"
4. copy wwwroot files to "platforms\capacitor\www"
5. copy "obj\Debug\net5.0\scopedcss\bundle\BlazorCapacitorWasmApp.styles.css" to "platforms\capacitor\www"
6. npx cap init
7. npx cap add android
8. copy "bin\Debug\net5.0\\_framework" to "platforms\capacitor\www\framework"
9. replace "_framework" with "framework" in platforms\capacitor\www\framework\blazor.webassembly.js
10. delete "*.gz" files under "platforms\capacitor\www\framework"
11. npx cap open android
12. Build with Android Studio
13. Run in Android Emulator (Pixel C API 30 , Pixel XL API 29)
14. API 28 emulators did not work

