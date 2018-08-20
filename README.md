# Artist Identification Using CNNs
## Neural Networks and Fuzzy Logic Course Project

## Team:
1.Vaibhav Sanjay Jade 
2.Samiran Gode 
3.Pratyush Dubey 
4.Mayank Mundada

Owing to space constraints (maximum size of the zip file that could be uploaded was 10 MB), we have deleted all the data files, trained models, and pickled data structures. Only the code, script and result files are present in the zip file uploaded. We are currently preparing dataset which would be uploaded on drive and link would be provided soon.

old code contains the .ipynb codes which we tried on Jupyter notebook on using CPU. As it takes much more time on CPU, er were not able to train resnet models at that time. Thr newly uploaded files are from Colab notebooks, where I was able to run the code on Tesla K80. Basline results are in old code folder, where as the working examples of Colab is in the root folder.

## Resources:
http://cs231n.stanford.edu/reports/2017/pdfs/406.pdf

(for siamese networks)https://github.com/jadevaibhav/Signature-verification-using-deep-learning

## Dataset:
We are working with much smaller dataset than original 'Painters by numbers', provided by Kaggle. We have taken following 12 painters:
'Aleksey_Savrasov','Claude_Monet','Da_Vinci', 'Frida_Kahlo','Michelangelo','Pablo_Picasso','Paul_Cezanne', 'Pierre_Renoir', 'Rembrandt','Salvador_Dali','Van_Gogh', 'Wassily_Kandisky'. 

## Data Preprocessing:
As mentioned in the above report, we are assuming the artistic features of a painter would present even if we take a slice of whole painting. As we are more concerned with Style(bush strokes, color-schemes etc) than the painting itself. We are taking a 224x224 slice from the images randomly.

## Methodologies:
### 1. Baseline CNN
A basline model with just a few layers which is meant as benchmark for further models. The code is present in 'old code' folder.

### 2. Resnet50 with randomly intiallized weights
 50 layer deep resnet model architecture with randomly intiallized weights and trained on artist dataset.
 
### 3. Resnet50 with transfer learning
50 layer deep resnet model architecture with using weights pre-trained on Imagenet dataset and fine-tuned on artist dataset. 

### 4. Resnet50 with siamese and triplet loss
Resnet architecture trained using siamese network and triplet loss methodology. After training the Resnet50 model, I have added a sofmax classifier and just trained the classifier on the dataset.

## Comparison:
The comparisons between models is summarized in comparison.ipynb. As per the test set, the Resnet50 model with transfer learning performs significantly better than the other. Suprisingly, the siamese model performs lesser than the plain transfer learning model(wheras it is also intiated with Imagenet weights). I am further investigating the problem with the siamese training model as it is supposed to work even better.

## Few last words...
Thank you for staying with me till the end. If you liked my repo and the work I have done, feel free to star this repo and follow me. I will make sure to bring out awesome deep learning projects like this in the future. Until the next time, サヨナラ!

###### PS: I am an anime fan ;)
