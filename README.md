<h1 align="center">Python List Slicing Cheatsheet 🐍</h1>
<p align="center">Collection of List slicing patterns for Python </p>


[![CC 4.0][license-image]][license-url]

[license-url]: http://www.wtfpl.net
[license-image]: https://img.shields.io/badge/License-WTFPL%202.0-lightgrey.svg?style=flat-square


## **Notations:**

```
list[:]             >> All        
list[Low:]          >> Low to End      
list[:High]         >> Begining to High
list[Low:High]      >> Low to High
list[::Step]        >> Start to End with Step
list[Low::Step]     >> Low to End with Step
list[:High:Step]    >> Start to High with Step
list[Low:High:Step] >> Low to High with Step
```
## **Example**

```python
list= ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I']
```
<p align="center"><img src="/list_image.png" alt=""></p>

***Simple***

```python
list[3]      >> 'D'
list[-3]     >> 'G'
list[:]      >> ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I']
list[3:]     >> ['D', 'E', 'F', 'G', 'H', 'I']
list[:3]     >> ['A', 'B', 'C']
list[-3:]    >> ['G', 'H', 'I']
list[:-3]    >> ['A', 'B', 'C', 'D', 'E', 'F']
```
***Double***
```python
list[-12:1]  >> ['A']
list[-12:3]  >> ['A', 'B', 'C']
list[-12:-3] >> ['A', 'B', 'C', 'D', 'E', 'F']
list[1:-8]   >> []
list[1:-11]  >> []
list[1:-6]   >> ['B', 'C']
list[2:6]    >> ['C', 'D', 'E', 'F']
```

***Double with step***
```python
list[2:7:4]  >> ['C', 'G']
list[2:7:5]  >> ['C']
list[2:7:2]  >> ['C', 'E', 'G']
list[1:8:2]  >> ['B', 'D', 'F', 'H']
list[-7:8:2] >> ['C', 'E', 'G']
```

***More variations***
```python
list[-1::]   >> ['I']
list[-3::]   >> ['G', 'H', 'I']
list[3::]    >> ['D', 'E', 'F', 'G', 'H', 'I']
list[::-1]   >> ['I', 'H', 'G', 'F', 'E', 'D', 'C', 'B', 'A']
list[::-4]   >> ['I', 'E', 'A']
list[::4]    >> ['A', 'E', 'I']
list[::-2]   >> ['I', 'G', 'E', 'C', 'A']
list[::2]    >> ['A', 'C', 'E', 'G', 'I']

```

***Even more variations***

```python
list[-7::2]  >> ['C', 'E', 'G', 'I']
list[-7::3]  >> ['C', 'F', 'I']
list[1::-1]  >> ['B', 'A']
list[1::-2]  >> ['B']
list[1::-7]  >> ['B']
list[6::-3]  >> ['G', 'D', 'A']
```

___
If you have any more patterns, ideas or suggestions, please share.

&copy; [Prasad Ostwal](https://ostwalprasad.github.io)


[![CC 4.0][license-image]][license-url]

[license-url]: http://www.wtfpl.net
[license-image]: https://img.shields.io/badge/License-WTFPL%202.0-lightgrey.svg?style=flat-square

