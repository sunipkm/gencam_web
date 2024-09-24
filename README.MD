# GenCam Web
Add dependencies to the workspace `Cargo.toml` under `[workspace.dependencies]` without default features.
Refer to the dependency in a member `Cargo.toml` like:
```toml
crate_name = { workspace = true, default-features = false, features = [
  "cool_feature",
] }
```