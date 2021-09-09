### Python

1. Set colorbar range and the ticks

```
levels=np.linspace(-100,100,11)
im=m.contourf(x,y,slhf,cmap=cmap,levels=levels)
cbar=m.colorbar(im,'bottom',size=0.2,pad=0.3,label='W*m-2')
cbar.set_clim(-100,100)
cbar.set_ticks(np.linspace(-100,100,11))
cbar.set_ticklabels( ('-100', '-80', '-60','-40','-20','0','20','40','60','80','100'))  
```

2. To adjust the layout of the subplots automatically.

```
plt.tight_layout()
```

3. To make a pdf output more beautiful.

```
bbox_inches = 'tight'
```
4. Plot sequence

```
zorder = 10
```

### Linux

1. Linux - check file/folder size under the current directory

```
du -sh *
```

### Midway
1. open jupyter


```
/sbin/ip route get 8.8.8.8 | awk '{print $NF;exit}'
jupyter-notebook --no-browser --ip=......
```
