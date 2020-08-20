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

func(a *aboutMe) Pronoun () {
    fmt.Println("He|Him")
}

func(a *aboutMe) Code () {
    fmt.Println("Go, NodeJS, Python")
}

func(a *aboutMe) ArchTech() {
    fmt.Println("AWS, microservices, K8s, Jenkins, gitops, Express.js, GRPC,
    REST")
}

func main() {
    aboutGokul := aboutMe{}
    aboutGokul.Job(2020)
    aboutGokul.Pronoun()
    aboutGokul.Code()
    aboutGokul.ArchTech()
}
```
