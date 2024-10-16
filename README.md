# tamrin_mabanibinayiii
import numpy as np
import cv2
# ابعاد تصویر
width, height = 400, 400
# ایجاد تصویر خالی
gradient_image=np.zeros((height, width, 3),dtype=np.uint8)
#رنگها 
color1 = np.array([255, 0, 0])
#قرمز
color2 = np.array([0, 0, 255])
#آبی
# ایجاد گرادینت
for i in range(width

# محاسبه نسبت برای ایجاد رنگ
شیب دار
ratio = i / (width - 1)
gradient_color= (1 - ratio) *color1 + ratio * color2gradient_image[:, i] =gradient_color
# نمایش تصویر
cv2.imshow('Gradient Image',gradient_image)
cv2.waitKey(0)
()cv2.destroyAllWindows
