# GenCam Web
Add dependencies to the workspace `Cargo.toml` under `[workspace.dependencies]` without default features.
Refer to the dependency in a member `Cargo.toml` like:
```toml
crate_name = { workspace = true, default-features = false, features = [
  "cool_feature",
] }
```
### Build GUI
```sh
$ scripts/build_web_server.sh
```

### Run GUI
```sh
$ scripts/start_web_server.sh
```

### Run websocket backend
```sh
$ cd gencam_wsock_server && cargo run --release
```