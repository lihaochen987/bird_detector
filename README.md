# bird_detector

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cBszWcDJP_9oe4K89GUhKjVMV5MxDXem?usp=sharing)

`bird.pt` are weights trained from Google Open Images for 300 epochs on a pre-trained YOLOv5 model. `ML_Workshop_Code.ipynb` includes the template code used to train bird.pt, as well as the code presented during the Machine Learning Workshop. `Slides Final.pdf` include the slides presented at the workshop.

The Machine Learning workshop is recorded through the link below (it is an hour long):

https://www.youtube.com/watch?v=YMpPSRhENe0



## Usage
To train your own weights through Google Open Images classes:

Note: `ML_Workshop_Code.ipynb` has not been tested on Jupyter Notebooks.

1. Access the notebook through the link: https://colab.research.google.com/drive/1cBszWcDJP_9oe4K89GUhKjVMV5MxDXem?usp=sharing

2. Create a new copy in your Google drive and change the `desired_class` variable to one of the variable available on the Google Open Images dataset. Disconnect and delete the runtime, then run all.



To access `bird.pt` trained weights:

1. Clone YOLOv5 into selected directory with:

   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   ```

2. Install YOLOv5 requirements with:

   ```bash
   pip install -r requirements.txt
   ```

3. Move `bird.pt` into the YOLOv5 cloned directory

4. Run the detection with:

   ```bash
   python3 detect.py --source 0 --weights bird.pt
   ```

   
