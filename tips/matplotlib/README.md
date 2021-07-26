### Figure
- Just using `plot aka plt`
```python
plt.plot(x,y)
plt.title('String Title')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.xlim(0,max(x))
plt.ylim(0,max(y))
plt.savefig('myfirstplot.png')
plt.show()
```

### Figure with Axes 
*Allows for multiple plots on one figure
- Make a complete plot
```python
axes = fig.add_axes([0, 0, 1, 1])
# The array is coordinates map according [x, y, w, h]

axes.plot(a,b)
axes.set_xlim(0, 10)
axes.set_ylim(0, 10)
axes.set_xlabel('A')
axes.set_ylabel('B')
axes.set_title('My Plot')
```
- Inlay a plot on another plot by using the same `fig`
```python 
axes2 = fig.add_axes([1,2, .25, .25])
# if using the same fig as above
```
- Save a plot complete example
```python
fig = plt.figure(dpi=400, figsize=(2,2))
axes = fig.add_axes([0,0,1,1])
axes.set_xlabel('A')
axes.set_ylabel('B')
axes.set_title('My Title bro')
axes.plot(a,b)

#bbox_inches make it include the axes and labels
fig.savefig('new_figure.png', bbox_inches="tight")
```
