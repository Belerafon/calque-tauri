# Calque Desktop (Tauri)

A lightweight desktop version of the [calque.io](https://calque.io/) calculator, built with Tauri for Windows.

## Project Structure

- `frontend/` — Frontend sources and build (HTML, JS, CSS)
- `src-tauri/` — Tauri (Rust) sources
- `src-tauri/target/release/Calque.exe` — Final exe application

## How to Build exe

1. **Make sure you have Rust (Cargo) and Node.js installed**
   - Rust: https://rustup.rs/
   - Node.js: https://nodejs.org/

2. **Open cmd (not PowerShell!) in the project folder**

3. **Run the command:**
   ```
   cmd /c "set PATH=%USERPROFILE%\.cargo\bin;%PATH% && npm exec tauri build -- --verbose"
   ```
   This will temporarily add Cargo to PATH and build a fresh exe.

4. **The built exe will appear here:**
   ```
   src-tauri/target/release/Calque.exe
   ```

## Download

You can always download the latest ready-to-use exe from the [Releases page](https://github.com/Belerafon/calque-tauri/releases).

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Notes
- All frontend sources and styles are identical to the original calque.io
- For Tauri/Rust, always use cmd, not PowerShell
- If Rust is not found, restart cmd or add `%USERPROFILE%\.cargo\bin` to PATH
