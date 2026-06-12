# nano-ros

Deterministic ROS 2 for embedded and real-time systems.

nano-ros is a space first ROS 2 client stack built for constrained targets.  
It is designed for predictable execution, static memory usage, and backend-agnostic transport.

**Platform focus:** RTEMS, Zephyr  
**Interface support:** ros2_control, EtherCAT, CAN, GPIO  
**Transport:** SpaceWire / CCSDS, zenoh, MIL-STD-1553B, local shared memory, target-specific backends

## Architecture

| Layer | Role |
|-------|------|
| Application | publishers, subscribers, services, actions, control loops |
| Interface | hardware and protocol adapters, including ros2_control, CAN, EtherCAT, GPIO |
| Runtime | deterministic scheduling, static or bounded memory, no heap in the hot path |
| Transport | backend-agnostic, pluggable per target |
| Platform | RTEMS and Zephyr BSP integration |

## Documentation

Full architecture and platform docs at [nano-ros.github.io](https://nano-ros.github.io)

## ROS 2 compatibility

ROS 2 Rolling
