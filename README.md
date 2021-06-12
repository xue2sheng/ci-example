# ci-example

To statically build on Windows:

.cargo/config

	[target.x86_64-pc-windows-msvc]
	rustflags = ["-C", "target-feature=+crt-static"]

To statically build on Linux, use musl target instead of regular linux:

	cargo build --target x86_64-unknown-linux-musl --verbose --release

More details at [release.yml](.github\workflows\release.yml)
