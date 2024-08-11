Project: Image Compression using C++

Image compression refers to compression of data that is applied to digital images in order to reduce their transmission and storage costs.Image Compression is the technique of reducing the image size without degrading the quality of the image. Image Compression is the solution associated with transmission and storage of large amount of information for digital Image. Transmission of Images includes different applications like broadcasting of Television, remote sensing via satellite and other long-distance communication while Image storage is required for medical images, satellite images, documents and pictures. Image compression deals with these types of applications.

One of the fundamental compression techniques that has been helpful for image and video compression standards is Huffman coding. Huffman coding is an essential method for achieving effective data representation in image compression algorithms. This technique, named for its creator David A. Huffman, is widely used in many image compression standards, including JPEG and PNG. Huffman coding is a form of entropy encoding that assigns variable-length codes to input symbols based on their frequencies of occurrence. The basic principle is to assign shorter codes to more frequently occurring symbols and longer codes to less frequent symbols, thereby reducing the average code length compared to fixed-length codes.

Prefix codes, or variable-length codes assigned to input characters, are bit sequences that are assigned so that the code assigned to one character does not prefix any other character's code. By doing this, Huffman Coding ensures that the generated bitstream can be decoded without any ambiguity. There are two major parts in a Huffman coding technique, first is to build a Huffman tree from inputs and second is to traverse the Huffman tree and assigning codes respectively.

This project involves implementation of Huffman algorithm for the purpose of lossless image compression. The proposed methodology is as follows: 

•	Read the input image (.bmp) and store its width, size, height and information of pixels in a structure (struct imageInfo). 

•	Save the information of each pixel such as intensity/RGB values and the corresponding hex values (class Pixel).

•	Identify and calculate the total number of distinct colors of the respective image.

•	Store the frequency and hex values of each distinct color respectively (class Color).

•	Create a Huffman’s Tree using all the stored information and save the bit codes/huff codes with respective hex values and frequency of colors.

•	The header of a new file is created in order to store the further information. 

•	The entire image matrices is traversed and corresponding bit codes of each pixel’s color is written in the file.

•	The written file is saved having the new information (such as frequencies ad hex values) of the compressed data formats.

Huffman coding successfully makes image files smaller without sacrificing quality. On average, it reduced file sizes significantly, showing clear benefits for saving storage space and speeding up data transfer. It performed well in maintaining image clarity, although there's room to make the encoding process faster. Overall, Huffman coding is a straightforward and effective method for compressing images efficiently, with potential for even better techniques in the future.
