<!-- Start SDK Example Usage -->


```go
package main

import(
	"context"
	"log"
	testgodevcon "github.com/speakeasy-sdks/test-go-dev-con"
)

func main() {
    s := testgodevcon.New()

    ctx := context.Background()
    res, err := s.Pets.CreatePets(ctx)
    if err != nil {
        log.Fatal(err)
    }

    if res.StatusCode == http.StatusOK {
        // handle response
    }
}
```
<!-- End SDK Example Usage -->