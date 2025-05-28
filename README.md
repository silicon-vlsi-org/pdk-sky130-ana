# SKY130 PDK for Analog Design
 
A subset of SKY130 for analog design.

- https://www.github.com/google/skywater-pdk
- https://skywater-pdk.readthedocs.io/
- See [Installation instructions here](install-pdk.md)

## Download

- `cd` to your home directory/
- `git clone https://github.com/silicon-vlsi-org/pdk-sky130-ana.git share`
  - **NOTE** Make sure the pdk is in `$HOME/share/pdk` for _xschem_ schematic editor to work properly.
- After installation, the directory structure should like this:

```bash

~/share/pdk
├── scripts 
└── sky130A
    ├── libs.ref
    │   └── sky130_fd_pr  (Primitive lib res/mos/cap/etc)
    └── libs.tech
        ├── combined
        ├── irsim
        ├── klayout
        ├── magic
        ├── netgen
        ├── ngspice
        ├── openlane
        ├── qflow
        ├── xcircuit
        └── xschem
```



