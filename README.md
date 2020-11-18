# cs7gv1_Assignment-1
Assignment 1 repo

Both parts are notebooks made with Google Colab. You should be able to run all for part A but part B is extremely slow. Google Colab and cv2_imshow() should display correctly, jupyter and plt.imshow() is a little buggy.

## A

### 3. Picking K

I wasn't exactly sure what to do here. I plotted the square root of the eigenvalues and you can see that the first 5 or so eigenvectors contribute a huge amount of the information, but despite this k=10 looks terrible. I picked k=15 because the plot seems to have mostly leveled out at that point and the remaining vectors should have little to contribute. Subjectivley, k=15 still left a lot to be desired.

### 4. Comment on Quality

Using 100 components you get a pretty good reconstruction of the image, while k=10 and k=15 are subjectively terrible. While not asked for, I think k=1 is probably the most interesting construction. The idea that a roughly flat grey component is the most important for contributing to the overall image makes sense. It sets a kind of baselayer of overall intensity for each patch which the other components can build on. I'm guessing the quality of reconstruction you get from a number of components also varies a lot with the size of image and number of patches.

## B - Mean Shift Filtering

Didn't get very far with this part of the midterm. There's a bit of information in the notebook.
