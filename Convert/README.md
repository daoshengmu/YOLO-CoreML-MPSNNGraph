
#### Convert the darknet pre-trained data to CoreML 

- Setup `darknet` python virtual environment

`virtualenv -p python3 darkflow_env`

`source darkflow_env/bin/activate`

- Install tensorflow and opencv

`pip install tensorflow opencv-python`

- Go to the `darkflow` folder and convert the weights to tensorflow pb file.

`python3 flow --model ../tiny-yolo-voc.cfg --load ../tiny-yolo-voc.weights --savepb`

`jupyter notebook`

- Launch Jupyter notebook `jupyter notebook` and open Convert_pb_coreml.ipynb, and run the script. After it finishes you will get `TinyYOLO.mlmodel`. Copy it to the Xcode project.