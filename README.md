# AI-Udemy-Masterclass
Final product of a Udemy masterclass (not all of the code is mine, most comes from course).

The goal of this project was to create and train an ML model to drive a car along a track in the most efficient and time-saving way possible. By the end of the course,
I had enough code to run the model successfully, although I wouldn't recommend training the VAE if you have less than a few tbytes of unused storage space. 
Also note that traning the Full World Model could take up to a month to reach peak efficiency for the car and requires a lot of storage space as well.

GENERAL STEPS: 

1. Build the environment (env.py)
2. Generate VAE Data (extract.py)
3. Train the VAE (vae_train.py)
4. Generate RNN Data (series.py)
5. Train the RNN (rnn_train.py)
6. Train the Full World Model (train.py)
7. Run the model (model.py)

This can also be found in training_process.py

The training utilizes CMA because there are less than 1000 parameters but should you want to train on more paremeters (in the thousands) all you need to do is 
navigate to train.py, locate line 405 and change 'default' from 'cma' to 'pepg' as well as change 'optimizer' on line 26 from 'cma' to 'pepg.'

TO INSTALL PACKAGES FOLLOW THESE STEPS: 

In your command ine - 
  conda create -n masterai python=3.6       #note that this model runs smoother on 3.6 than 3.7
  conda activate masterai
  conda install -c install-forge tensorflow
  python -m pip install cma
  conda install -c kna pybox2d
  pip install pillow 
  pip install gym == 0.9.4
  
 
ANACONDA IS RECOMMENDED
When in the anaconda homescreen toggle "Applications" to material and install Spyder, then navigate to AI Masterclass files and good luck!



