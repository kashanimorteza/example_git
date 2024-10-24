<!---------------------------------------[Description]-->
## Description
    This is a example of git



<!---------------------------------------[Install]-->
<br><br>

## Concept 

گیت یک مخزن (repository) می سازه که از سه لایه منطقی به فایل ها نگاه میکنه :
<br>
1 – لایه اول یا همان (working tree) که هنوز اقدامی برای ثبت تغییرات انجام نشده و فایل ها در حال تغییر هستند 
<br>
2 – لایه دوم یا همان (stage)که با وارد کردن فایل ها به این لایه، آنها آماده ثبت تغییر می شوند
<br>
3 – لایه سوم (Repository) که تمام تغییرات فایل ها ثبت می شوند
</div>
<br>
<div align="right" dir="rtl">
fork کردن در واقع یعنی یه کپی از پروژه گرفتن و تغییر دادنش
<br>
میشود از سازندش در خواست کرد تغیییرات رو ببینه و با پروژه اصلی خودش مرج کنه




<!---------------------------------------[Python]-->
<br><br>

## Python

#### Install
    add-apt-repository ppa:deadsnakes/ppa
	apt update -y
	apt install python3 -y
	apt install python3-pip -y
	apt install python3-venv -y

#### Virtual environment 
	python3 -m venv .myenv3
	.myenv3/bin/python3 -m pip install --upgrade pip
	source .myenv3/bin/activate
	pip install -r requirements.txt



<!---------------------------------------[WebApi]-->
<br><br>

## WebApi

#### Run simple
	fastapi run api.py

#### Run With uvicorn (HTTP)
    uvicorn api:app --host 127.0.0.1 --port 8000

#### Run With uvicorn (HTTPS)
	Create SSl
	----------------
	openssl req -x509 -newkey rsa:2048 -keyout key.pem -out cert.pem -nodes
    
	Run
	----------------
	uvicorn api:app --host 127.0.0.1 --port 8000 --ssl-keyfile=key.pem --ssl-certfile=cert.pem

#### Run With Nginx (HTTP)
	...

#### Run With Nginx (HTTPS)
	...

#### Chrome
	http://127.0.0.1:8000

#### Doc
	http://127.0.0.1:8000/docs

<!---------------------------------------[Structure]-->
<br><br>

## Structure
	Api
	Route
	Service
	Logic
	Model

<!---------------------------------------[Example]-->
<br><br>

## Example
	simple example : model_a

