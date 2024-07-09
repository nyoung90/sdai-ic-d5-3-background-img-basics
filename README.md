# Parallax Effect Implementation

## Instructions

Follow these steps to create a parallax effect on a webpage:

1. [ ] **Create a New HTML File**
   - Create a new `index.html` file and add the basic boilperplate and structure. **Recall:** use `!` the hit `enter` to quickly and easily add boilerplate to your HTML file, which should now look something like this:
     ```html
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Parallax Effect</title>
         <link rel="stylesheet" href="styles.css">
     </head>
     <body>

     </body>
     </html>
     ```

2. [ ] **Add a `<section>` Element w/ PLaceholder Text**
   - Add a `<section>` element with a class of `parallax-section`:
     ```html
     <section class="parallax-section"></section>
     ```
   - Inside this section, add multiple paragraphs of lorem ipsum text to take up more than 2/3 or a screen's worth of space both above and below the image. Use your AI for help as needed, as it can rapidly produce a great deal of lorem ipsum already in paragraph tags.
   - **EXample Prompt**: Produce 12 paragraphs of lorem ipsum in HTML paragraph tags. Each paragraph should have at least three long sentences. 

3. [ ] **Find and Add an Image**
   - **Find an Image**: Use [Pexels](https://www.pexels.com) or [Unsplash](https://www.unsplash.com) to find a suitable image. Ensure the image is of high quality and free to use.
   - **Download the Image**: Click the download button on the chosen image to save it to your computer.
   - **Create Directory**: In your VS Code workspace, create a directory named `assets`, and within it, create another directory named `images`.
   - **Add to VS Code**: Move the downloaded image to the newly created `assets/images` folder within your VS Code workspace.

4. [ ] **Set as Background Image**: Update the `background-image` property in your CSS file to target the new image:
     ```css
     .parallax-section {
         background-image: url('assets/images/your-image-file.jpg');
         background-size: cover;
         background-repeat: no-repeat;
         background-position: center;
         background-attachment: fixed;
         max-height: 50vh; /* Set maximum height to 50vh */
     }
     ```

5. [ ] **Provide Attribution**: Add attribution for the image in this README file:
     ```markdown
     ## Image Attribution
     - Image used in the parallax section by [Photographer Name](URL-to-photographer-profile) from Pexels/Unsplash
     ```


### Explanation of CSS Properties
- **background-image**: Sets the background image for the section.
- **background-size: cover**: Ensures the image covers the entire section.
- **background-repeat: no-repeat**: Prevents the image from repeating.
- **background-position: center**: Centers the image within the section.
- **background-attachment: fixed**: Creates the parallax effect by fixing the background image in place while the rest of the content scrolls.

### Additional Notes
- Ensure the file path in the `url('assets/images/your-image-file.jpg')` is correct relative to your CSS file location.
- The `max-height: 50vh` property ensures the section's height does not exceed half of the viewport height (the veiwable area as adjusted for the device).
- Always provide proper attribution for images according to the guidelines of Pexels or Unsplash.
- Test your design across different screen sizes to ensure the parallax effect works well.