# AI-Udemy-Masterclass
Final product of a Udemy masterclass (not all of the code is mine, most comes from course).

The goal of this project was to create and train an ML model to drive a car along a track in the most efficient and time-saving way possible. By the end of the course,
I had enough code to run the model successfully, although I wouldn't recommend training the VAE if you have less than a few tbytes of unused storage space. 
Also note that traning the Full World Model could take up to a month to reach peak efficiency for the car and requires a lot of storage space as well.

Steps: 

1. Build the environment (env.py)
2. Generate VAE Data (extract.py)
3. Train the VAE (vae_train.py)
4. Generate RNN Data (series.py)
5. Train the RNN (rnn_train.py)
6. Train the Full World Model (train.py)
7. Run the model (model.py)

This can also be found in training_process.py
