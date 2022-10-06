# Sample to test SHA256SUM hash

## How to use this repo

1. Clone this repo

    ```
    git clone https://github.com/lethe2211/sha256hash-sample.git
    ```

2. Check the contents of `dir1/file.dat` and `dir2/file.dat`

    ```
    cat dir1/file.dat

    cat dir1/file.dat
    ```

3. Check the hash of `dir1/file.dat` and `dir2/file.dat`

    ```
    # Windows (DOS)
    CertUtil -hashfile dir1/file.dat SHA256
    CertUtil -hashfile dir2/file.dat SHA256

    # Linux
    sha256sum dir1/file.dat dir2/file.dat

    # Mac
    shasum -a 256 dir1/file.dat dir1/file.dat
    ```

3. Tweak `dir2/file.dat`

    ```
    vim dir2/file.dat

    cat dir2/file.dat
    1
    2
    3
    4
    ```

4. Check the hash of these files again
