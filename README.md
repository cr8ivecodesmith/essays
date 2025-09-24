# Matt Lebrun's Essays Site

NOTE:

Clone this repo then clone the theme repo within this directory.


## Development setup

1) Make a virtual environment and install the requirements

```
uv venv -p 3.13
```

```
direnv allow .envrc
uv pip install -r requirements.txt
```

2) Sync the [zenmatt](https://github.com/cr8ivecodesmith/zenmatt) theme

```
git submodule update --init --recursive .
```

3) Copy the favicon to the theme folder

```
cp favicon.ico zenmatt/static/img/
```

4) Run the dev server

```
pelican -r -l -p 8888
```

5) Open your [browser](http://localhost:8888)

6) Deploy changes

```
make github
```
