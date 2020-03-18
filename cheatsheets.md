1. 统一子图colorbar+设置刻度：
levels=np.linspace(-100,100,11)

im=m.contourf(x,y,slhf,cmap=cmap,levels=levels)
cbar=m.colorbar(im,'bottom',size=0.2,pad=0.3,label='W*m-2')
cbar.set_clim(-100,100)
cbar.set_ticks(np.linspace(-100,100,11))
cbar.set_ticklabels( ('-100', '-80', '-60','-40','-20','0','20','40','60','80','100'))  

