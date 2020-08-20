```go
package main

import (
	"fmt"
)

type aboutMe struct {}

func(a *aboutMe) Job (year int) {
    switch {
        case year >= 2020:
            fmt.Println("Software Engineer II @ Eagleview")
        case year == 2019:
            fmt.Println("GIS Engineer @ Cropin Technologies")
        case year < 2019 && year >= 2016:
            fmt.Println("Engineer - Search @ Mapbox Technologies")
    }
}

func main() {
    aboutGokul := aboutMe{}
    aboutGokul.Job(2020)
}
```
