# rubiks-cube-solvers
A collection of solvers for various size rubiks cubes
- 2x2x2 python solver from http://codegolf.stackexchange.com/questions/35002/solve-the-rubiks-pocket-cube
- 3x3x3 C solver from https://github.com/muodov/kociemba
- 4x4x4 Java solver from https://github.com/cs0x7f/TPR-4x4x4-Solver
- 5x5x5 Java solver from xyzzy (source code not included per author's request)

If anyone has a 6x6x6, 7x7x7, or NxNxN solver that they would like to
contribute I would love to find one.

NOTE that I did not write any of these solvers.  This is just a
collection I put together with instructions.

The input for all of the solvers is a single string description of all six
sides in U, R, F, D, L, B order. They all use this order because the
3x3x3 kociemba solver uses this order and that was the first solver I ever
experimented with so I tweaked the other solvers to accept the same input to
make life easy.


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
$ rubiks_2x2x2_solver.py URBRFBDRLULFBLRDFDFUULBD
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
$ sudo apt-get install default-jre openjdk-7-jdk
$ cd ~/rubiks-cube-solvers/4x4x4/TPR-4x4x4-Solver/
$ ./make.sh
$ java -cp .:threephase.jar:twophase.jar solver UUURUUUFUUUFUUUFRRRBRRRBRRRBRRRBRRRDFFFDFFFDFFFDDDDBDDDBDDDBDDDLFFFFLLLLLLLLLLLLULLLUBBBUBBBUBBB
```

### Install 5x5x5 solver
The first time it solves a cube it creates several prune tables.  Creating
these prune tables will take a while (more than 30 minutes on my laptop) but
you only have to do this once.

```
$ sudo apt-get install default-jre openjdk-7-jdk
$ cd ~/rubiks-cube-solvers/5x5x5/
$ java -cp bin -Xmx8g justsomerandompackagename.reducer LLBUULLBUUDUUDDLLLBBLLURRDDUUBDDUUBDDDFFDDFBBDDFBBFLRBBFLRBBBBRDDDDLRRDDLRRFFLFFRRLDDRRLBBRRBRRRRBRRUULUUFFLUUUUFRRBBFFLBBFFLLLLDDLLDFFFFBUUUURFFUURFF```
```
