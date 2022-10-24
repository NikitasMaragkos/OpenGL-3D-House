# OpenGL-3D-House
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT "MIT License")

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House.PNG?raw=true)

With this code you can create a house and a moving sun that lights the whole area. The house is on top of a layer that represents the grass and on the roof of the house we have a spotlight pointing to the front of it.

#### Sun

It has been constructed with the help of a tetrahedron that with recursive subdivision it transformed into a sphere.The sun starts at (-50,0,0) and travels to (50,0,0) through a cyclic movement. It is a point light with specular and diffuse characteristics. As it travels it has a steady increasement to its power and then a steady decreasement. Double buffering has been used as well.

#### House

It has been constructed with a combination of some basic vertices that have been transformed through some rotations and translations. It is necessary to compute the normal vectors of each face correctly so as to have the correct lighting effects.

#### Grass

For the grass we have 2 options:
* Single polygon : In this case the lighting effects are not so good. This can be observed with the effect of the spotlight that points to the grass.
* Multiple small polygons : In this case since we have more vertices with their normals pointing up, the effects of lighting are extremely more obvious and smooth.

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House3.PNG?raw=true)

#### Spotlight

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House4.PNG?raw=true)

A simple spotlight that helps us understand more efficiently the effects of light and shadow.

#### Shadows

For the shadow effects we have 2 options:
* Flat: With the help of the spotlight on and by having multiple polygons as grass we can see that we can observe the squares on the floor.

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House7.PNG?raw=true)

* Smooth : With the help of the spotlight on and by having multiple polygons as grass we can see that we have a realistic shadow effect without squares.

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House7smooth.PNG?raw=true)

#### Scene movement

With left-right arrow someone can move the camera position to an angle that will provide them with a better view.

![House cover image](https://github.com/NikitasMaragkos/OpenGL-3D-House/blob/main/Images/House6.PNG?raw=true)
