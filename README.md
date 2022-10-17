# TDDC-301 template

## Ceedling
The projects can be tested locally using either ceedling directly or docker

### Direct
```
$ cd cd solutions/exercise-N
$ ceedling test:all
```
### Docker
```
$ cd cd solutions/exercise-N
$ docker run -v $(pwd):/usr/project -ti feabhas/ceedling ceedling test:all
```
## GCov
```
$ cd cd solutions/exercise-N
$ ceedling gcov:all
$ ceedling utils:gcov
```

## Documentation
To generate the Doxygen documentation: 
* `$ cd solutions/exercise-N/src `
* `$ docker run --rm -it -v $(pwd):/app corentinaltepe/doxygen doxygen Doxyfile`

The generated html can be found at:
`doc/html/index.htm`
e.g.
`./solutions/exercise-1/src/doc/html/index.html`
