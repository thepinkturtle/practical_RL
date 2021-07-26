### Figure
- Make a complete plot
```python
axes2 = fig.add_axes([0, 0, 1, 1])
# The array is coordinates map according [x, y, w, h]

axes2.plot(a,b)
axes2.set_xlim(1,2)
axes2.set_ylim(0,25)
axes2.set_xlabel('A')
axes2.set_ylabel('B')
axes2.set_title('My Plot')
```
