## پروژه تشخیص چهره (fa)

**شرح:**

این اسکریپت پایتون از طریق وب کم چهره ها را در زمان واقعی تشخیص می دهد و نام آنها را روی صفحه نمایش می دهد.

**نیازمندی های نصب:**

- پایتون 3
- کتابخانه OpenCV (`cv2`): `pip install opencv-python`
- کتابخانه SimpleFacerec: `pip install simple-facerec`

**پیش نیازها:**

- وجود یک پوشه به نام "images" در همان دایرکتوری اسکریپت که شامل تصاویر از پیش ذخیره شده افراد برای تشخیص است.

**دستورالعمل های اجرا:**

1. با استفاده از ترمینال به دایرکتوری اسکریپت بروید.
2. اسکریپت را اجرا کنید: `python main_video.py`

**عملکرد:**

- **رمزگذاری چهره ها:** اسکریپت به طور خودکار چهره ها را از تصاویر داخل پوشه "images" برای تشخیص رمزگذاری می کند.
- **بارگیری دوربین:** اسکریپت به وب کم شما دسترسی پیدا می کند.
- **تشخیص و تشخیص در زمان واقعی:** اسکریپت به طور مداوم فریم های ویدیویی را از وب کم تجزیه و تحلیل می کند.
  - چهره ها را در داخل فریم ها تشخیص می دهد.
  - چهره های شناخته شده را با مقایسه آنها با تصاویر رمزگذاری شده تشخیص می دهد.
  - مستطیل هایی را دور چهره های تشخیص داده شده می کشد.
  - نام های مربوطه را بالای هر مستطیل نمایش می دهد.
- **خروج:** برای خروج از اسکریپت کلید Esc (`key == 27`) را فشار دهید.

**عیب یابی:**

- **کتابخانه های گمشده:** اگر با خطاهای مربوط به کتابخانه های گمشده مواجه شدید، آنها را با استفاده از `pip` طبق دستورالعمل های "نیازمندی های نصب" نصب کنید.
- **مشکلات وب کم:** مطمئن شوید که وب کم شما کار می کند و قابل دسترسی است.
- **مشکلات تشخیص چهره:**
  - تأیید کنید که تصاویر در پوشه "images" به اندازه کافی روشن هستند و به طور واضح چهره افراد را نشان می 
  - اگر چهره ها به درستی تشخیص داده نمی شوند، برای تشخیص بهتر موقعیت خود را تنظیم کنید.

**اطلاعات اضافی:**

- برای سفارشی سازی و تنظیمات بیشتر، کتابخانه SimpleFacerec را بررسی کنید.


# FaceDetection(en)

 **README for main_video.py**

**Description:**

This Python script utilizes a webcam to detect and recognize faces in real-time, displaying their names on the screen.

**Installation Requirements:**

- Python 3
- OpenCV (`cv2`) library: `pip install opencv-python`
- SimpleFacerec library: `pip install simple-facerec`

**Prerequisites:**

- Ensure a folder named "images" is present within the same directory as the script, containing pre-saved images of individuals for recognition.

**Instructions to Run:**

1. Navigate to the script's directory using a terminal.
2. Execute the script: `python main_video.py`

**Functionality:**

- **Encode faces:** The script automatically encodes faces from images within the "images" folder for recognition.
- **Load camera:** The script accesses your webcam.
- **Real-time detection and recognition:** The script continuously analyzes video frames from the webcam.
  - Detect faces within the frames.
  - Recognize known faces by comparing them to the encoded images.
  - Draw rectangles around detected faces.
  - Display the corresponding names above each rectangle.
- **Exit:** Press the Esc key (`key == 27`) to terminate the script.

**Troubleshooting:**

- **Missing libraries:** If you encounter errors regarding missing libraries, install them using `pip` as mentioned in the Installation Requirements.
- **Webcam issues:** Ensure your webcam is functional and accessible.
- **Face recognition difficulties:**
  - Verify that images in the "images" folder are adequately illuminated and clearly show individuals' faces.
  - Reposition yourself for clearer recognition if faces are not properly detected.

**Additional Information:**

- Explore the SimpleFacerec library for further customization and configuration options.
