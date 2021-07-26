### Figure
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
