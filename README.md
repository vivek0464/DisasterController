# DisasterController
Project for Codefundo++

## About
Possibility of natural disaster beforehand can act as a huge life saving tool for millions of people that die in these natural calamities,panic button in the case we are stuck in a disaster and automated damage control methodologies with the help of a single damage control platform can fasten the reconstruction as well as save lots of lives.
Due to time shortage our prediction tool will only be trained for floods as of now.

This will be 3 component mobile application consisting of:
1. DisasterPredictor(Only for floods as of now)
2. HelpMe Button
3. DamageControl

### DisasterPredictor
Artificial neural network(ANN) has been widely applied in flood forecasting and got good results.However,it can still not go beyond one or two hidden layers for the problematic non-convex optimization.Here we will try to integrate stacked autoencoders(SAE) and back propagation neural networks(BPNN) for the prediction of stream flow,which simultaneously takes advantages of the powerful feature representation capability of SAE and superior predicting capacity of BPNN.To further improve the non-linearity simulation capability,we first classify all the data into several catefories by K-means clustering.Then, multiple SAE-BP modules are adopted to simulate their corresponding categories of data.

The app will notify the user with the possibility of floods within 24 hours every time probability goes more than 50%.

Data Preparation:
We will predict the stream flow for next 6 hour by using data gathered in the previous years. To be more specific, we chose the flow data in flood periods from 1998 to 2010. 6482 samples of data from 1998 to 2008 are selected as training samples and 1676 samples in the remaining two years are used as testing samples. We utilize two hidden layers in SAE-BP model, whose number of unit are respectively 20 and 15. The number K of K-means 4.

Technologies: python,tensorflow,keras,react-native,nodejs,MySQL

### HelpMe Button
If you are stuck in a flood, click on this button and message with your current location will be sent via all messaging apps like whatsapp,messenger available in your phone to all the users connected to you.

Technologies: python,twilio API,react-native,nodejs,MYSQL

### NOTE:
If there is time still left after the completion of first 2 components,then we will proceed to the third component of the application.

### DamageController
We will build a single platform for the victims,that will collect donations,when the money reaches certain amount,partition the money received into various areas like for water bottles,food,medicines,sanitary napkins etc ,automatically purchase those stuffs from the online vendors and distribute them to the flood affected locations.

Technologies: react-native,nodejs,MySQL 

### To Contribue To The Project
There are lots of features that can be added to the application like predictions for other natural disasters such as cyclones,earthquakes etc ,refining the current model's predictions etc.

