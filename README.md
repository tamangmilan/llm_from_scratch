You can run this colab notebook on a free google colab - T4 GPU. 
I've reduced the number of training data so that anyone should be able to successfully train and inferencing yourself within like 5 min time. 

The model will give much better accuracy if you increase the number of dataset. It might take longer time but you should definitely give a try. 
Below is the code where you can increase the number of training dataset. 

# Just update the number 1500 to any number if you want to traing for longer period of time to get more accurate result. 
# In similar way, you can also increase validation dataset below. You can find this line of code block is in step1 of colab notedbook.

raw_train_dataset, rt_to_skip = random_split(train_dataset, [1500,len(train_dataset)-1500])
raw_validation_dataset, vt_to_skip = random_split(validation_dataset, [50,len(validation_dataset)-50])
