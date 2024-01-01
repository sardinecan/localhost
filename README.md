# localhost
Several solutions for running a local HTTP server

## Python 
### Python 3
```bash
python3 -m http.server --directory /path/to/directory
```

## Julia
```julia
pkg> add LiveServer
```
### Repl
```julia
julia> using LiveServer
julia> serve(host="0.0.0.0", port=8001, dir=".")
```
### Terminal
```bash
julia -e 'using LiveServer; serve(host="0.0.0.0", port=8001, dir=".")'
```

