This repo contains the FuseSoc stlye core files for some HDL experiments.
At the moment, this mostly is being used as a way of playing with the OSVVM
testbench code using a simple avalon_stream_forker core as a test ground.

To experiment yourself you will need to grab fusesoc. If you've got pip
installed, you should be good with

* sudo pip install fusesoc

Once done, clone this repo. If you've got modelsim installed and the correct
MODEL_TECH environment variable set, you should be able to run a simulation
with

fusesoc --cores-root=/path/to/clone sim grayter:utilities:avalon_stream_forker

GHDL support will be coming just as soon as GHDL supports unbounded arrays
of unbounded records.