# Number Plate Recognition & Reader
## Demo


https://github.com/Sovik-Gupta/Numberplate_recognition_reading/assets/27665277/51bf4b7e-2264-4d8a-bbd0-2aeccf2f79f8







## Model

1) A Yolov8 pre-trained model (YOLOv8n) to detect cars/truck/bus

2) A LPD(Licensed Plate Detector) reads the plate adn captures the image. 
- The LPD model is available [here](https://drive.google.com/file/d/1Zmf5ynaTFhmln2z7Qvv-tgjkWQYQ9Zdw/view?usp=sharing).

## Dependencies

PLease download the sort model from [this repository](https://github.com/abewley/sort).

## Project Setup

* Make an environment with python=3.8 using the following command 
``` bash
conda create --name .venv
```
* Activate the environment
``` bash
conda activate .venv
``` 

* Install the dependencies using the following command 
```bash
pip install -r requirements.txt
```
* Run main.py with your respective Video and it will cerate a test.csv
``` python
python main.py
```
* Run the add_missing_data.py file for interpolation of values to match up for the missing frames and smooth output.
```python
python add_missing_data.py
```

* Finally run the visualize.py passing in the interpolated csv files and hence obtaining a smooth output for license plate detection.
```python
python visualize.py
```
