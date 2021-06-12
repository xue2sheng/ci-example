# ci-example

To statically build on Windows:

.cargo/config
	[target.x86_64-pc-windows-msvc]
	rustflags = ["-C", "target-feature=+crt-static"]
