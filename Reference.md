
## Reference for preprocessing techniques and baseline model

1. **Paper Name:** Classification of X-Ray Images for Pneumonia Detection Using Texture Features and Neural Networks.
**From** https://link.springer.com/chapter/10.1007/978-3-030-35445-9_20 | Intuitionistic and Type-2 Fuzzy Logic Enhancements in Neural and Optimization Algorithms: Theory and Applications pp 237-253.

	**Preprocessing steps:** 
		
	a. Resize to Region of Interest:
		For pneumonia, RoI appears as a region of white cloudy figure inside lungs, specifically inside black space, known as air space.

	b. Crop to only chest area

	c. Histogram Equalization

	d. Gray level Co-Occurence Matrix: Mappiing gray level change vectors on gray level domain.
 
	e. Use Image Texture parameters: Contrast, Entropy and Homogenety

	Model:	Accuracy: 93% 
< Image>
	
	
2.  **Paper Name:** Attention-Guided Convolutional Neural Network for Detecting
Pneumonia on Chest X-R

	**From** IEEE Xplore
	
	**Preprocessing steps:** 
		    
	a. Replace pneumonia region of image by average value of image and use it as a non-pneumonia image to increase focus on preumonia region.


	b. Use U-Net/CNN based segmentation to isolate lungs. 

3. CNN vs MLP: https://www.semanticscholar.org/paper/Models-of-Learning-to-Classify-X-ray-Images-for-the-Saraiva-Santos/0b8f202505b3d49c42fd45d86eca5dbd0b76fded

4. NLP based processing of Clinical notes/comments/interpretations of Chest X-Ray images  https://bit.ly/39Wqf2w
