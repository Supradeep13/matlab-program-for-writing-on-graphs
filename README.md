# matlab-program-for-writing-on-graphs
This program allows use to write anything on a matlab graph at a specified position and specified length. 
clc;
close all;
clear all;
set(groot,'defaultLineLineWidth',4);
hold on;
Char=upper(input('Enter Name or Word','s'));
n=input('Enter X co-ordinate: ');
y=input('Enter Y co-ordinate: ');

l=input('Enter size of letters: ');
a=n;
k=0.8;
for i=Char
    switch i
    case 'A'
       A(n,y,l);
        n=n+k*l;
     case 'B'
        B(n,y,l);
         n=n+k*l;
    case 'C'
        C(n,y,l);
         n=n+k*l;
    case 'D';
        D(n,y,l);
         n=n+k*l;
    case 'E'
         E(n,y,l);
          n=n+k*l;
         case 'F'
         F(n,y,l);
          n=n+k*l;
    case 'G'
       G(n,y,l);
        n=n+l*k*1.5;
      case 'H'
          H(n,y,l);
         n=n+k*l;
    case 'I' 
        I(n,y,l);
         n=n+k*l;
        case 'J' 
        J(n,y,l);
        n=n+l*k*1.5;
     case 'K'  
         K(n,y,l);
         n=n+k*l;
      case 'L' 
          L(n,y,l);
         n=n+k*l;
       case 'M'
           M(n,y,l);
        n=n+l*k*1.5;
        case 'N'
            N(n,y,l);
         n=n+k*l;
        case 'O'
            O(n,y,l);
        n=n+l*k*1.5;
        case 'P'
            P(n,y,l);
        n=n+l*k/1.5;
       case 'Q'
            Q(n,y,l);
        n=n+l*k*1.5;
        case 'R'
          R(n,y,l); 
        n=n+l*k/1.5;
        case 'S'
       S(n,y,l);
         n=n+k*l;
        case 'T'
       T(n,y,l);
         n=n+k*l;
        case 'U'
       U(n,y,l);
        n=n+k*l;
        case 'V'
       V(n,y,l);
         n=n+k*l;
        case 'W'
       W(n,y,l);
        n=n+l*k*1.5;
        case 'X'
       X(n,y,l);
        n=n+l*k*1.5;
        case 'Y'
       Y(n,y,l);
         n=n+k*l;
        case 'Z'
       Z(n,y,l);
         n=n+k*l;
        otherwise
        n=n+l;
end  
end
axis([a-1 n+1 y-l-4 l+4])



function A(x,y,l)
x1=[x,x+l/4,x+l/2];
y1=[y-l,y,y-l];
x2=[x+l/8,l/8+l/4+x];
y2=[y-l/2,y-l/2];
plot(x1,y1,x2,y2);
end
function B(x,y,l)
    [x1,y1]=circle(x+l/4,y-3/4*l,l/4,-1);
    [x2,y2]=circle(x+l/4,y-1/4*l,l/4,-1);
    x3=[x+l/4 x x x+l/4];
    y3=[y y y-l y-l];
    x4=[x x+l/4];
    y4=[y-l/2 y-l/2];
    plot(x1,y1,x2,y2,x3,y3,x4,y4);
end  
function C(x,y,l)
    l=l/2;
    x=x+l;
    y=y-l;
    [x y]=circle(x,y,l,1);
plot(x,y);
end
function D(x,y,l)
    y=y-l/2;
    [x1,y1]=circle(x,y,l/2,-1);
    x2=[x x];
    y2=[y+l/2 y-l/2];
    X=[x1,x2];
    Y=[y1,y2];
    plot(X,Y);
end  
function E(x,y,l)
    x1=[x+l/2 x x x+l/2];
    y1=[y y y-l y-l];
    x2=[x x+l/2];
    y2=[y-l/2 y-l/2];
    plot(x1,y1,x2,y2);
end
function F(x,y,l)
    x1=[x+l/2 x x];
    y1=[y y y-l];
    x2=[x x+l/2];
    y2=[y-l/2 y-l/2];
    plot(x1,y1,x2,y2);
end
function G(x,y,l)
    [x1,y1]=curve(x+l/2,y-l/2,pi/4,3*pi/2,l/2);
    [x2,y2]=curve(x+l/2,y-3*l/4,-pi/2,pi/2,l/4);
    x3=[x2(end) x+l x+l];
    y3=[y2(end) y-l/2 y-l];
    X=[x1,x2,x3];
    Y=[y1,y2,y3];
    plot(X,Y);
    
end  

function H(x,y,l)
    x1=[x x];
    x2=[x x+l/2];
    y1=[y y-l];
    y2=[y-l/2 y-l/2];
    x3=[x+l/2 x+l/2];
    y3=[y y-l];
    plot(x1,y1,x2,y2,x3,y3);
