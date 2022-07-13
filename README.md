# ECS 

Entity component system implement in Rust [following](https://ianjk.com/ecs-in-rust/)

## Quick Start
```console
cargo run
```

## Simple Example how it works
```rust
struct Name(&'static str);
struct Health(i32);

let world = World::new();
let entity0 = world.new_entity();
world.add_component_to_entity(entity0, Name("Zeus"));
world.add_component_to_entity(entity0, Health(1000));
```

## License
MIT
