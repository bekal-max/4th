i= imread('lena.png');
n= imnoise(i,'salt $ pepper');
f= ones(3,3)/9;
s= imfilter(n,f);
subplot(2,2,1), imshow(s); subplot(2,2,2), imshow(n);subplot(2,2,3), imshow(i);
subplot(2,2,1), imhist(s); subplot(2,2,2), imhist(n);subplot(2,2,3), imhist(i);
