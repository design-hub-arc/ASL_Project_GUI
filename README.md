# ASL_Project_GUI
Downloadable Python GUI for use of the ASL neural net  <br>
ASL PROJECT (PYTHON DOWNLOADABLE) WINDOWS INSTRUCTIONS <br>
Python version 3.8                                     <br>

files you need:                                                           <br>
(not in this repo) -'model.hdf5'        trained model (zipped as 'model') <br>
(not in this repo) -'DELETE'            test images folder (zipped)       <br>
(in this repo)     -'asl_PythonGUI.py'  GUI program                       <br>

	* Install Python3 with PIP, and GIT if not already installed.
		- https://www.python.org/downloads/
		- https://git-scm.com/downloads

	* Now let's make a directory for all of our work, models, and datasets to be stored. And go to it.
		- mkdir ASLProject
		- cd ASLProject

	* Clone the ASL-Net repository.. (you will need git installed for this)
		- git clone https://github.com/designhubarc/ASL-NET.git

	* Next let's get our dataset (used for testing only). Unzip and save it anywhere. 
	  - Remember where it is, because you will need to find this folder for testing.
	  (NOTE: this dataset will only be used for testing and the directory of the folder will be chosen by the user) 
		- folder of images called 'DELETE'

	* Next let's get our trained model. Unzip and move it to our ASLProject directory.
		- model.hdf5

	* Place testGUI.py it into the folder ASL-NET. 
		- This is the folder you will run testGUI.py from.

	* We need our Python dependencies installed with PIP
	  The command is 'pip3 install ...'
		- pip3 install numpy
			       matplotlib
			       tensorflow or tensorflow-gpu
			       tqdm
			       pyqt5

NOTE: If using a GPU, I believe you will need the CUDA toolkit.. 
      This part is much more complicated to setup, but here is the official what you need. 
      https://www.tensorflow.org/install/gpu


	* Finally, to test that it runs and produces a PDF, go into the folder ASL-NET and run asl_PythonGUI.py
		- give the PDF a name and select the DELETE folder for the images to process
		- choose a folder to store the results PDF
		- click grade
		- once the program finishes, there should be a PDF of results with the name you gave it in the folder you saved it to
