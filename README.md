# NN
it is required to make a neyral network that can identify hand written numbers.so i am going to explain this code:-
first I used the MNIST dataset and imported it to the code, it consists of 785 coulums where each row represents the pixels of an image and a label at the first coulumn.I made two variables one for the number of rows and the other for the number of columns (m,n).then  we found the transpose of the function making each coulumn representing the image where it will be much easier and simplified .
when we design a neural network. it mainly consist of input values(A0) (in our case it is each  coulumn of the matrix of MNIST representing  the pixcels of  a single image) and then hidden layers (2 hidden layers in our case) (Z1,Z2) and finally the output value which is the predtected number.
we first find the dot product of each  image array and multiply it with and array of random weigths with 784 size ranging in value between -0.5 to 0.5 and we add that to a random bias(we apply that to each neuron found the first layer(10 neurons )).
we can look at numbers as combunation of lines and curves which we call edges. the last layer can help as in searching for certain edges and comparing it to the patern of values made by learning from previous errors.
 before we pass the output value to the second layer, we need to pass them to the ReLU function which make sure there is no negative values (A1). then we make the same dot product to the output array of first layer (A1) and random array of weights (W2) .we pass the output values to the softmax function which will turn the output values into probabilty values.the code will then choose the number with the highest probability.
the we calculate the error by comparing the predicted values with actual values and the code will train to change the weigth and bias values untill it reaches the most accurate values.

# diffrence between tensorflow and building from scratch
tensorflow was much easier in writing the code but it will be restricted to certain application so if you have a specific problem that requires deep learning writing the code from scratch will be more flexibility and better performance 
