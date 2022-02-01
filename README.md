# Invert Color Shader for Unity
Hello everyone!

I was looking for a simple free invert color shader for ages. I fed up with it so I decided to make my own. 
I'm giving it for free! You are free to use it in any way you want (commercial or personal)

Though I would appreciate if you credit me in the projects you're working on

**Features:**
- Inverts Color (Any pixel on the screen, UI image or not)
- Mask Texture
- Texture Tint
- Works with existing Unity UI features such as filled or sliced image
- Also works with 3D objects if you ask it nicely

![Image1](https://i.imgur.com/Zt2huoW.png)

![Image2](https://i.imgur.com/8m64mT8.gif)

![Image3](https://i.imgur.com/XtXyfYa.png)


**How to use?**
- Import the shader to your project (drag-drop to a folder)
- Create a new Material and change the Shader type to InvertUI
- Optional: Pick a mask texture
- Create an image with a canvas.
- Assign the material you've created to the material property of the image ([See here](https://i.imgur.com/eEKmjZN.png))
- Thats it! 

**Issues**
- Sidenote: Source Image property of the Image component does not work with the shader. So it does nothing. If you want to change the mask, change the Tex property of the material)  
- The mask texture needs to have alpha. So the pixels of the texture where you want it to invert should have bigger than 0 alpha and other parts should have exactly 0 alpha. So a black and white texture would not work.
- Does not support canvas group alpha or half transparency. It either has full inversion or not
- Doesn't mask an another image this shader shader. So no two images can combine. One will pass through another
- Made with Amplify Shader Editor


I hope this helps! Keep developing!
