This are the setup and running steps:
#1. blockMesh --> edit constant/polyMesh/boundary --> edit defaultFaces "empty" to "wall" (i have an issue to define the pipe wall boundary, so i need to edit it manualy)
#2. setField
#3. decomposePar --> please edit system/decomposePar with your own hardware preference
#4. mpirun -np x foamRun -parallel --> set the number of x with the number of core within your decomposePar setting
or you can run "foamRun" after "setField" to start running without parallelization

Caesar Wiratama
December 31th, 2023
