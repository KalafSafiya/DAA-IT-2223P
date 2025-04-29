# DAA-IT-2223P
Design and Analysis of Algorithms Practical
Day 01

Scalar Operations
-----------------
a = 5;
b = 3;
c = 8;

a + b;  % Addition
a - b;  % Subtraction
a * b;  % Multiplication
a / b;  % Division

Matrix and Array Operations
---------------------------
A = [1234];  % A scalar array

B = [2; 3; 4];  % Column vector

C = [5 4 1; 1 3 4; 7 8 9];  % 3x3 matrix

size(C);   % Size of matrix C
numel(C);  % Number of elements in C

sum(C, 1);  % Column-wise sum
sum(C, 2);  % Row-wise sum

min(C);    % Minimum element of C
min(min(C));  % Minimum element of C (alternative method)

max(C);    % Maximum element of C
max(max(C));  % Maximum element of C (alternative method)

C(2);      % Accessing the second element of C (linear indexing)
C(2, 1);   % Accessing the element at row 2, column 1 of C
C(1, :);   % Accessing the first row of C
C(:, 2);   % Accessing the second column of C
C(1, end); % Accessing the last element of the first row of C
C(end:-1:2);  % Accessing rows from the last to the second row in reverse order


Matrix Operations
-----------------
P = [1 2 3 4; 5 6 7 8; 9 1 2 3; 8 3 4 5];
Q = [4 3 2 1; 8 7 6 5; 3 2 1 9; 5 4 3 8];

P + Q;  % Matrix addition
P - Q;  % Matrix subtraction
P * Q;  % Matrix multiplication

P + 5;  % Scalar addition to each element of P
P .* Q; % Element-wise multiplication of matrices P and Q

[P Q];  % Concatenating matrices P and Q horizontally
[P; Q]; % Concatenating matrices P and Q vertically


Creating Matrices
-----------------
S = zeros(4, 3);  % 4x3 matrix of zeros
T = ones(2, 3);   % 2x3 matrix of ones


Conditional Statements and Loops
--------------------------------
num = 4;
if num > 0
    disp('The number is positive')
else
    disp('The number is negative')
end

i = 1;
while i <= 5
    disp(i)
    i = i + 1;
end



