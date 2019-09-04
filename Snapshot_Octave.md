
### In Octave

Change the style of cursor: PS1('>> ')  
Add ";" at the end of a line, could inhibit print.

Not Equal is\: ~=  
AND:  1 && 0  
OR:   1 || 0  

Control step size: v=1:0.1:2   
[val, ind] = max(a)  
All one matrix:  ones(2,3)  
All zero matrix: zeros(1,3)  
Random matrix:   rand(1,3)  
Unit matrix:     eye(3)  
Square array with equal horizontal and vertical addends: magic(3)  

sum(a)  
sum(A,1) based on column  
sum(A,2) based on line  
prod(a)  
floor(a) and ceil(a)  

Tricks:  
size(A)  size(A,1)  
The larger one of line and column: length(v)  
C = [A B] equals to C = [A, B]  
C = [A ; B]  
A .* B       A.^2      1./A        A .* eye(9)  
[r,c] = find(A >= 7)  
A .* eye(9)        sum(sum(A.* eye(9)))  
Variables in the current scope: who  
whos(tell the Size, Bytes and Class)  
clear feature all  

Save v as a name hello.mat: save hello.mat v  
save hello.txt v -ascii % save as text (ASCII)  
load data: load featuresZ.dat / load('featuresX.dat')  

Put all elements of A into a single vector: A( : )  
C = [A B]/C = [A , B]      C = [A ; B]  

Choose the largest of each column: max(A, [ ], 1)  
Choose the largest of each line:   max(A, [ ], 2)  
Choose the largest element: max(max(A))or max(A(:))  

Pseudoinverse matrix: pinv(A)  

plot(t,y1)    plot(t,y2,'r')  
xlabel('time')    ylabel('value')  
legend('sin', 'cos')  
title('my plot')  
cd /Users/Glory/Desktop; print -dpng 'myPlot,png'  
figure(1); plot(t, y1)  
figure(2); plot(t, y2)  
Divides plot a 1\*2 grid, access first element: subplot(1,2,1)  
plot(t,y1)  
subplot(1,2,2)  
plot(t,y2)  
axis([0.5 1 -1 1])  
clf  
A = magic(5)    imagesc(A)  
imagesc(A), colorbar, colormap gray;  


```python
for i = 1:10,  
v(i) = 2^i;  
end;  

while i <= 5,  
v(i) = 100;  
i = i+1;  
end;  

if v(1) == 1,  
disp('The value is one');  
elseif v(i) == 2,  
disp('The value is two');  
else  
disp('The value is not one or two.');  
end;  

function y = squareThisNumber(x)  
y = x^2;  
function [y1,y2] = squareAndCubeThisNumber(x)  
y1 = x^2;  
y2 = x^3;  
```

