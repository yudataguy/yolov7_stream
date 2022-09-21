# YOLO v7 + Streaming 

## Steps

* Download yolov7 weights

```bash 
wget https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt
```

* Create python virtual environment

```bash
python3 -m venv venv
```

* Activate virtual environment

```bash
source venv/bin/activate
```

* Install requirements

```bash
pip install -r requirements.txt
```

* Run the script

```bash
python detect.py --weights yolov7.pt --conf 0.25 --img-size 640 --view-img --nosave --source 0
```

*0* is the webcam id. If you have multiple webcams, you can change it to 1, 2, etc.
You can use rtsp or http stream as well, replace 0 with url.

* Quit

Double press `q` in preview screen to quit the script
