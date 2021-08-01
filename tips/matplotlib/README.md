### Subplots
- Create axes and fig in one go
```python
import matplotlib.pyplot as plt
fig, axes = plt.subplots(nrows=3, ncols=1)
```
- Figure level commands for subplots
```python
# Assign axes data
axes[0][0].plot(x,y)
axes[0][1].plot(a,b)

# Add titles and whatnot to a axes subplot
axes[0][1].set_ylabel("y 0 1")
axes[0][1].set_xlabel("x 0 1")
axes[0][1].set_title("xy 0 1")

# Add a title to the entire subplot
fig.suptitle("Figure level title")

# Config subplots to have good spacing
plt.tight_layout()

# Save the entire figure aka subplots
fig.savefig("new_subplots.png", bbox_inches="tight")
```
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
*Allows for multiple plots on one figure*
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
