# Hacking

## Requirements
- kind 0.9 or above
- Go 1.15+

## Project Structure

```
└── plugin
    ├── actions
    │   └── cluster.go - Creating/deleting clusters
    ├── router
    │   └── handlers.go - URL routing
    ├── settings
    │   ├── capabilities.go - List of actions this plugin does
    │   ├── meta.go - Plugin name, description, icon
    │   └── options.go - Boilerplate to load routes for main.go
    └── views
        ├── ~
        ├── cluster_view.go - UI logic
        ├── feature_gates.go - Autogenerated list of feature gates
        └── node_images.go - Default kind node versions
```

## Build From Source
Run `make build` from the root directory then move the compiled binary from `/bin/octant-plugin-for-kind` to `$/HOME/.config/octant/plugins`.
