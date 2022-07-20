# Format

The format of a `knifer.toml` looks like:

```toml
[knifer]
desc = "A composer for developing quantii"

[system]
cpu = {"count" = 4}
ram = "8G"
disk = {reserve = "4G"}

[services.quantii]
build = {"commands": ["cargo build"]}
expose = [3000]

```

A compose file can call a smaller, individual setup file.
