# Zig Nix + macOS Framework Bug

`0.12.0-dev.694+937e8cb70`

If you load the Nix environment (nix shell or nix develop) and run
`zig build -Denable-coretext` then you'll get an error where it looks at
the wrong framework search path.

If you are outside the Nix environment, it works.