end

function I(x,y,l)
    x1=[x x+l/2];
    y1=[y y];
    x2=[x+l/4 x+l/4];
    y2=[y y-l];
    x3=[x x+l/2];
    y3=[y-l y-l];
    plot(x1,y1,x2,y2,x3,y3)
end
function J(x,y,l)
 
  [x1,y1]=circle(x+3/8*l,y-5*l/8,3*l/8,-2);
  x2=[max(x1) max(x1)];
  y2=[max(y1) y];
  x3=[x1 x2];
  y3=[y1 y2];
  x4=[x x+l];
  y4=[y y];
  plot(x3,y3,x4,y4);
  
end
function K(x,y,l)
    x1=[x x];
    y1=[y y-l];
    x2=[x+l/2 x x+l/2];
    y2=[y y-l/2 y-l];
    plot(x1,y1,x2,y2);
end
function L(x,y,l);
    x=[x x x+l/2];
    y=[y y-l y-l];
    plot(x,y);
end
function M(x,y,l)
    x=[x x x+l/2  x+l x+l];
    y=[y-l y y-l y y-l];
    plot(x,y);
end
function N(x,y,l)
    X=[x x x+l/2 x+l/2];
    Y=[y-l y y-l y];
    plot(X,Y);
end
function O(x,y,l)
    l=l/2;
    x=x+l;
    y=y-l;
    [x1 y1]=circle(x,y,l,1);
    [x2 y2]=circle(x,y,l,3);
    x=[x1 x2];
    y=[y1 y2];
    plot(x,y);
end
function P(x,y,l)
[x1,y1]=circle(x,y-l/4,l/4,-1);
x2=[x x];
y2=[y-l y];
plot(x1,y1,x2,y2);
end
function Q(x,y,l)
    l=l/2;
    x=x+l;
    y=y-l;
    [x1 y1]=circle(x,y,l,1);
    [x2 y2]=circle(x,y,l,3);
    x3=[x x+l];
    y3=[y y-l];
    x=[x1 x2];
    y=[y1 y2];
    plot(x,y,x3,y3);
end
function R(x,y,l)
[x1,y1]=circle(x,y-l/4,l/4,-1);
x2=[x x];
y2=[y-l y];
x3=[x x+l/4];
y3=[y-l/2 y-l];
plot(x1,y1,x2,y2,x3,y3);
end
function S(x,y,l)  
    x1=x+l/4;
    y1=y-3*l/4;
    y2=y-l/4;
[a1,b1]=circle(x1,y1,l/4,-1);
[a2,b2]=circle(x1,y2,l/4,1);
l1=[max(a2) max(a2)+0.6*(max(a1)-max(a2))];
l2=[max(b2) max(b2)];
l3=[min(a1) min(a2)];
l4=[min(b1) min(b1)];
 plot(a1,b1,a2,b2,l1,l2,l3,l4);
end 
function T(x,y,l)
    x1=[x x+l/2];
    y1=[y y];
    x2=[x+l/4 x+l/4];
    y2=[y y-l];
    plot(x1,y1,x2,y2);
end
function U(x,y,l)
    [x1 y1]=circle(x+l/4,y-l*3/4,l/4,-2);
    x2=[min(x1) min(x1)];
    y2=[y max(y1)];
    x3=[max(x1) max(x1)];
    y3=[max(y1) y];
    X=[x2,x1,x3];
    Y=[y2,y1,y3];
    plot(X,Y);
   
end
function V(x,y,l)
    X=[x x+l/4 x+l/2];
    Y=[y y-l y];
    plot(X,Y);
end
function W(x,y,l)
    x1=[x x+l/4 x+l/2 x+3*l/4 x+l];
    y1=[y y-l y y-l y];
    plot(x1,y1);
end
function X(x,y,l)
    x1=[x x+l];
    y1=[y y-l];
    x2=[x x+l];
    y2=[y-l y];
    plot(x1,y1,x2,y2);
end
function Y(x,y,l)
    x1=[x x+l/4 x+l/4];
    y1=[y y-l/2 y-l];
    x2=[x+l/4 x+l/2];
    y2=[y-l/2 y];
    plot(x1,y1,x2,y2);
end
function Z(x,y,l)
    x1=[x x+l/2 x x+l/2];
    y1=[y y y-l y-l];
    plot(x1,y1);
end

function [xaxis,yaxis]=circle(x,y,r,angle)
    t=angle*pi/2:pi/20:pi+angle*pi/2;
    xaxis=r*cos(t)+x;
    yaxis=r*sin(t)+y;
end

    
function[xaxis,yaxis]=curve(x,y,staang,stoang,r);
    t=staang:pi/20:stoang;
    xaxis=r*cos(t)+x;
    yaxis=r*sin(t)+y;
end
