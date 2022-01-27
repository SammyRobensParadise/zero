# makefile

.PHONY: help

help:
	@echo "Makefile commands:"
	@echo "compile      - compiles c++ to web assembly"

compile:
	@echo "Building C++ functions from /functions to web assembly"
	cd src/core && clang++ --target=wasm32 --no-standard-libraries -Wl,--export-all -Wl,--no-entry -o entry.wasm main.cpp
	@echo "Success 🎉"
