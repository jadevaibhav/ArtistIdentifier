# Artist Identification Using CNNs
## Neural Networks and Fuzzy Logic Course Project

## Team:
1.Vaibhav Sanjay Jade 
2.Samiran Gode 
3.Pratyush Dubey 
4.Mayank Mundada

Owing to space constraints (maximum size of the zip file that could be uploaded was 10 MB), we have deleted all the data files, trained models, and pickled data structures. Only the code, script and result files are present in the zip file uploaded. We are currently preparing dataset which would be uploaded on drive and link would be provided soon.

## Resources:
http://cs231n.stanford.edu/reports/2017/pdfs/406.pdf

(for siamese networks)https://github.com/jadevaibhav/Signature-verification-using-deep-learning

## Dataset:
We are working with much smaller dataset than original 'Painters by numbers', provided by Kaggle. We have taken following 12 painters:
'Aleksey_Savrasov','Claude_Monet','Da_Vinci', 'Frida_Kahlo','Michelangelo','Pablo_Picasso','Paul_Cezanne', 'Pierre_Renoir', 'Rembrandt','Salvador_Dali','Van_Gogh', 'Wassily_Kandisky'. 

## Data Preprocessing
As mentioned in the above report, we are assuming the artistic features of a painter would present even if we take a slice of whole painting. As we are more concerned with Style(bush strokes, color-schemes etc) than the painting itself. We are taking a 224x224 slice from the images randomly.


