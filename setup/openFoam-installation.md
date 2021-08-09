There are two branches of openFoam: ESI-OpenCFD [openfoam.com](https://www.openfoam.com/) and OpenFOAM-9 [openfoam.org](https://openfoam.org/).
Please follow the instructions for the branch you choose. I recommend you install both branches.

There are several ways to install openFoam (use instructions from openfoam.* pages to decide which is best for you):
* natively (pre-compiled or not)
* through Docker (by making a container)
* by Windows Subsystem Ubuntu

From my personal experience, 
* if using Mac OS X, use openFoam on Docker Desktop
* if using Windows, follow [this](http://www.cfdyna.com/Home/openFOAM_Win.html)
* if using Ubuntu, Linux, you have it easy
	
For post-processing, it is best to install native [paraview](https://www.paraview.org/)


OpenFoam Installation Tips & Notes & Troubleshooting for Systems
	
Mac
* openFoam container in docker does not come with text editor or paraview 
* so, use two terminal windows--one to use nano or vim (text editor) and the other to run openFoam
* you will have to run a .sh script to set up docker, find explicit instructions [here](https://www.addictivetips.com/mac-os/run-shell-sh-script-on-macos/)
	  
Windows 10
1. https://www.youtube.com/watch?v=cUbC0MrkiOA
2. I still haven't figured out a streamlined approach to setting openFoam up on Windows 10. Here are misc. that could help:
3. If compiling on Docker Desktop, install WSL. Check version <wsl.exe -l -v>. If Ubuntu (20.04) is 1, run <wsl.exe --set-default-version Ubuntu (*) 2> to set it to 2.
4. open Docker Desktop app
5. go to 'settings' (cog)
6. click 'Resources' and select 'WSL INTEGRATION' 
7. allow both 'Enable integration with my default WSL distro' and 'Ubuntu'
8. in Ubuntu, <docker search openfoam> //displays list of available containers
9. <docker container run -ti cfdengine/openfoam> //choose existing container and run
10. check installation by opening Docker under Images--it should display
11. in Ubuntu, make shell script [here](https://develop.openfoam.com/Development/openfoam/-/wikis/packaging/docker/openfoam-docker) executable, run <chmod +x openfoam-docker.sh>.
12. in Ubuntu, run shell <sh openfoam-docker.sh>.
13. to make life easier, compile tutorial folders on Desktop or an easy access location.
