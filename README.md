# iml-assignment-1

## Use nbstripout

nbstripout is a python tool which removes outputs from a notebook. This helps avoid conflicts

### Install
```bash
pip install nbstripout
nbstripout --install --attributes .gitattributes
```

If you use starship and get `No valid notebook detected on stdin` use:

```bash
git config filter.nbstripout.clean "python -m nbstripout 2>/dev/null || cat"
```