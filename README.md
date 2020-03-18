# Annotation for VOC Pascal

Example of augmentating image with bounding boxes.
This code is based on [aleju/imgaug](https://github.com/aleju/imgaug).

Augmentable annotation format is Pascal VOC only.

## Examples

![original.jpg](Documents/original.png)

Above image can be augmented to the following images.

| Example 1 | Example 2 | Example 3 | Example 4 |
| ---- | ---- | ---- | ---- |
| ![example1.jpg](Documents/example1.png) | ![example2.jpg](	Documents/example2.png) | ![example3.jpg](Documents/example3.png) | ![example4.jpg](Documents/example4.png) |

## Requirements

 * Python3
 * Pipenv
 * imgaug
 * cv2
 * pascal_voc_writer
 * xml.etree.ElementTree
 * shutil
 * numpy

## Usage

Put files(Images and Annotations) to augment in `input/`.
(Do not create sub directories.)

Run script.

    pipenv run python augment.py

Augmented images with annotations are generated in `output/`folder.
If there is no bounding boxes in the image, Annotation files (`*.xml`) are moved to `empty/`.

## Please do Not remove Below Folders

 * empty
 * input
 * output
 * util