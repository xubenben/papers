### Distill knowledge
Many works including <Beyason dark knowledge> try to transfer "knowledge" from "teacher" to "student". \
I think the main idea here ia to consider knowledge as a "learned mapping from input vectors to output vectors" , and we know that NN can similate any functions. This is so-called ""Distilling the knowledge".
But Why do this?
Because in apllication, we don't really care how a model is trained. Efficiency is another key point.

### relative probabilities 
Another point I find intersting is that "The relative probabilities of incorrect answers tells a lot." For example, in MNIST task, one version of 2 may be given a probability of 10^(-6) for 3 and 10^(-9) for 7. This valuable information defines that\
3 is more similar of 2 than 7 in strcture. But this has little influence as the probabilities are so close to zero.

How to utilize this information? Use soft targets can help generalize.

### Specialist Models
This is awesome. When the number of classes is very large, complex model can be repalced by an ensemble model which contain a generalist model and many specialist models.

