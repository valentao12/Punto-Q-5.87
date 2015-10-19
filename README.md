# Punto-Q-5.87
Further Analysis
% Script file: cont _ view

XY = linspace (-pi,pi,100);

YX = XY;

[X,Y] = meshgrid(XY,YX);

Z = sin(2.*Y).*cos(2.*X).*exp(-sqrt(X.^2+Y.^2)./2);

Figure (1) % contour plot

contour (X,Y,Z,13)

xlabel (‘X’), ylabel (‘Y’), zlabel (‘Z’)

title (‘Contour plot’)

figure (2) % view plots

subplot (2,2,1)

surf (X,Y,Z)

shading faceted

view (0,0);

xlabel (‘X’),ylabel (‘Y’), zlabel (‘Z’)

subplot (2,2,2)

surf (X,Y,Z)

shading faceted

view (90,0)

xlabel (‘X’),ylabel(‘Y’), zlabel(‘Z’)

subplot (2,2,3)

surf (X,Y,Z)

shading faceted

view (-37.5-90,0)

xlabel (‘X’),ylabel(‘Y’), zlabel(‘Z’)

subplot (2,2,4)

surf (X,Y,Z)

shading faceted

view (-37.5-45,0)

xlabel (‘X’),ylabel (‘Y’), zlabel (‘Z’)
