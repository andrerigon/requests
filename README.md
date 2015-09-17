# requests
[![GoDoc](https://godoc.org/github.com/golang/gddo?status.svg)](http://godoc.org/pkg/github.com/leonmaia/requests)

![amazing](https://raw.github.com/leonmaia/requests/master/readme_assets/jake_amazed.gif)


Features
--------

- Retries
- Connection Timeouts

Installation
------------

To install Requests, simply:

    $ go get github.com/leonmaia/requests


Usage
------------
```go
package whatever

import (
	"github.com/leonmaia/requests"
)

func GetExampleWithDefaultTimeoutAndRetries() error {
	r, err := requests.NewRequest("GET", "http://google.com", nil)
	if err != nil {
		return err
	}

	response, err := r.Do()
	if err != nil {
		return err
	}
	// Do whatever you want with the response
	return nil
}
```
How to Contribute
------

I strongly encourage everyone whom creates a usefull custom assertion function
to contribute them and help make this package even better.

Make sure all the tests are passing, and that you have covered all the changes
you made.

