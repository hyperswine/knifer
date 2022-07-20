# Knifer

Wasm container system for quantii and neutron.

How it works:

Build knifer for your platform. The main feature is a userspace container system that can be given access to system resources in a controller fashion, like an app. But with the benefits of sandboxing and a separate rootfs. Depending on the OS, may be structured differently. On Quantii-Neutron, uses default settings.

Knifer is basically a toolchain that allows you to build guest containers from image specs (like docker compose). It also offers a rich UI to compose your container. The native format is TOML.

## Container

A container is an isolated environment in userspace. All apps in the container must be built for wasm-wasi, and run on wasmer. So when you do `./program` on a knifer container, you are actually running `wasmer program`.
