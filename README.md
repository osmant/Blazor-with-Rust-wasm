# Blazor with Rust Wasm

This app is created to experiment how Blazor WebAssembly app can use `wasm` module generated by Rust library using `wasm32-unknown-unknown` target.

To be able to run the app follow the steps below.

1. Clone the repo
2. Open BlazorAppExternalWasm project or folder
   - If you are using Visual Studio or Rider or other IDE, simply run the project using the IDE.
   - If you are using CLI, run `dotnet run` command.

Note: you don't need to build hello-wasm Rust project separately. `dotnet run` or `dotnet build` or `dotnet clean` commands are also taking care of rust target folder's maintenance.

`dotnet run` or `dotnet build` commands are compiling the Rust library by targeting the `wasm32-unknown-unknown` before building the BlazorWebAssembly project.

`dotnet clean` command is cleaning up the Rust project's target folder, which is where the last compilation artifacts are stored, after finishing the cleanup of BlazorWebAssembly project bin directory.


