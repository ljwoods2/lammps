Download H5MD
```
sudo apt-get install libhdf5-dev
```

Configure build
```
cd build
cmake ../cmake/ -D PKG_MISC=yes -D PKG_H5MD=yes
```


Compile
```
cmake --build .
```

Optional, add to path
https://docs.lammps.org/Build_cmake.html
```
make install
```

Run
```
./lmp 
```

Run with example sim
```
cd ../tmp/out
../../build/lmp < ../example.in
```

Run with v3 test
```
lmp < ../example_v3.in
```

Per MPI rank memory allocation (min/avg/max) = 6.915 | 6.915 | 6.915 Mbytes
   Step          Time           Temp          PotEng         KinEng         TotEng         Press          Volume        v_poten    
         2   0.002          300            197.81322      155.0734       352.88661      65748.927      96071.912     -2.5579538e-13