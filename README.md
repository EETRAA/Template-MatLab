# Template-MatLab
DSP-matlab templates
## mesh grid
> [x,y] = meshgrid(-10*pi:0.1:10*pi);
> 
> z = cos(x).*sin(y);
> 
> mesh(x,y,z),xlabel('x'),ylabel('y'),zlabel('z')
> ==%surf(x,y,z),xlabel('x'),ylabel('y'),zlabel('z'), make surface|surfc, surf, surfl, meshc, meshz==

## yet another func plot
> [x,y] = meshgrid(-2:0.1:2);
> 
> z = y.*exp(-x.^2-y.^2);
> 
> mesh(x,y,z),xlabel('x'),ylabel('y'),zlabel('z')

## dimensions plot3
> t = 0:pi/10:2*pi;
> 
> [X,Y,Z] = cylinder(1+sin(t));
> 
> surf(X,Y,Z),colormap('default');
> 
> axis square

## ezplot 

> ezplot(FUN2,[XMIN,XMAX,YMIN,YMAX]) 

## one figure, multi diagrams;

> figure(10)          ==% define figure==
> 
> subplot(2,2,1);     ==% subplot(x,y,n)x表示显示的行数，y表示列数，n表示第几幅图片==
>  
>plot(...);
> 
> subplot(2,2,2);
> 
> plot(...);
> 
> subplot(2,2,3);
> 
> plot(...);
> 
> subplot(2,2,4);
> 
> plot(...);

## multi figures, multi diagrams;
> figure(1);         ==% 第一个子图==
> 
> plot(...);
> 
> figure(2);         ==% 第二个子图==
> 
> plot(...);
> 
> figure(3);
> 
> plot(...);
> 
> figure(4);
> 
> plot(...);
