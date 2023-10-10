
# Military Vehicles Image Recognition

Military Vehicles Object detection from ARMA Game

The model is able to detect these classes
* CSAT Varsuk
* CSAT Marid
* CSAT Zamak (Transport)
![test_01](https://github.com/RsGoksel/Military-Vehicles-Detection/assets/80707238/99a730de-9310-4ce8-87d5-8a804d564a07)

The dataset used is available on [Kaggle](https://www.kaggle.com/datasets/gkselmech/arma-military-object-detection/data).

## Usage

1. Clone the repository

```bash
git clone https://github.com/RsGoksel/Military-Vehicles-Detection
```

2. Install requirements

```bash
pip install -r requirements.txt
```

3. Replace your images to the `source` folder

4. Run the model

```bash	
python detect.py --source ./input/ --weights runs/train/yolo_tr/weights/best.pt --conf 0.5 --name Arma_Detection
```

![Gif](https://github.com/RsGoksel/Military-Vehicles-Detection/assets/80707238/04856e5b-67a7-4979-8f7d-23966d34d969)


## Train

 1. Clone the repository

```bash
git clone https://github.com/RsGoksel/Military-Vehicles-Detection
```

2. Install requirements

```bash
pip install -r requirements.txt
```

3. Execute Data handling file if you got "xml" file format dataset version. If you downloaded mine, just create train-val folders.

4. Train a model

```bash	
python train.py --data './data.yaml' --epochs 10
```

