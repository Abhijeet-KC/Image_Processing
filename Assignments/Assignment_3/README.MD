# HSV and RGB spaces
## Image Processing and Color Space Analysis

## Guidelines

1. **Pick an image of your choice and plot it**

2. **Convert it into HSV space and plot it**

3. **Isolate channels**
   - From RGB: R, G, B channels and plot them
   - From HSV: H, S, V channels and plot them  
   - Use a grid (subplots) to show them together

4. **Visualize RGB and HSV space in a scatterplot**  
   - Create scatterplots for RGB and HSV  
   - Make the plot interactive if possible

5. **Custom function to adjust brightness**
   - Arguments: Image and adjustment factor  
   - Operation: Adjust brightness in HSV space (by scaling V channel)  
   - Return: Brightness adjusted RGB image  

6. **Generate brightness variations**
   - Use the function to create:  
     - One darker image  
     - One brighter image  
   - Plot original, darker, and brighter images in a grid  

7. **Histograms**
   - For original image: RGB histogram and Hue histogram  
   - For darker image: RGB histogram and Hue histogram  
   - For brighter image: RGB histogram and Hue histogram  
   - Plot them side by side in a grid  

8. **Feature extraction & clustering**
   - Extract features from RGB and HSV spaces  
   - Apply KMeans with `n_clusters=1`  
   - Use **inertia** to measure compactness  
   - Compare compactness in RGB vs HSV  

---

## Bonus
HSV histograms may look more compact, but:  
- Compactness ≠ classifier performance  
- Different classes may overlap in HSV despite lower inertia  
- Histograms ignore spatial information in images  
- Classification performance depends on dataset, task, and features, not just histogram compactness
