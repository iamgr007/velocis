# Efficient Rust HTTP Web Server

This repository demonstrates an efficient implementation of a lightweight HTTP web server in Rust. Built with performance and simplicity in mind, this project serves as a foundational base for developers looking to create fast, scalable, and reliable web services in Rust.

## Features

- **Asynchronous I/O**: Powered by [Tokio](https://tokio.rs) for non-blocking, high-performance networking.
- **Minimal Dependencies**: Focuses on a clean and minimalistic implementation.
- **Custom Routing**: Define routes easily for different endpoints.
- **Static File Serving**: Serve static files from a specified directory.
- **Extensible**: Easily add middleware or extend functionality.

## Requirements

To build and run this project, you need:

- [Rust](https://www.rust-lang.org) (1.65 or later)
- Cargo (comes with Rust)

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yourusername/efficient-rust-http-server.git
cd efficient-rust-http-server
```

### Build the Project

Run the following command to build the project:

```bash
cargo build --release
```

### Run the Server

Start the server with:

```bash
cargo run
```

By default, the server listens on `http://127.0.0.1:8080`. You can modify the port and address in the `main.rs` file.

### Example Usage

- Visit `http://127.0.0.1:8080/` to see a welcome message.
- Visit `http://127.0.0.1:8080/static/<filename>` to serve static files.

## Code Structure

```
.
├── src
│   ├── main.rs         # Entry point for the application
│   ├── router.rs       # Custom routing logic
│   └── static_files.rs # Static file handling module
├── Cargo.toml          # Project dependencies and metadata
└── README.md           # Project documentation
```

## Configuration

You can customize the server settings (e.g., port, host, routes) in the `main.rs` file. For more complex configurations, consider using environment variables or a configuration library like [config](https://docs.rs/config).

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this implementation.

### Steps to Contribute

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature-branch`.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Tokio](https://tokio.rs): For powering asynchronous I/O.
- [Rust Language](https://www.rust-lang.org): For providing an amazing platform to build robust and performant systems.
