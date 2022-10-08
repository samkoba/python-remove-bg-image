# python-remove-bg-image

```python
#Install the rembg module first
pip install rembg
```
```python
#the process of removing background from input and output state
from rembg import remove
from PIL import Image
input_path = 'assets/travelkoba-python.jpg'
output_path = 'assets/travelkoba-python-rembg.png'
input = Image.open(input_path)
output = remove(input)
output.save(output_path)
```


```python
#display the results before and after processing
from IPython.display import Image
from IPython.display import display
x = Image(filename='assets/travelkoba-python.jpg', width=200) 
y = Image(filename='assets/travelkoba-python-rembg.png', width=200) 
display(x, y)
```

Output before & after
<br>
<img height="148px" src="https://user-images.githubusercontent.com/7510963/194719360-214ca88c-cfc0-414f-a3dc-706856fcdba8.jpg" /> <img height="148px" src="https://user-images.githubusercontent.com/7510963/194719715-03fedda1-af85-4b7c-b23c-88176c2e4004.png" />

    

