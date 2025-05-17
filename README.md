# SKY130 PDK for Analog Design
 
A subset of SKY130 for analog design.

- https://www.github.com/google/skywater-pdk
- https://skywater-pdk.readthedocs.io/

## Download

- `cd` to your home directory/
- `git clone https://github.com/silicon-vlsi-org/pdk-sky130-ana.git share`
  - **NOTE** Make sure the pdk is in `$HOME/share/pdk` for _xschem_ schematic editor to work properly.

## Installation

- Followed the [xschem SKY130 Integration](https://xschem.sourceforge.io/stefan/xschem_man/tutorial_xschem_sky130.html) instructions to install the PDK.
- **Note**: latest version of Magic is required for compiling the PDK. You can find the latest Magic and instructions [here](https://github.com/silicon-vlsi-org/eda-magic)
- Basic steps:
  - `git clone git://opencircuitdesign.com/open_pdks`
  - `cd open_pdks`
  - `./configure --enable-sky130-pdk --prefix=/home/ubuntu/pdk`
    - This will install in the local directory instead in root.
  - `make`
  - `make install`
  - If everything goes fine, you will have almost 8GB of PDK files and most of the space is occupied by the digital libraries. 
  - For the analog simulation, trimmed it down to the following directories:

```bash

pdk
├── scripts  (probably not necessary)
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

- See the [xschem github page](https://github.com/silicon-vlsi-org/eda-xschem) on how to setup environment variables for _xschem_ schematic editor.
