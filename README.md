# goxcrypto
Cryptebyte Package of Golang Crypto Module

https://stackoverflow.com/questions/25741841/how-can-i-check-if-my-program-is-compiled-for-32-or-64-bit-processor
    package main
    
    import (
    "fmt"
    "runtime"
    "strconv"
    )
    
    func main() {
    const PtrSize = 32 << uintptr(^uintptr(0)>>63)
    fmt.Println(runtime.GOOS, runtime.GOARCH)
    fmt.Println(strconv.IntSize, PtrSize)
    }
