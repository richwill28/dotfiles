# Windows Subsystem for Linux (WSL)

## WSL Installation

1. Install Windows Terminal.
   - Always launch PowerShell via Windows Terminal. For whatever reason, the `wsl` keyword is not recognized in PowerShell.
2. Then, follow [this guide](https://learn.microsoft.com/en-us/windows/wsl/install-manual).
3. That's all.

## Ubuntu Installation

1. Always install with the following command

   ```shell
   wsl --install -d Ubuntu
   ```

2. Then, do a full upgrade of all the packages in Ubuntu.

   ```shell
   sudo apt update
   sudo apt full-upgrade
   sudo apt autoremove
   sudo apt clean
   sudo apt autoclean
   ```

3. Check for a new Ubuntu release.

   ```shell
   sudo do-release-upgrade -c
   ```

4. If a new release is available, do

   ```shell
   sudo do-release-upgrade
   ```

5. Again, do a full upgrade as in Step 2.

6. Add Ubuntu repositories.

   ```shell
   sudo add-apt repository main restricted universe multiverse
   sudo apt update
   sudo apt upgrade
   ```

7. That's all.

## Ubuntu Setup

1. Install `git`.
2. Install `vim`.
3. Install `curl`.
4. Install `wget`.
5. Install `zsh`.
6. Install `oh-my-zsh`.
7. Download the following font files
   - [MesloLGS NF Regular.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
   - [MesloLGS NF Bold.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
   - [MesloLGS NF Italic.ttf](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
   - [MesloLGS NF Bold Italic](https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)
8. Double-click on each file and click Install. This will make `MesloLGS NF` font available to all applications on your system.
9. Configure Windows Terminal to use this font:
   1. Open Settings.
   2. Click either on the selected profile under Profiles or on Defaults.
   3. Click Appearance.
   4. Set Font face to `MesloLGS NF`.
10. Install `powerlevel10k`.
11. Restart `zsh` with `exec zsh`.
12. Type `p10k configure` if the configuration wizard doesn't start automatically.
13. Apply (Dracula theme)[https://draculatheme.com/windows-terminal] to Windows terminal.
14. To set `powerlevel10k` prompt character to `λ`, edit `~/.p10k.zsh`.
15. Install `zsh-autosuggestions`.
16. Install `zsh-syntax-highlighting`.

## Essential Packages

- `build-essential`
- `gdb`
- `llvm`
- `clang`
- `clang-tidy`
- `lldb`
- `cmake`
- `python-is-python3`
- `python3-pip`
- `opam`
- `dune`
- Rust
- Go
