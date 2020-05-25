# CoppeliaSim Lunar Terrain

A simple lunar-like virtual scene to be used with robotics simulator [CoppeliaSim](https://www.coppeliarobotics.com/). 

*Note: The terrain does not correspond to a real region of the Moon, but has, instead, been modeled using the **Terrain.ttm** tool available by default. Digital elevation models can be imported as heightfield shapes in CoppeliaSim as per the information provided [here](https://www.coppeliarobotics.com/helpFiles/en/importExport.htm).*  

## Getting Started

This repository contains the scene file of a lunar terrain along with some 3D files required to customize and add complexity to the scene. These include: a collection of [rocks](https://www.thingiverse.com/thing:3013912) and a 3D model of SpaceIL and Israel Aerospace Industries [Beresheet Lunar Lander](https://www.thingiverse.com/thing:3558422). 

### Prerequisites

To get your simulations up and running on the lunar terrain scene all you need is the latest version of [CoppeliaSim](https://www.coppeliarobotics.com/downloads) simulator. 

Latest version the scene was used with: *V4.0.0 rev4*

## Visuals

This is an example of the look and use of the terrain for a 18-m virtual lunar traverse.
![Image of terrain](/img/map.png)

## Terrain characteristics 

The terrain contains multiple elevation changes with a maximum slope angle of 22 degrees. The interaction with the ground is computed using the Scaled Box Fast model and, to simulate the frictionless character of lunar regolith, the dynamic object representative of the terrain is characterized by an isotropic friction coefficient of 0.4. This can be changed in the *Dynamic Properties > Material Properties* menu under *Linear Primary and Secondary Axis*, see [here](https://www.coppeliarobotics.com/helpFiles/en/shapeDynamicEngineProperties.htm) for reference. 

The terrain was initially meant to be simulated using the high-fidelity physics engine, [Vortex](https://www.cm-labs.com/vortex-studio/), but it can work with any of the other engines available in CoppeliaSim. 
*Note: Make sure to change material properites and simulation/dynamic step times accordingly.*

In its default configuration, the terrain does not contain any rocks. These can be easily imported into the scene via *File > Import > Mesh...* and selecting any of the multiple STL files available in the rocks folder.

The terrain includes the lander and a 3-m egress ramp inclined at 15 degrees. 

## Authors

* **David Rodriguez** - *Initial scene definition* - @drodriguezSRL

## Acknowledgments

* Thanks to [BREXIT](https://www.thingiverse.com/BREXIT/about) and [IdoPrints](https://www.thingiverse.com/IdoPrints/about) form [Thingiverse](https://www.thingiverse.com/) for the STL files. 

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to run tests on major updates before merging.

## License

* Rocks by [BREXIT](https://www.thingiverse.com/BREXIT/about) is licensed under the Creative Commons - [Attribution license](https://creativecommons.org/licenses/by/3.0/us/).
* Beresheet Lunar lander by [IdoPrints](https://www.thingiverse.com/IdoPrints/about) is licensed under the Creative Commons - [Attribution license](https://creativecommons.org/licenses/by/3.0/us/).
* Lunar soil texture source image: NASA. 

The rest of this project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/)

