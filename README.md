# Nexus-Info-CHATBOT
This project involves developing of a basic interactive chatbot for college enquiry using   a feedforward neural network which is implemented using Tensorflow/Keras.
Model Loading:

The load_model function from tensorflow.keras.models is used to load a pre-trained neural network model stored in the file 'chatbotmodel.h5'.
Prediction:

The predict_class function takes a user message as input, preprocesses it, and then uses the loaded neural network model to predict the intent of the message.
The bag-of-words representation of the message is generated using the bag_of_words function, and then fed into the neural network model for prediction.
The model predicts the probabilities of each intent class, and if the probability exceeds a certain threshold, the intent with the highest probability is chosen as the predicted intent.
Response Generation:

The predicted intent is used to retrieve a random response from the intents defined in the intents.json file.
The get_response function selects a random response associated with the predicted intent from the JSON file.
User Interaction Loop:

The code runs in a loop, continuously prompting the user for input and generating responses based on the predicted intent.
The loop continues until the user inputs "bye" or "Goodbye", at which point the program exits.
Overall, the chatbot system uses a feedforward neural network model for intent classification, where the input is represented using a bag-of-words approach, and responses are generated based on the predicted intent.




