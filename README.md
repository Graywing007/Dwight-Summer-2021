# Dwight-Summer-2021

SEE SETUP for installation, Guide, Manual, instructions, etc.

Basement's computer OpenFOAM is compiled using Docker Desktop.
0. Open Docker Desktop
1. Open Ubuntu
2. < cd ../.. >
3. < cd /mnt/c/Users/Fluent/Desktop/ >
4. < sh openfoam-docker.sh >

decomposeParDict in basement's computer should be distributed to 8 CPU cores (2 2 2) instead of 10.

Things to work on
* dynamic meshing //Zoe (sixDofRigidBodyMotion -- use either dynamicOversetFvMesh or dynamicMotionSolverFvMesh)
* running blood-* on different solvers
* LES model simulations
* write up instructions for future research students //Zoe
* make presentation

Checklist of things done
* make animations of blood-LES //Zoe
* [vorticity](https://www.youtube.com/watch?v=4wGO__XLsmg) and circulation //Zoe

Misc.
* [Develop Openfoam](https://develop.openfoam.com/Development/openfoam)
* [Over Set Meshes](https://www.youtube.com/watch?v=QEGnNLvQVfA)
* [Smagorinsky Turbulence](https://www.youtube.com/watch?v=V8ydRrdCzl0)
* [axisymmetric wedges 1](https://www.cfd-online.com/Forums/openfoam-solving/186540-wedge-boundary-condition-math-behind.html)
* [axisymmetric wedges 2](https://www.cfd-online.com/Forums/openfoam-meshing/186049-2d-axisymmetric-model-openfoam-4-0-a.html#post645900)
