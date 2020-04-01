# Ideal Image Digit Classifier
The idea is simple. Add up every image with the corresponding labels and take the average. I called them the "ideal images" because they were a direct result from the images given. 

# Resources
For this project I decided to use MNIST digit data set, http://yann.lecun.com/exdb/mnist/, so I ended up having 10 ideal images, 1 for each digit. In all, the memory required to store the ideal images would be 7840 bytes (Height: 28 x Width: 28 x Classes: 10). I also used https://scikit-learn.org/ for other models to compare performance.

# Performance
The model got about 82% accuracy on the test data. When compared to logistic regression and neural networks, it falls short. Logistic regression was able to reach around 91% accuracy and the shallow neural network was able to attain around 98%. However, considering the ideal images model and code can be stored within less than 10 kilobytes of code and run on virtually any system due to the light-weight calculations, I say that could potentially be a trade off.

# Room for improvement
As of right now I am working on the difference calculation, that is the difference between the ideal images and the actual images. I just used a basic euclidian distance but I feel like there is a better one out there. 
Additionally, I believe that the score calculation can be improved too, as of now the only thing contributing to score is the difference. The score is how confident the ideal image model is that an image is a part of a class.

# Interactive online Jupyter notebook, 
https://mybinder.org/v2/gh/SjDuque/Ideal-Image-Digit-Classifier/03898b59b1a3086b70cc2132e697f67203dce08c?filepath=Ideal-Image%20Number%20Classifier.ipynb
