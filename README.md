# rubiks-cube-solvers
A collection of solvers for various size rubiks cubes
- 2x2x2 python solver
- 3x3x3 C solver
- 4x4x4 Java solver
- 5x5x5 Java solver

If anyone has a 6x6x6, 7x7x7, or NxNxN solver that they would like to
contribute I would love to find one.

NOTE that I did not write any of these solvers.  This is just a
collection I put together with instructions.


## Install
First git clone this repo
```
$ sudo apt-get install git
$ cd ~/
$ git clone https://github.com/dwalton76/rubiks-cube-solvers.git
```

### Install 2x2x2 solver
```
$ sudo cp ~/rubiks-cube-solvers/2x2x2/rubiks_2x2x2_solver.py /usr/local/bin/
```

### Install 3x3x3 solver
```
$ sudo apt-get install build-essential libffi-dev
$ cd ~/rubiks-cube-solvers/3x3x3/
$ make
$ sudo make install
```

### Install 4x4x4 solver
```
$ cd ~/rubiks-cube-solvers/4x4x4/TPR-4x4x4-Solver/
$ ./make.sh
$ java -cp .:threephase.jar:twophase.jar solver UUURUUUFUUUFUUUFRRRBRRRBRRRBRRRBRRRDFFFDFFFDFFFDDDDBDDDBDDDBDDDLFFFFLLLLLLLLLLLLULLLUBBBUBBBUBBB
```

### Install 5x5x5 solver
5x5x5 solver install...the first time it solves a cube it creates several
prune tables.  Creating these prune tables will take a while (more than
30 minutes) but you only have to do this once.

```
$ cd ~/rubiks-cube-solvers/5x5x5/
$ java -cp bin -Xmx8g justsomerandompackagename.reducer LLBUULLBUUDUUDDLLLBBLLURRDDUUBDDUUBDDDFFDDFBBDDFBBFLRBBFLRBBBBRDDDDLRRDDLRRFFLFFRRLDDRRLBBRRBRRRRBRRUULUUFFLUUUUFRRBBFFLBBFFLLLLDDLLDFFFFBUUUURFFUURFF```
```
