usage:

in `build.gradle.kts`
```
dependencies {
    implementation(files("libs/modified.aar"))
}
```

in `CMakeList.txt`
```
find_package(gmp REQUIRED CONFIG)
target_link_libraries(${CMAKE_PROJECT_NAME} gmp::gmp)
```