# muxter

A simple and elegant multiplexer for Go.

## 🚀 Installation


go get github.com/yourusername/muxter


## 📝 Usage


package main

import (
    "github.com/yourusername/muxter"
)

func main() {
    // Create a new multiplexer
    mux := muxter.New()

    // Add routes
    mux.Handle("/", handler)
    mux.HandleFunc("/hello", func(w http.ResponseWriter, r *http.Request) {
        fmt.Fprintf(w, "Hello, World!")
    })

    // Start server
    http.ListenAndServe(":8080", mux)
}


## ✨ Features

- 🎯 Simple & lightweight
- 🔄 Compatible with standard `http.Handler` interface
- 🛠️ Support for route parameters
- 🔌 Middleware support
- ⚡ Fast & efficient routing
- 📦 Zero external dependencies
- 🛡️ Type-safe handlers

## 📄 License

MIT License - see [LICENSE](LICENSE) file for details