# NewsClassfier

## Thought process :thinking:
I had to do something on my own to brush up what I had learned in the udacity course so I was searching for ideas I was by struck how news papers:newspaper:
classify its content into diffrent sections and if it could be automated 	:wrench: using NLP.

## Hunt for the dataset
I had now started the hunt for the dataset and after 2 days searching I had found nothing but I had eye on dataset provided on kaggle by BBC but it was for text
summary but I had a idea how to tweak it to get it my way. So decided not to waste more time on finding the dataset.

## Preprocessing
Now here comes the hard part :fearful: . I had the dataset already spilt into its section but now I had to load it into an array but not all of them had same number of files and some files were only readble in binary encoding.

After this I had to go through the normal procedure of making them into a single line tokennize it , put paddings in place and split it into traning and valdataion set.

## Model
I actually started out with a embedding layer and two bidierctional LSTMs and it did what all my models do the first the first time they over fit :slightly_frowning_face:.
Then I made it one Bidirectional LSTMs still over fit then I had to move to GlobalAveragePooling1D layer to fix it it gave me an accuracy of 82% which I was happy :smile: with.

