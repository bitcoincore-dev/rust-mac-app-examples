all: build## 	all

.PHONY: app build clean release

build:## 	cargo build
	@cargo build

clean:## 	cargo clean
	@cargo clean

release:## 	cargo build --release
	@cargo build --target=aarch64-apple-darwin --target=x86_64-apple-darwin --release || cargo build --release

app:## 	cd app && xcodebuild
	@cd app && xcodebuild -arch x86_64 -arch Arm64
