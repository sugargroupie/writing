# Adding Images in the Sitecore XM Experience Editor
This guide is designed for beginner-level users who are just starting with the Sitecore XM Experience Editor. It covers two primary methods for placing images on full-width and medium-width page types:
- Users with access to the Insert Code Snippet item in the Rich Text Editor (RTE) can place images through the Body Copy component.
- All access users, and those specifically without access to the Insert Code Snippet item in the Rich Text Editor, can place images through the Flex Image component.

Both methods allow you to integrate images with features such as in-line with text, left-aligned or right-aligned of the text, code snippets, captions, and custom flex settings. These options ensure that images are responsive and accessible.

Aligned images on a page should always follow the heading in the HTML, just as all content should follow the heading that defines the section to which it belongs. Verify its order in mobile view or in the HTML code, as it is not visually apparent on desktop layouts.

Follow the sections below to learn how to add components, upload assets to the Media Library, optimize your images, and implement accessibility requirements.

**Note:** add preferred images to the Media Library before attempting to use either component.

<br>

## 1. Placing Images Using the Rich Text Editor (RTE)
The Rich Text Editor embedded in the **Body Copy Component** is ideal for content-rich pages where text and images are mixed together. This component provides you with the following features:
- **Insert a Media Link:** Embed images directly from the Media Library.
- **Insert a Code Snippet:** Add custom HTML or embed options as needed.
- **Provide a Caption:** Supply additional context for your images.

### How to Add the Body Copy Component
1. In the Experience Editor, click the **Add Component** button.
2. Click **Add Here** to place the component on the page where you want your content to appear.
3. Go to the PAGECONTENT tab and select the **Body Copy** component, which includes the Rich Text Editor.
4. Click anywhere on the background of the component to bring up the editing ribbon.
5. Select the rectangle button on the left to open the editing window.
6. Click the **Insert Code Snippet** button. Select **Flex Image** setting to add a placeholder image and caption to the window.
7. Swap out the placeholder content with your preferred image and caption text. Click the **Accept** button.
8. Save the page.

### Uploading Images to the Media Library
- In the Content Editor, open the Media Library, navigate to the appropriate site folder, and click Upload.
- Select an optimized image file based on your display requirements.
- Update metadata fields such as title, caption, and Alt Text to ensure the image is accessible.

### Example: Embedding an Image in RTE
  ```html
  <p>Welcome to our new archive! Below is an image that adds context to our story:</p>
  <figure>
    <img src="/media-library/path/to/your-image.jpg" alt="A brief and descriptive alternate text" />
    <figcaption>Image Caption: A snapshot of our latest project progress.</figcaption>
  </figure>
  <p>Feel free to explore further details in the text below.</p>
</div>
```

> Explanation: The snippet above uses `<figure>` and `<figcaption>` to wrap the image with its caption, ensuring both visual appeal and adherence to accessibility standards.

<br>

## 2. Placing Images Using the Flex Image Component
The Flex Image Component is optimized for responsive image layouts and provides more control over image placement and styling. This component includes:
- **Direct Image Insertion:** Choose images directly from the Media Library.
- **Caption Field:** Add a caption below the image.
- **Flex Settings:** Customize image layout settings for responsiveness. The options are:
  - Flex-25-Left
  - Flex-25-Right
  - Flex-33-Left
  - Flex-33-Right
  - Flex-50-Left
  - Flex-50-Right

### How to Add the Flex Image Component
1. In the Experience Editor, click the **+ Add Component** button.
2. Click **Add Here** to place the component on the page where you want your content to appear.
3. Go to the PAGECONTENT tab and select the **Flex Image** component.
4. Save the page.
5. Click anywhere on the component to bring up the Flex Image editing ribbon.
6. Select the rectangle button on the left to open the editing window.
7. Set values for the following fields:
   - Image
   - Caption
   - Flex Setting

### Uploading Images to the Media Library
- In the Content Editor, open the Media Library, navigate to the appropriate site folder, and click Upload.
- Select an optimized image file based on your display requirements.
- Update metadata fields such as title, caption, and Alt Text to ensure the image is accessible.

### Example: HTML for Flex Image
```html
<div class="flex-33-right"><img src="/media-library/path/to/flex-image.jpg" alt="A detailed description for accessibility" /><span class="flex-caption">Image Caption: A concise explanation of the image.</span></div>
```
 
> Explanation: This screenshot displays the flex settings for the image, its caption, and alternative text.

<br>

## 3. Tips and Tricks

### Image Optimization Tips
- Compression: Use online tools like TinyPNG or Polarr Pro Photo Editor to reduce file sizes without sacrificing quality.
- Resolution: Upload images in resolutions optimal for web display. Avoid using images that are larger than needed.
- File Format: Consider using modern formats such as PNG or WebP for improved compression efficiency. JPEG may be used for high-quality photographs.

### Accessibility Requirements
- Alternative Text (Alt Text): Always provide descriptive alt text for images to aid users with screen readers.
- Captions: Use captions to offer clarity and context to your images.
- Contrast: Ensure that any text overlaid on images has sufficient contrast to maintain readability.

### Troubleshooting Common Mistakes
- Image Not Displaying: Verify that the image path is correct and confirm the image has been uploaded to the Media Library.
- Missing Alt Text or Caption: Ensure you provide appropriate alt text and that the caption fields are filled to meet accessibility standards.
- Layout or Flex Issues: For the Flex Image Component and Body Copy Component work in tandem, recommended use is to always insert the Flex Image directly above the Body Copy.

<br>
By following these guidelines, you can effectively integrate images into your pages with best practices in component usage, media uploading, image optimization, and accessibility. If you have any questions or need further examples please share your thoughts!
