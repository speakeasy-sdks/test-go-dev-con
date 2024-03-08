<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	testgodevcon "github.com/speakeasy-sdks/test-go-dev-con"
	"github.com/speakeasy-sdks/test-go-dev-con/pkg/models/shared"
	"log"
)

func main() {
	s := testgodevcon.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->