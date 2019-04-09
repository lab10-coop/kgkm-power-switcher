# kgkm-power-switcher

"Ka Göd ka Musi" was die winning project of the 24 Hour Infineon Blockchain Hackaton.
https://www.youtube.com/watch?v=TqVXTohUEpI
https://www.youtube.com/watch?v=vT8lANjT620


The project is a node-js server that starts and stops the delievery of power based on the events of a streemable token (see also [streem-poc](https://github.com/lab10-coop/streem-poc)
Power will be delivered if there is at leased one paying for the Power stream.


## Requirements

- Raspberry Pi 3 (other Linux compatible hardware should work as well)
- Raspbian (other Linux should work as well)
- [EG-PMS2](https://energenie.com/item.aspx?id=7415)

## Setup
- Install NPM & Node (tested with v10.15.3)

```
apt-get install libpcsclite1 libpcsclite-dev
git clone https://github.com/lab10-coop/kgkm-power-switcher.git
cd kgkm-power-switcher
npm install
```

## Running
```
npm start
```


for disabling the root requirement for the USB Power:
http://blog.rotten.li/2011/01/05/sispmctl-using-it-as-non-root/


See also: requirements for pcsc. https://github.com/santigimeno/node-pcsclite
