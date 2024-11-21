# haraganUEx
3D design and fabrication of a "haragan": a simple four-sticks tool to remove mud and dirty.

## Motivation

To design and be able to fabricate useful tools, using surrounding waste materials to help in a disease, is very motivating.

In this case we where impacted by recent water and mud flood, 29-30th october 2024, at Valencia, Spain. Resulting in more than 200 deads and
uncountable material wounds.

After the flood, they do not have access to tools to remove the dirty and we were motivaded  

## Motivation

<img width="600" src="https://github.com/user-attachments/assets/026a4247-c13c-4fa0-b14e-653e6763bccc">


<img width="600" src="https://github.com/user-attachments/assets/e8b70895-7735-4da8-910b-6f1643edd989">



# from_ods_to_imagematrix

Extract contents from a Open Office sheet's columns and convert it to text in image arrays.
Can rescale the input image with command line arguments. 

## Requires

- Python 3

- Libraries:
  - [pyexcel](http://docs.pyexcel.org/en/latest/): to read and write libre office and excel sheets
  - [PIL](https://pypi.org/project/Pillow/): to modify and create images with texts
  - [argparse](https://docs.python.org/3/library/argparse.html): to read arguments from command line

Can all be installed in one step using:

`pip install -r requirements.txt`

## Usage:

From Linux command line:

`python3 ./from_ods_to_imagematrix_V6.py [ARGUMENTS]`

Arguments:

-  -h, --help            show this help message and exit

- --outWidth [OUTWIDTH], -ow [OUTWIDTH]
                        Width in mm of the output image

- --outHeight [OUTHEIGHT], -oh [OUTHEIGHT]
                        Height in mm of the output image

- --inWidth [INWIDTH], -iw [INWIDTH]
                        Width in mm for the scaled input image

- --inHeight [INHEIGHT], -ih [INHEIGHT]
                        Height in mm of the scaled input image

- --datasheet [DATASHEET], -d [DATASHEET]
                        Input data sheet file name

- --imagefile [IMAGEFILE], -i [IMAGEFILE]
                        Input image file name

- --fontfile [FONTFILE], -f [FONTFILE]
                        Truetype font file name

- --fontsize [FONTSIZE], -s [FONTSIZE]
                        Truetype font size (pt)


## Examples:

Example for Linux command line for one field matrix generation:

`python3 ./from_ods_to_imagematrix_V6.py -ow 1000 -oh 800 -iw 43 -ih 43 -d datasheets/table_names_1.ods -i images/base_llavero_V0.1.png -f  fonts/Misyalli-dafont.ttf -s 24`

