# NST
Перенос стиля с 2х изображений
Используется предобученная модель vgg19.

style loss считается по 2м изображениям, доля каждого задается lamda

style_loss = styleA_loss * lamda + styleB_loss * (1 - lamda)
total_loss = content_weight * content_loss + style_weight * style_loss 

1. Первое изображение для переноса стиля: styleA 
![Кандинский](https://upload.wikimedia.org/wikipedia/commons/b/b4/Vassily_Kandinsky%2C_1913_-_Composition_7.jpg)

2. Второе изображение для переноса стиля: styleB 

![Хокусай](https://upload.wikimedia.org/wikipedia/commons/0/0a/The_Great_Wave_off_Kanagawa.jpg)
3. Изображение для переноса

![Tuebingen_Neckarfront](https://upload.wikimedia.org/wikipedia/commons/0/00/Tuebingen_Neckarfront.jpg)
4. Результат 

![Tuebingen_Neckarfront](https://github.com/albinail/NST/blob/master/result-3%20(1).png)
