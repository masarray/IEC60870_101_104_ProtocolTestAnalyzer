# Package Structure

Use this structure for every public binary release zip.

## Recommended Zip Name

`IEC60870-Protocol-Test-Analyzer-vX.Y.Z-win-x64.zip`

## Recommended Folder Layout

```text
IEC60870-Protocol-Test-Analyzer-vX.Y.Z-win-x64/
  IEC-60870-Protocol-Analyzer.exe
  lib60870.dll
  System.IO.Ports.dll
  README-RUN.txt
  profiles/
    default-iec104.json
  docs/
    Quick-Start.pdf
```

## Packaging Rules

- Keep the executable and required DLLs in the package root.
- Keep profile files under `profiles/`.
- Keep user-facing quick docs under `docs/` if included.
- Do not include private source files.
- Do not include debug-only artifacts unless intentionally needed.

## README-RUN.txt Suggested Content

Include a very short text file with:

- supported protocols
- how to launch the analyzer
- where to find release notes
- basic support or feedback location

## What To Upload To GitHub Releases

Upload the zip package as the main release asset.

Optional:

- checksum file
- PDF quick-start guide
- sample profile pack
