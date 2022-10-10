
# Human Detector from YOLOv5

[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)


"Human Detector from YOLOv5" sends an email when a person is detected from YOLOv5. The content of the email will be the text of the detection result and an attached image, as shown in the Demo. This may be useful, for example, when a fixed-point camera is installed in an off-limits area.

## Installation
Please refer to [YOLOv5](https://github.com/ultralytics/yolov5)

Python>=3.7.0 environment, including PyTorch>=1.7.

```bash
  git clone https://github.com/ultralytics/yolov5  # clone
  cd yolov5
  pip install -r requirements.txt  # install
```


## Usage
`detect.py` runs and activate human detection.

```
  python detect.py --source <dir_or_filepath> 
```

Before run `detect.py`, change settings as follows.

- Line: 60 `user = "<email Address From>"`
- Line: 61 `password = "<App pass>"`
- Line: 277 `sendMail('<email Address To>', path_img, mail_html)` 

For using Gmail, please get `<App pass>` from following:  
`Gmail Account > Security > Signing in to Google`



## Demo

![demo_human_detector](https://user-images.githubusercontent.com/73092523/194889561-c900cb03-071c-4f42-9766-7a0e2914c29c.png)


## Reference

 - [YOLOv5](https://github.com/ultralytics/yolov5)
 - [Integrating Python with Email Delivery](https://docs.oracle.com/en-us/iaas/Content/Email/Reference/python.htm)

