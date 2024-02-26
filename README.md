# Portfolio
___
## Multithreaded Sudoku Solver
[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Multithreaded-Sudoku-Solver)

This project was made with <b>Java (Libraries: Concurrent, Arraylist)</b>.

This software takes a Sudoku board as an input (array of numbers from 1 to 9, with 0's representing empty cells), solves the board through a recursive algorithm and prints the result.

An example of an initial Sudoku board to solve:

![starting board](https://github.com/RealMaximeCaloz/Portfolio/blob/ba2f7d42176e32726565c832dc0f597c661cd021/startingboard.png)

If the board is unsolvable, that information will be printed for the user.

A new ExecutorService job is submitted for each number which would be a valid guess for the Sudoku board's first empty cell, hence harnessing the power of multithreading and parallel processing.

The Sudoku board is solved very quickly, even if it is near-impossible to solve for humans:

![final board](https://github.com/RealMaximeCaloz/Portfolio/blob/77fe443203d9171137cb02da38cdd3406de40a03/finalboard.png)

___
## Commercial Bulk Instagram Post Generator
[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Commercial-Bulk-Instagram-Post-Generator)

This project was made with <b>Java (Libraries: AWT, I/O, Graphics)</b>.

This software takes into input a folder filled with images (backgrounds for posts), and an array of strings with the text to add to each post.

This software will crop all the images in bulk down to square size, dim the images to increase contrast with text, and will add 1 string from the array of strings to each image.

This effectively generates Instagram posts in bulk extremely quickly with little-to-no effort.

You can even brand the posts with your own Instagram handle, to prevent content stealing, and free publicity.

If you want to generate 1000 posts in seconds, so that you do not have to worry about content creation for the next 3 years, you can simply use this software.

Example of a generated Instagram post:

![generated post example](https://github.com/RealMaximeCaloz/Portfolio/blob/9bafd87537acef1f05bb3b98450d5e4c2e436707/GeneratedInstagramPostExample.jpg)

A [REST API version](https://github.com/RealMaximeCaloz/REST_API) of this program has also been created to practice using Spring Boot and Thymeleaf.

The REST API features a front-end which accepts a String and an image as inputs.

![api_inputs](https://github.com/RealMaximeCaloz/Portfolio/blob/17861c2ebc76d13eea9eb51ff4c8d721b5c5d1b0/pic1_rest_api.png)


The API adds the text to the image provided, and returns the processed image to the user on the front end.

![api_outputs](https://github.com/RealMaximeCaloz/Portfolio/blob/17861c2ebc76d13eea9eb51ff4c8d721b5c5d1b0/pic2_rest_api.png)

___
## Image Cryptography Tool
[Click here to view this project's code repository](https://github.com/RealMaximeCaloz/Image-Cryptography-Tool)

This project was made with <b>Python (Libraries: PIL, NumPy)</b>.

This software uses bitwise operations to cloak a given image within the image information of another image, making it nearly invisible to unsuspecting parties.

Example of an image to hide:

![image to hide](https://github.com/RealMaximeCaloz/Portfolio/blob/7b6f6c8bc71cd3dca12de19d0a39c66480079096/epiccar.jpg)

Example of the container image in which you want to cloak your hidden image:

![container image](https://github.com/RealMaximeCaloz/Portfolio/blob/7b6f6c8bc71cd3dca12de19d0a39c66480079096/basiccar.jpg)

After running this software, you obtain a combined image which contains the hidden image, but it looks very much like the unmodified container image.

Example of the combined image, which contains the hidden image:

![combined image](https://github.com/RealMaximeCaloz/Portfolio/blob/7b6f6c8bc71cd3dca12de19d0a39c66480079096/composite-image-with-hidden-image.jpg)

You (or the party you are trying to send a hidden message to) can also run an image extractor in the software, which will extract the hidden image from the combined image.

Example of the hidden image extracted from the combined image:

![extracted image](https://github.com/RealMaximeCaloz/Portfolio/blob/7b6f6c8bc71cd3dca12de19d0a39c66480079096/hidden-image-extracted-from-composite.jpg)

As you can see, the extracted hidden image has inherited a few visual artefacts.

However, its depiction is still blatantly obvious, despite having been secretly cloaked in a completely different image.
