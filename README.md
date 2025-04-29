```
DAA Practical 
Day 05

Activity 01
Functional ATM simulation 
-------------------------



balance = 1000;

while true
  
    fprintf('\nATM Menu:\n');
    fprintf('1. Deposit\n');
    fprintf('2. Withdraw\n');
    fprintf('3. Balance Inquiry\n');
    fprintf('4. Exit\n');

    choice = input('Please select an option (1-4): ');


    switch choice
        case 1 
            amount = input('Enter amount to deposit: ');
            if amount > 0
                balance = balance + amount;
                fprintf('Deposit successful! New balance: %.2f\n', balance);
            else
                fprintf('Invalid amount. Please enter a positive value.\n');
            end
            
        case 2  
            amount = input('Enter amount to withdraw: ');
            if amount > 0
                if amount <= balance
                    balance = balance - amount;
                    fprintf('Withdrawal successful! New balance: %.2f\n', balance);
                else
                    fprintf('Insufficient funds! Your balance is: %.2f\n', balance);
                end
            else
                fprintf('Invalid amount. Please enter a positive value.\n');
            end
            
        case 3  
            fprintf('Your current balance is: %.2f\n', balance);
            
        case 4  
            fprintf('Thank you for using the ATM. Have a great day!\n');
            break;
            
        otherwise
            fprintf('Invalid selection. Please choose a valid option (1-4).\n');
    end
end



Activity 02
------------

marks = zeros(1, 5);


for i = 1:5
    marks(i) = input(sprintf('Enter marks for student %d (out of 100): ', i));
    
   
    if marks(i) >= 90 && marks(i) <= 100
        grade = 'A';
    elseif marks(i) >= 80 && marks(i) < 90
        grade = 'B';
    elseif marks(i) >= 70 && marks(i) < 80
        grade = 'C';
    elseif marks(i) >= 60 && marks(i) < 70
        grade = 'D';
    else
        grade = 'F';
    end
    
    fprintf('Student %d: Marks = %d, Grade = %s\n', i, marks(i), grade);
end


while true
    fprintf('\nMenu:\n');
    fprintf('1. Show all marks as a bar chart\n');
    fprintf('2. Show average marks\n');
    fprintf('3. Exit\n');
    
    choice = input('Please select an option (1-3): ');

    switch choice
        case 1 
            figure;
            bar(marks);
            xlabel('Student');
            ylabel('Marks');
            title('Student Marks');
            
        case 2 
            avg_marks = mean(marks);
            fprintf('Average Marks: %.2f\n', avg_marks);
            
        case 3
            fprintf('Thank you!.. Goodbye!\n');
            break;
            
        otherwise
            fprintf('Invalid selection. Please choose a valid option (1-3).\n');
    end
end


Activity 03
------------

num_voters = input('Enter the total number of voters: ');


votes = zeros(1, 4);


for i = 1:num_voters
    fprintf('\nVoting Menu:\n');
    fprintf('1. Candidate A\n');
    fprintf('2. Candidate B\n');
    fprintf('3. Candidate C\n');
    fprintf('4. Candidate D\n');
    
    choice = input(sprintf('Voter %d, enter your choice (1-4): ', i));
    
    switch choice
        case {1, 2, 3, 4}
            votes(choice) = votes(choice) + 1;
        otherwise
            fprintf('Invalid vote! Not counted.\n');
    end
end


fprintf('\nElection Results:\n');
fprintf('Candidate A: %d votes\n', votes(1));
fprintf('Candidate B: %d votes\n', votes(2));
fprintf('Candidate C: %d votes\n', votes(3));
fprintf('Candidate D: %d votes\n', votes(4));


[max_votes, winner_idx] = max(votes);
if sum(votes == max_votes) > 1
    fprintf('It is a tie!\n');
else
    fprintf('Winner: Candidate %c\n', char('A' + winner_idx - 1));
end


while true
    fprintf('\nVisualization Menu:\n');
    fprintf('1. Show Bar Chart of Votes\n');
    fprintf('2. Show Pie Chart of Votes\n');
    fprintf('3. Show Scatter Plot (creative visualization)\n');
    fprintf('4. Exit\n');
    
    viz_choice = input('Enter your choice: ');
    
    switch viz_choice
        case 1
            figure;
            bar(votes);
            title('Vote Count Bar Chart');
            xlabel('Candidates');
            ylabel('Number of Votes');
            xticklabels({'A', 'B', 'C', 'D'});
            grid on;
            
        case 2
            figure;
            pie(votes, {'Candidate A', 'Candidate B', 'Candidate C', 'Candidate D'});
            title('Vote Distribution Pie Chart');
            
        case 3
            figure;
            scatter(1:4, votes, 100, 'filled');
            title('Scatter Plot of Votes');
            xlabel('Candidates');
            ylabel('Number of Votes');
            xticks(1:4);
            xticklabels({'A', 'B', 'C', 'D'});
            grid on;
            
        case 4
            fprintf('Exiting visualization menu.\n');
            break;
            
        otherwise
            fprintf('Invalid choice! Try again.\n');
    end
end
















