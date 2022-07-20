# Format

The format of a `knifer.toml` looks like:

```toml
[knifer]
desc = "A compose file for developing quantii"

[system]
cpu = {"count" = 4}
ram = "8G"
disk = {reserve = "4G"}

[services.quantii]

```
