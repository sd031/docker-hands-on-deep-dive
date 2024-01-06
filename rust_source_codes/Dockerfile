# Use an official Rust image as the base
FROM rust:latest

# Create a new directory for your application
WORKDIR /usr/src/myapp

# Copy the Cargo.toml and source code
COPY ./Cargo.toml ./Cargo.lock ./
COPY ./src ./src

# Build your application
RUN cargo build --release

# The command to run when the container starts
CMD ["./target/release/myapp"]
