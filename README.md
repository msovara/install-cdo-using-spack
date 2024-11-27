# install-cdo-using-spack

## Source the spack environment
```
source setup-env.sh
```
1. Search the spack repository for the ```cdo``` application and download the gcc compiler version. 
```
spack list cdo
spack install cdo %gcc@12.2.0
```
2. Change the directory to /scripts/modules/ and then create a symlink to the spack module. 
```
cd /apps/chpc/scripts/modules/earth/CDO
```
3. In another terminal, in the /home/apps/ directory, create a directory where the symbolic link to the spack module file.
```
ln -s /home/msovara/spack/share/spack/modules/linux-centos7-haswell/cdo/2.2.0-gcc-12.2.0-qu2jwp5 2.2.0
```
4. Test for the existence of the module file then load the module.
```
module avail 2>&1 | grep -i cdo
module show
module load
```

