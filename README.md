These tests include two positive and two negative test cases:

The email is sent to recipient without/with picture attached, the size of the picture exceeds 35mb, to incorrect email.


**To run tests you have to:**

1) Activate Less secure app access = ON in your account

2) The interface of your gmail account should be in English

3) Run docker image with the preferable name 
	**docker build -t your_image_name .**
	
4) Add the image name, login and password from your gmail account in docker-compose.yml 
(image, EMAIL_ADDRESS, EMAIL_PASS)

5) Run tests by script:
	**docker-compose up**
	
6) To see the report, implement the following script:
	**allure serve ./allure_report**