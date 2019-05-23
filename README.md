# nix-nwb

Experiments in converting data between the [NIX][nix] data format and
the [NWB][nwb] format.

## nwb → nix

The "easier" path, because NIX is a more generic data format than
NWB. The script was build using a [data set][allan] from the Allan
institute: [H19.28.012.11.05-2.nwb][allan-data]

## nix -> nwb

Since NIX is very the more abstract data format, a generic conversion
from NIX o NWB is not feasible. But for specific data that are stored
in a stereotypical way a it will be possible. `nix2nwb.py` was build
around a data set recorded with [relacs][relacs]. Since for the recording
at hand there was no corresponding high level type in NWB, for now the
generic `TimeSeries` data container was used.

[allan]: http://download.alleninstitute.org/informatics-archive/prerelease/H19.28.012.11.05-2.nwb
[allan-data]: http://download.alleninstitute.org/informatics-archive/prerelease/
[relacs]: https://github.com/relacs/relacs
[nix]: www.g-node.org/nix
[nwb]: https://neurodatawithoutborders.github.io/
