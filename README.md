foamToVTKSwapEndian
===================

Experimental modified foamToVTK from OpenFOAM, for exporting data with the opposite endianess. This was created for this thread at CFD-Online's forums: http://www.cfd-online.com/Forums/openfoam-paraview/147729-big-endian-little-endian-conversion-how-do-openfoam.html


Disclaimer and License
======================

This offering is not approved or endorsed by OpenCFD Limited, the producer of the OpenFOAM software and owner of the OPENFOAM® and OpenCFD® trade marks.

This is bound to the same license as OpenFOAM, namely GNU Public License v3. Quoting from OpenFOAM's license statement:

    OpenFOAM is free software: you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    OpenFOAM is distributed in the hope that it will be useful, but WITHOUT
    ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
    FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License
    for more details.

    You should have received a copy of the GNU General Public License
    along with OpenFOAM. If not, see <http://www.gnu.org/licenses/>.


How to get+build foamToVTKSwapEndian
====================================

Check the list of branches that exist. So far:

  * of21x


For example, these instructions are for OpenFOAM 2.1.x:

For getting and building from git:
```
git clone git://github.com/wyldckat/foamToVTKSwapEndian.git
cd foamToVTKSwapEndian
git checkout of21x
wmake foamToVTKSwapEndian
```

For getting and building from zip:
```
wget "https://github.com/wyldckat/foamToVTKSwapEndian/archive/of21x.zip" -O foamToVTKSwapEndian.zip
cd foamToVTKSwapEndian-of21x
wmake
```


How to use it
=============

A new option exists `-otherEndian`:
```
foamToVTKSwapEndian -otherEndian
```
