# Imagix - Rust Image Resizing Tool

Imagix is a Rust-based image resizing tool designed to efficiently resize images to specified dimensions. It supports both single image and batch resizing, providing flexibility and ease of use.

# Technologies
- Rust
- Image library
- Structopt

## Features

- **Size Options:** Choose from three predefined size options - Small, Medium, and Large.
- **Modes:** Operate in two modes - Single (resize a single image) and All (resize all images in a folder).
- **Supported Formats:** Imagix supports JPEG and PNG file formats for resizing.

## Usage

### Resize a Single Image

```bash
imagix resize --size <small/medium/large> --mode single --folder <path_to_image>
```

### Resize All Images in a Folder

```bash
imagix resize --size <small/medium/large> --mode all --folder <path_to_folder>
```

## Size Options

- `Small`: 200x200 pixels
- `Medium`: 400x400 pixels
- `Large`: 800x800 pixels

## Examples

### BEFORE ( Size = 128,244 bytes )
![Before](./imagecli/tmp/images/image1.jpeg)

### AFTER ( Size = 5,160 bytes )
![After](./imagecli/tmp/images/tmp/image1.jpeg)


### Resize Single Image

```bash
imagix resize --size small --mode single --folder /path/to/image.jpg
```

### Resize All Images in a Folder

```bash
imagix resize --size medium --mode all --folder /path/to/images/

```

### Get statistics from a folder containing image files

``` bash
imagecli stats --srcfolder <SRCFOLDER>
```

## Building

To build Imagix, ensure you have Rust installed on your system. Then, run:

```bash
cargo build --release
```

## Testing

Imagix comes with a test suite to ensure functionality. Run the tests using:

```bash
cargo test
```

## Current state
The library only outputs JPEG image format

## License

Imagix is licensed under the [MIT License](LICENSE).
```

