# Video to PNG Converter

This Python script converts videos to a series of PNG images, allowing users to specify the frame rate at which images are saved. Additionally, it offers an option to remove the background from each image before saving.

## Installation

To run this script, you'll need to ensure you have the required Python libraries. Install them using the `requirements.txt` file provided in this repository.


## Installation

To run this script, you'll need to ensure you have the required Python libraries. Install them using the `requirements.txt` file provided in this repository.

```
pip install -r requirements.txt
```


## Usage

Ensure you have Python 3.6 or newer installed on your system. Clone this repository or download the script and `requirements.txt` file. Then, install the required libraries as mentioned above.

To use the script, run it from the command line with the desired options:

```
python video_to_png.py [options]
```



## Options

- `-i`, `--input` <input_file>: Specify the path to the input video file. If not provided, the script will attempt to use the first video file found in the current directory.

- `-o`, `--output` <output_folder>: Specify the path to the output folder where PNG images will be saved. If not specified, images are saved to a default `output` directory at the root of the program.

- `-f`, `--fps` <frames_per_second>: Specify the number of frames per second to save. By default, all frames are saved (`-1`). Setting this to a positive number will save frames at the specified rate.

- `-r`, `--remove_bg`: Enable background removal from each image before saving. By default, this feature is disabled.

- `-h`, `--help`: Display help information showing all command-line options.

## Example

To convert a video named `example.mp4` into PNG images, saving every frame, with the background removed, and write them to the `./output_images` directory, you can use the following command:


```
python video_to_png.py -i example.mp4 -o ./output_images -r
```

If you want to save images at 10 frames per second without removing backgrounds, you would use:

```
python video_to_png.py -i example.mp4 -o ./output_images -f 10
```


## Issues

If you encounter any issues or have suggestions for improvements, please submit them to the GitHub issue tracker for this project.
