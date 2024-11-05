# install-cdo-using-spack

```
source setup-env.sh
spack install cdo %gcc@12.2.0

cd /apps/chpc/scripts/modules/earth/CDO
ln -s /home/msovara/spack/share/spack/modules/linux-centos7-haswell/cdo/2.2.0-gcc-12.2.0-qu2jwp5 2.2.0

module avail 2>&1 | grep -i cdo
module show
module load

```
