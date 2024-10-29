## Meteor Challenge
### Processo seletivo para Estágio na Tarken - Victor Ferreira Alvarenga
### The challenge
The challenge is to read an image and identify stars, meteors and water by its colors. By doing that, I'm able to count how many stars and meteors there are in the sky. Also, by getting the image width, it is possible to verify each pixel column and check if meteors and water bodies are aligned, thus meaning that meteors will fall on water.

### What did I use?
Python and one of the most popular image libraries: OpenCV. I've also had to use Numpy Arrays to manipulate image values.

### How the script works for counting stars and meteors?
Initially, the script creates masks using RGB (Red, Green and Blue) color schem, which allows individual pixels to be filtered by its colors. By using ```countNonZero()```, OpenCV treats any pixel from an outside color mask as a "zero". 
The results from this implementation is:
- Number of stars: 315
- Number of meteors: 328

### And how the script verifies which meteors will fall on water?
The script iterates through each pixel column of the image. If it finds any water mask in the column, it means that any meteor in this very same column will fall on water.

### What's the message in the sky?
As I'm not an expert in working with images, I could only think about iterating again through the image and translating it to some code like Morse. Unfortunally, none of the messages I translated made any sense. The results and approach methods are explained in the Jupyter Notebook file.



