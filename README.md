# secret-htmls
- https://tarv7.github.io/secret-htmls/

## How to encode
### Pre requisites
- Install staticrypt
### Prepare keys file
- Run `cp keys.sample.txt keys.txt`
- Change `keys.txt` values
### Encode HTML
- `staticrypt input_path.html --password $(cat keys.txt | grep page-x: | sed 's/page-x://g') --short`
