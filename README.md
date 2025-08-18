# Lux Mock Library

Centralized mock utilities and helpers for the Lux ecosystem.

## Features

- **GoMock utilities**: Simplified gomock controller and matcher utilities
- **Mock generators**: Tools for generating mocks
- **Test helpers**: Common testing utilities

## Installation

```bash
go get github.com/luxfi/mock
```

## Usage

```go
import (
    "github.com/luxfi/mock/gomock"
)

func TestExample(t *testing.T) {
    ctrl := gomock.NewController(t)
    defer ctrl.Finish()
    
    // Use your mocks here
}
```

## Generating Mocks

Use the standard mockgen tool:

```bash
mockgen -source=interface.go -destination=mocks/mock_interface.go -package=mocks
```

## License

See the LICENSE file for licensing terms.