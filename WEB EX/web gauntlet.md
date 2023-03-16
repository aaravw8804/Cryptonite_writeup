so first i inserted admin as both username and password but that did not work 
however i got the following query  ```  SELECT * FROM users WHERE username='admin' AND password='pass' ```
in SQL this command returns to the user the username and password that he had initiallly entered
since we do not know the password we change the part of the query from AND into a comment using --
so the query becomes ```  SELECT * FROM users WHERE username='admin'-- AND password='pass' ```
so we can now use username admin'-- and password of our choice

then we enter round two 
in round two we remove the -- because we cannot use the - comment 
but in the query we change admin'-- to admin';
this is because after ; everything is another statement 
so we use admin'; for both round two and three 

now in round 4 we cannot use admin as the username 
therefore we divide 'admin' into two parts and concatenate those parts using '||'
therefore the username becomes ad'||'min';
this helps us to get into round 5 

now i saw that the previous username can also be used for round 5
after this when we open the php file we get a block of text with the required flag at the end 
