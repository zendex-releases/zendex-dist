# Zendex

Steam depot and bundle tooling. Windows x64, per-user install.

## Download

Latest release: see the Releases tab on this repository.

| File | Purpose |
| --- | --- |
| `Zendex-6.10.1-Setup.exe` | Windows installer, per-user, no admin rights |
| `Zendex_Client_Hardened.zip` | Portable build, extract the whole folder |

## Verify

```powershell
Get-FileHash .\Zendex-6.10.1-Setup.exe -Algorithm SHA256
```

Compare against `SHA256SUMS.txt` in the same release.

Unsigned build: Windows SmartScreen may show a warning on first run. Choose
**More info** then **Run anyway**, or unblock the file first:

```powershell
Unblock-File .\Zendex-6.10.1-Setup.exe
```

## Requirements

- Windows 10/11, 64-bit
- .NET 9 Runtime for depot downloads (the installer offers it)
- Steam installed

## License

GPL-3.0-or-later. See `LICENSE`.
