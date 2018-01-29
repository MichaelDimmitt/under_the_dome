## under_the_dome - testcoverage, makes for an update.
Good test coverage ensures output.

![under_the_dome](https://user-images.githubusercontent.com/11463275/35491585-4f353cc2-0475-11e8-8b8b-ba56ec7cae68.png)

### js-node, test coverage allows, UpdatePackages. RemoveUnused Packages.

## How it works, UpdatePackages:
Requires 90 percent test coverage before it will run for your application.

1) finds packages that have the most dependencies to evaluate first.
2) incrementally updates the package 
3) and runs test suite
4) until the application breaks <br>(if single test or more fails. store test failure output and version<br>keep last healthy package and move on to the next package)
5) (if no future package is found move on to the next package) until program end.

## How it works, RemoveUnused Packages:

1) find packages of largest size and least dependencies to evaluate first.
2) removes packages one by one 
3) (if single test or more fails. store test failure output and version <br>Keep the package instead of deleting on healthy package version and move on to the next package)
4) (if no future package is found move on to the next package) until program end.
