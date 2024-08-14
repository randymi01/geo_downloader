# geo_dl

geo_dl is a python CLI tool for downloading, extracting, and organizing GSEs containing 10x single cell counts data into format able to be read in by seurat or scanpy.

## Requirements

* Requests
* tqdm
* click

```bash
pip install -r requirements.txt
```

## Basic Usage
Write desired GSEs into a txt file separated by a new line
```bash
python geo_dl.py -c <codes txt file> -o <output path>
```

## Command-Line Flags

The script accepts the following command-line options:

- `-c`, `--codes` *(required)*:  
  Relative file path containing GEO accession codes.

- `-o`, `--output_path` *(required)*:  
  Relative folder path where data should be stored.

- `-d`, `--delete` *(optional, default: `False`)*:  
  Set to `True` to delete tar files after extraction.

- `-l`, `--download` *(optional, default: `True`)*:  
  Set to `True` to download tar archives. Set to `False` to skip downloading.

- `-e`, `--extract` *(optional, default: `False`)*:  
  Set to `True` to extract inner tar archives.
## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
