# hypfrnt_pyControl_rsync
This code aligns timestamp data of [pyControl system](https://pycontrol.readthedocs.io/en/latest/) to electrophysiology timestamp data at 1 kHz.

## Getting Started

### Prerequisites
- [Python 3](https://www.python.org/)
- [code](https://github.com/yuichi-takeuchi/code)
- [python_utils](https://github.com/yuichi-takeuchi/python_utils)

The codes have been tested with Python 3.7.6.

### Installing
1. Install Python
2. Clone [code](https://github.com/yuichi-takeuchi/code) in the \code\helper directory as a submodule
2. Clone [python_utils](https://github.com/yuichi-takeuchi/python_utils) in the \code\lib directory as a submodule

### How to use
1. Locate pyControl data (blahblah.txt) at the \data directory.
2. Locate ephys 1 kHz timestamp of rsync signal (blablah_rsync_1k_tsp.mat) at the \data directory.
3. Launch \code\align_pyc2amplpx_main.ipynb.
4. Result timestamps will be saved as blahblah.hdf in the \results directory.

## Versioning
We use [SemVer](http://semver.org/) for versioning.

## Authors
- **Yuichi Takeuchi PhD** - *Initial work* - [GitHub](https://github.com/yuichi-takeuchi)
- Affiliation: Department of Physiology, University of Szeged, Hungary
- E-mail: takeuchi.yuichi@med.u-szeged.hu

## License
This project is licensed under the MIT License.

## Acknowledgments
- [Berényi lab](http://www.berenyilab.com/)

## References
- [pyControl](https://pycontrol.readthedocs.io/en/latest/)
