# install-cdo-using-spack

```
source setup-env.sh
spack install cdo %gcc@12.2.0
```
Change dir to /scripts/modules/ and then create a symlink to the spack module 
```
cd /apps/chpc/scripts/modules/earth/CDO
```

In the /home/apps/ directory create an application direcorty that will keep the symlink to the different version module files
```
ln -s /home/msovara/spack/share/spack/modules/linux-centos7-haswell/cdo/2.2.0-gcc-12.2.0-qu2jwp5 2.2.0
```
Test the for the existence of the module file. Load the module file
```
module avail 2>&1 | grep -i cdo
module show
module load
```

