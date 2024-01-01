# localhost
Several solutions for running a local HTTP server

## Python 
First check your python version installed: 
```bash
python -V
# or
python3 -V
```

### Python 2
```bash
cd /path/to/directory
python -m SimpleHTTPServer <port>
```

### Python 3
```bash
python3 -m http.server <port> --directory /path/to/directory
```

## Julia
First you need to install `LiveServer`. Just enter following command int the the repl:
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
	
